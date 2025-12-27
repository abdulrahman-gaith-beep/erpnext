# Forking and Customizing ERPNext - Complete Guide

This guide will help you fork this ERPNext repository and customize it for your own needs while keeping the original repository intact and maintaining the ability to sync updates.

> **Can I make it private?** YES! See [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md) for complete details on keeping your fork private.

## Table of Contents
1. [Understanding the Setup](#understanding-the-setup)
2. [Quick Start - Fork Setup](#quick-start---fork-setup)
3. [Repository Privacy Options](#repository-privacy-options)
4. [Customization Strategy](#customization-strategy)
5. [Step-by-Step Customization](#step-by-step-customization)
6. [Maintaining Your Fork](#maintaining-your-fork)
7. [Important Legal Considerations](#important-legal-considerations)

---

## Understanding the Setup

### Current Repository
- **Original Upstream**: `frappe/erpnext` (main ERPNext project)
- **This Repository**: `abdulrahman-gaith-beep/erpnext` (already a fork)
- **License**: GPL-3.0 (allows forking and modification)
- **Framework**: Built on Frappe Framework

### What You Can Do
✅ Fork this repository to your own account  
✅ Modify the code for your needs  
✅ Use it commercially (under GPL-3.0 terms)  
✅ Keep your changes private or make them public  
✅ Create your own branded version  

### What You Should NOT Do
❌ Use "ERPNext" trademark in your product name without permission  
❌ Remove or modify the GPL-3.0 license  
❌ Claim the original work as yours  
❌ Remove copyright notices from the original code  

---

## Quick Start - Fork Setup

### Option A: Fork This Repository (Recommended)
If you want to use this repository as your base:

```bash
# 1. Fork via GitHub UI
# Go to: https://github.com/abdulrahman-gaith-beep/erpnext
# Click "Fork" button in top-right
# Choose your account/organization

# 2. Clone YOUR fork
git clone https://github.com/YOUR-USERNAME/erpnext.git
cd erpnext

# 3. Add this repo as a remote (optional, for syncing)
git remote add upstream https://github.com/abdulrahman-gaith-beep/erpnext.git

# 4. Add original ERPNext as another remote (optional, for major updates)
git remote add erpnext-upstream https://github.com/frappe/erpnext.git

# Verify remotes
git remote -v
```

### Option B: Fork Original ERPNext
If you want to fork directly from the original ERPNext:

```bash
# 1. Fork via GitHub UI
# Go to: https://github.com/frappe/erpnext
# Click "Fork" button

# 2. Clone YOUR fork
git clone https://github.com/YOUR-USERNAME/erpnext.git
cd erpnext

# 3. Add original as upstream
git remote add upstream https://github.com/frappe/erpnext.git
```

---

## Repository Privacy Options

### Can I Make My Fork Private?

**YES!** ✅ You can make your fork private, especially for internal company use.

**Quick Steps to Make Private:**
1. After forking, go to your repository on GitHub
2. Click **Settings** → **General** → scroll to **Danger Zone**
3. Click **Change repository visibility**
4. Select **Make private**
5. Confirm the change

**Important Considerations:**
- ✅ Private repository is **allowed** for internal company use
- ✅ You don't have to share your code if using internally
- ⚠️ If you distribute the software to others, you must provide source code
- ⚠️ GPL-3.0 license still applies even if repository is private

**For Complete Details:**
See [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md) for:
- When you can keep code private
- When you must share code
- SaaS/cloud service considerations
- Legal compliance requirements
- Detailed scenarios and examples

---

## Customization Strategy

### 1. Create Your Own Branch
Always work on a custom branch to keep main clean for syncing:

```bash
# Create and switch to your custom branch
git checkout -b custom/my-company-erp

# Or create version-specific branch
git checkout -b custom/v16-mycorp
```

### 2. What to Customize

#### A. Branding & Identity
- Company name
- Logo and icons
- Color scheme
- Application title
- Email templates
- Print formats

#### B. Configuration
- Package metadata (`package.json`, `pyproject.toml`)
- Application configuration
- Default settings
- Repository URLs

#### C. Features
- Add custom modules
- Modify existing modules
- Remove unwanted features
- Add integrations

#### D. Infrastructure
- Deployment scripts
- Docker configurations
- CI/CD pipelines
- Environment variables

---

## Step-by-Step Customization

### Step 1: Update Package Metadata

#### A. Update `package.json`
```json
{
  "name": "your-company-erp",
  "description": "Your Company's ERP System based on ERPNext",
  "repository": {
    "type": "git",
    "url": "git+https://github.com/YOUR-USERNAME/your-erp.git"
  },
  "homepage": "https://yourcompany.com/erp",
  "author": "Your Company Name",
  "license": "GPL-3.0",
  "bugs": {
    "url": "https://github.com/YOUR-USERNAME/your-erp/issues"
  }
}
```

#### B. Update `pyproject.toml`
```toml
[project]
name = "your-company-erp"
authors = [
    { name = "Your Company Name", email = "dev@yourcompany.com"}
]
description = "Your Company's ERP System based on ERPNext"

[project.urls]
Homepage = "https://yourcompany.com/erp"
Repository = "https://github.com/YOUR-USERNAME/your-erp.git"
"Bug Reports" = "https://github.com/YOUR-USERNAME/your-erp/issues"
```

### Step 2: Rebrand the Application

#### A. Update Application Name
Look for configuration files in the `erpnext` directory:
- `erpnext/hooks.py` - Application hooks and configuration
- `erpnext/__init__.py` - Main initialization

#### B. Update README.md
Create your own README that:
- Describes YOUR system
- Credits ERPNext as the base
- Provides YOUR installation instructions
- Lists YOUR custom features

Example:
```markdown
# Your Company ERP

A customized ERP system based on ERPNext, tailored for [your industry/use case].

## Based On
This project is built on top of [ERPNext](https://github.com/frappe/erpnext), 
a powerful open-source ERP system licensed under GPL-3.0.

## Custom Features
- Feature 1
- Feature 2
- Feature 3

## Installation
[Your installation instructions]

## License
GPL-3.0 (inherited from ERPNext)

## Credits
- Original ERPNext: https://github.com/frappe/erpnext
- Frappe Framework: https://github.com/frappe/frappe
```

### Step 3: Add Custom Modules

Create your own modules in the `erpnext` directory:

```bash
# Create custom module directory
mkdir -p erpnext/custom_module

# Add your custom code
# - Custom doctypes
# - Custom reports
# - Custom dashboards
# - Custom integrations
```

### Step 4: Modify UI/Branding

#### A. Update Logo and Icons
Replace files in `erpnext/public/images/`:
- Logo files
- Favicon
- App icons

#### B. Update Color Scheme
Modify CSS/SCSS files for your brand colors.

#### C. Update Email Templates
Customize email templates in the system to reflect your branding.

### Step 5: Configure Development Environment

Create a `.env` or configuration file for your custom settings:

```bash
# .env.example
APP_NAME="Your Company ERP"
COMPANY_NAME="Your Company"
SUPPORT_EMAIL="support@yourcompany.com"
```

### Step 6: Update Documentation

Create/update these files:
- `CUSTOMIZATION_NOTES.md` - Document your changes
- `DEPLOYMENT.md` - Your deployment process
- `CONTRIBUTING.md` - Your contribution guidelines

---

## Maintaining Your Fork

### Syncing with Upstream

#### Get Updates from Original Repository
```bash
# Fetch updates from upstream
git fetch upstream

# Or from original ERPNext
git fetch erpnext-upstream

# View changes
git log HEAD..upstream/develop

# Merge into your branch (be careful!)
git merge upstream/develop

# Or cherry-pick specific commits
git cherry-pick <commit-hash>
```

#### Handling Conflicts
When merging updates:
1. Review conflicts carefully
2. Keep your customizations
3. Integrate new features selectively
4. Test thoroughly after merging

### Best Practices

#### 1. Keep Changes Modular
- Use inheritance and extensions
- Avoid modifying core files when possible
- Create custom modules instead of editing existing ones

#### 2. Document Everything
```python
# Add comments to modified files
# Original ERPNext code - Modified for [purpose]
# Modified by: [Your Name]
# Date: [Date]
# Reason: [Why you changed it]
```

#### 3. Version Control Strategy
```bash
# Tag your releases
git tag -a v1.0.0-custom -m "Custom version 1.0.0"
git push origin v1.0.0-custom

# Keep branches organized
# main/develop - clean upstream copy
# custom/develop - your development branch
# custom/production - your production branch
```

#### 4. Testing
- Test all customizations thoroughly
- Create custom test suites
- Test after merging upstream changes

---

## Important Legal Considerations

### GPL-3.0 License Compliance

Since ERPNext is GPL-3.0, you MUST:

✅ **Keep the GPL-3.0 license** - Don't change it  
✅ **Include original copyright notices**  
✅ **Make source code available** if you distribute the software  
✅ **License your modifications under GPL-3.0** as well  
✅ **Document your changes** clearly  

### Trademark Considerations

From the ERPNext Trademark Policy:

🚫 **Cannot use "ERPNext" in:**
- Your product name
- Your company name
- Your domain name (as main identifier)
- Your logo/branding

✅ **Can mention ERPNext:**
- In documentation: "Based on ERPNext"
- In descriptions: "Powered by ERPNext"
- In about pages: "Built on ERPNext technology"

### Recommended Approach

```markdown
# Good Examples:
- "Acme ERP (based on ERPNext)"
- "CustomERP - Powered by ERPNext technology"
- "Your Company's ERP System built on ERPNext"

# Bad Examples (don't use):
- "Acme ERPNext"
- "ERPNext for Manufacturing"
- "ERPNext Pro"
```

---

## Repository Protection

### Protecting Original Repository

Don't worry! When you fork:
- ✅ Original repo stays completely unchanged
- ✅ You can't accidentally push to original
- ✅ All your changes are in YOUR fork
- ✅ Original maintainer controls their repo

### Setting Up Protection

```bash
# Verify you can't push to upstream
git remote -v

# origin should point to YOUR repo
# upstream should point to original (fetch only)

# If you want extra safety, make upstream fetch-only:
git remote set-url --push upstream DISABLE_PUSH

# Now this will fail (as intended):
git push upstream  # Error: invalid remote
```

---

## Quick Start Checklist

Use this checklist when setting up your fork:

- [ ] Fork repository to your account
- [ ] Clone your fork locally
- [ ] Add upstream remotes
- [ ] Create custom branch
- [ ] Update `package.json` with your info
- [ ] Update `pyproject.toml` with your info
- [ ] Update README.md with your project info
- [ ] Replace logos and branding
- [ ] Create custom modules directory
- [ ] Document your customizations
- [ ] Set up development environment
- [ ] Test basic functionality
- [ ] Create your first custom feature
- [ ] Tag your first release
- [ ] Set up CI/CD for your fork
- [ ] Create deployment documentation

---

## Getting Help

### Resources
- **Privacy & Licensing Guide**: [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md)
- **ERPNext Documentation**: https://docs.erpnext.com/
- **Frappe Framework Docs**: https://frappeframework.com/docs
- **ERPNext Forum**: https://discuss.frappe.io/
- **Your Fork Issues**: Create issues in YOUR repository

### Community
- Join ERPNext community forums
- Ask questions about customization
- Share your custom modules (if open source)
- Contribute improvements back to ERPNext (optional)

---

## Example Workflow

Here's a complete example of forking and customizing:

```bash
# 1. Fork on GitHub (click Fork button)

# 2. Clone your fork
git clone https://github.com/YOUR-USERNAME/your-erp.git
cd your-erp

# 3. Set up remotes
git remote add upstream https://github.com/abdulrahman-gaith-beep/erpnext.git
git remote add erpnext-upstream https://github.com/frappe/erpnext.git

# 4. Create custom branch
git checkout -b custom/production

# 5. Make your changes
# - Edit package.json
# - Edit pyproject.toml
# - Update README.md
# - Add custom modules
# - Update branding

# 6. Commit your changes
git add .
git commit -m "Initial customization: rebrand and configure for Your Company"

# 7. Push to your fork
git push origin custom/production

# 8. Continue development on this branch
git checkout -b custom/feature/new-module
# ... make changes ...
git commit -m "Add custom inventory module"
git push origin custom/feature/new-module

# 9. Merge features to production
git checkout custom/production
git merge custom/feature/new-module
git push origin custom/production

# 10. Tag releases
git tag -a v1.0.0 -m "First production release"
git push origin v1.0.0
```

---

## Summary

You now have a complete guide to:
1. ✅ Fork ERPNext safely without affecting the original
2. ✅ Customize it for your needs
3. ✅ Maintain your fork with updates
4. ✅ Stay compliant with licenses and trademarks
5. ✅ Organize your custom development

**Remember**: This is YOUR fork now. You can modify it however you want, as long as you comply with the GPL-3.0 license and trademark policies!

---

**Need more help?** Create an issue in your fork's repository or consult the ERPNext community forums.
