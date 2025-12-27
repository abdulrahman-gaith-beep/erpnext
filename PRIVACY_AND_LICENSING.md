# Privacy and Licensing Guide for Your Fork

This document explains your options for keeping your ERPNext fork private or public, and the legal implications of each choice.

## Quick Answer

**YES, you CAN make your fork private!** ✅

However, there are important considerations based on the GPL-3.0 license and how you use the software.

---

## Privacy Options

### Option 1: Private Repository (GitHub)

You can absolutely keep your fork in a **private GitHub repository**:

```bash
# When forking on GitHub:
1. Click "Fork" button
2. Uncheck "Copy the develop branch only" if you want all branches
3. After fork is created, go to Settings → General → Danger Zone
4. Click "Change repository visibility"
5. Select "Make private"
6. Confirm the change
```

**Important**: Even if your repository is private, you still need to comply with GPL-3.0 license terms (see below).

### Option 2: Keep Fork Public

Your fork can remain public if you want to:
- Share your customizations with others
- Get community contributions
- Show off your work
- Build a product ecosystem

---

## GPL-3.0 License: What You MUST Know

ERPNext is licensed under **GPL-3.0**, which has specific rules:

### ✅ You CAN Keep Code Private IF:

**1. Internal Use Only**
- You use it only within your company/organization
- You don't distribute the software to anyone outside
- Your employees use it internally
- You DON'T sell access to the software as a service

**Example Scenarios (Private OK)**:
- ✅ Running ERP for your own business
- ✅ Using it for your company's internal operations
- ✅ Your employees accessing it on company network
- ✅ Hosting on your own servers for your own use

**In these cases:**
- ✅ Repository can be private
- ✅ Code can stay private
- ✅ You don't have to share your modifications
- ✅ You can keep it secret forever

### ❌ You MUST Make Code Public IF:

**1. You Distribute the Software**
- You give/sell the software to other people/companies
- You provide the software as a product to customers
- You deploy it for clients

**2. You Offer Software as a Service (SaaS)** ⚠️
This is a **gray area** in GPL-3.0:
- Traditional GPL-3.0: Might not require source disclosure for SaaS
- AGPL (different license): Would require disclosure
- Best practice: Consult a lawyer if doing SaaS

**In these cases:**
- ❌ Must provide source code to recipients
- ❌ Recipients get the same GPL-3.0 rights
- ❌ Can't prevent recipients from redistributing

---

## Detailed Scenarios

### Scenario 1: Internal Company Use
```
Situation: You customize ERPNext for your manufacturing company
Users: Only your employees
Distribution: None

Repository Privacy: ✅ CAN BE PRIVATE
Code Sharing: ❌ NOT REQUIRED
License Compliance: ✅ Use as you wish internally
```

### Scenario 2: Selling to Customers
```
Situation: You sell customized ERPNext to other companies
Users: Your customers
Distribution: Yes (selling software)

Repository Privacy: ⚠️ Customers must get source code
Code Sharing: ✅ REQUIRED to customers
License Compliance: ⚠️ Must provide source under GPL-3.0
GitHub Repo: Can stay private, but must provide code another way
```

### Scenario 3: SaaS/Cloud Service
```
Situation: You offer ERP as a cloud service (customers access via web)
Users: Paying customers
Distribution: Debatable (network use)

Repository Privacy: ⚠️ Legal gray area
Code Sharing: ⚠️ Consult lawyer
License Compliance: ⚠️ GPL-3.0 may not require, AGPL would
Recommendation: Consider AGPL compliance or legal advice
```

### Scenario 4: Open Source Contribution
```
Situation: You want to share improvements with community
Users: Public
Distribution: Yes (public repository)

Repository Privacy: ❌ Must be public
Code Sharing: ✅ Required (and desired)
License Compliance: ✅ Use GPL-3.0
```

---

## How to Make Your Fork Private

### Step-by-Step (GitHub)

1. **Create/Fork the Repository**
   ```bash
   # Fork via GitHub UI or create new private repo
   ```

2. **Make It Private** (if not already)
   - Go to your repository on GitHub
   - Click **Settings** (top right)
   - Scroll to **Danger Zone**
   - Click **Change repository visibility**
   - Select **Make private**
   - Type repository name to confirm
   - Click **I understand, change repository visibility**

3. **Verify Privacy**
   ```bash
   # Only you and collaborators you invite can see it
   # Check: Repository should show "Private" badge
   ```

### Important Notes

⚠️ **Forking from Public Repo**:
- When you fork a public repo, your fork is initially public
- You must manually change it to private after forking
- Some GitHub plans limit private repository features

⚠️ **License File**:
- Keep the `license.txt` file (GPL-3.0) in your repository
- Even if private, the license still applies
- This protects you legally

---

## Best Practices for Private Forks

### 1. Document Your Intent

Create a file like `USAGE_POLICY.md`:

```markdown
# Usage Policy

This is a private fork of ERPNext for internal use by [Your Company].

## Usage Scope
- Internal company use only
- Not distributed to external parties
- Not offered as a service to third parties

## License Compliance
- Based on ERPNext (GPL-3.0)
- Used under internal use exception
- Source code kept private as permitted

## If Distribution Occurs
If we ever distribute this software, we will:
1. Provide source code to recipients
2. Include GPL-3.0 license
3. Comply with all license terms
```

### 2. Access Control

```bash
# Keep your repository private
# Only invite necessary collaborators:
# Settings → Collaborators → Add people

# Don't:
# - Share repository URL publicly
# - Post code snippets publicly without permission
# - Deploy publicly accessible instances without license compliance
```

### 3. Maintain License File

```bash
# Always keep these files:
- license.txt (GPL-3.0)
- README.md (with ERPNext attribution)
- Any copyright notices
```

### 4. Track Your Modifications

Create `MODIFICATIONS.md`:

```markdown
# Modifications Log

This file tracks changes made to the original ERPNext codebase.

## Date: YYYY-MM-DD
- Modified: [file path]
- Reason: [why changed]
- Type: [feature/bugfix/customization]

(Required for GPL-3.0 compliance if you ever distribute)
```

---

## Converting Between Public and Private

### Make Public → Private

```bash
# On GitHub:
# Settings → General → Danger Zone → Change visibility → Make private
```

**Considerations**:
- Previous public versions are still out there
- Anyone who cloned it still has a copy
- GitHub plan may limit private repos

### Make Private → Public

```bash
# On GitHub:
# Settings → General → Danger Zone → Change visibility → Make public
```

**Considerations**:
- Everyone can see your code
- Can't easily "unpublish"
- Good for community contributions

---

## Special Considerations

### Multi-Company Scenario

**Question**: Can I use one private fork for multiple companies I own?

**Answer**: ✅ Yes, if:
- You own/control all the companies
- They're part of the same organizational structure
- It's still "internal use"

**Warning**: If companies are separate legal entities with different ownership, consult a lawyer.

### Contractor/Developer Access

**Question**: Can contractors see my private repository?

**Answer**: ✅ Yes, you can:
- Add contractors as collaborators
- Have them sign NDAs (separate from GPL)
- They can work on your private code

**Important**: 
- GPL doesn't prevent NDAs for development
- But if you distribute to contractors as "users", GPL applies

### Backup and Security

**For Private Repositories**:

```bash
# Set up regular backups
# Don't rely only on GitHub

# Clone to secure location
git clone --mirror https://github.com/YOUR-USERNAME/your-erp.git
cd your-erp.git
git remote add backup /path/to/secure/backup/location
git push backup --mirror

# Or use encrypted backup services
```

---

## Summary Table

| Use Case | Repository Privacy | Must Share Code | Notes |
|----------|-------------------|-----------------|-------|
| Internal company use | ✅ Can be private | ❌ No | Most common case |
| Sell to customers | ⚠️ Can be private* | ✅ Yes, to customers | Must provide source |
| SaaS/Cloud service | ⚠️ Gray area | ⚠️ Consult lawyer | GPL-3.0 unclear on SaaS |
| Open source contribution | ❌ Must be public | ✅ Yes, to everyone | Share with community |
| Consulting/deployment | ⚠️ Depends | ✅ Yes, to clients | If you deploy for others |

*Repository can be private, but must provide source code through other means to recipients

---

## Recommended Approach

### For Most Users (Internal Use)

1. ✅ **Keep repository private**
2. ✅ **Use only within your organization**
3. ✅ **Keep license file intact**
4. ✅ **Document that it's internal use**
5. ✅ **Don't distribute to third parties**

### If You Plan to Distribute

1. ⚠️ **Consult with a lawyer** familiar with GPL
2. ⚠️ **Plan how to provide source code**
3. ⚠️ **Consider using AGPL** if offering as SaaS
4. ⚠️ **Document all modifications**
5. ⚠️ **Prepare distribution package** with source

---

## Legal Disclaimer

**⚠️ This is NOT legal advice!**

This guide provides general information about GPL-3.0 license. For legal questions about your specific situation:

- **Consult a lawyer** specializing in open source licensing
- **Review GPL-3.0 license** carefully: https://www.gnu.org/licenses/gpl-3.0.html
- **Seek professional advice** if distributing or offering as service

---

## Quick Decision Tree

```
Are you using it ONLY within your company?
├─ Yes → ✅ Repository CAN be private
│         ✅ Code CAN stay private
│         ✅ No distribution required
│
└─ No → Are you giving/selling to others?
        ├─ Yes → ⚠️ Must provide source to recipients
        │         ⚠️ Repository can be private but must share code
        │         ⚠️ Recipients get GPL rights
        │
        └─ No → Are you offering as SaaS/cloud service?
                ├─ Yes → ⚠️ CONSULT A LAWYER
                │         ⚠️ GPL-3.0 gray area
                │
                └─ No → ✅ You're probably okay with private
```

---

## Frequently Asked Questions

### Q: Can I keep my fork private forever?
**A**: Yes, as long as you're using it internally and not distributing it to others.

### Q: What if I later decide to distribute?
**A**: You must then provide source code to recipients under GPL-3.0 terms.

### Q: Can I switch from private to public later?
**A**: Yes, you can change visibility at any time on GitHub.

### Q: Will making it private protect my customizations?
**A**: Yes, from public view. But if you distribute the software, recipients get the source code.

### Q: Can my employees see the private repository?
**A**: Only if you add them as collaborators. GitHub private repos are only visible to authorized users.

### Q: Does private repository violate GPL-3.0?
**A**: No, not for internal use. GPL-3.0 allows private use without source distribution.

---

## Resources

- **GPL-3.0 Full Text**: https://www.gnu.org/licenses/gpl-3.0.html
- **GPL FAQ**: https://www.gnu.org/licenses/gpl-faq.html
- **GitHub Private Repos**: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility
- **Open Source Initiative**: https://opensource.org/licenses/GPL-3.0

---

**Bottom Line**: For internal company use, your fork can be completely private. Just keep the license file and don't distribute the software to others! 🔒
