# Quick Start: Fork and Customize ERPNext

This is a streamlined guide to get you started quickly. For comprehensive details, see [FORKING_GUIDE.md](./FORKING_GUIDE.md).

## 🚀 Quick Setup (5 Minutes)

### Step 1: Fork the Repository
1. Click the "Fork" button at the top of this page
2. Choose your GitHub account/organization
3. Wait for fork to complete
4. **Optional**: Make repository private (Settings → Change visibility → Make private)
   - ✅ You CAN make it private for internal company use
   - See [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md) for details

### Step 2: Clone Your Fork
```bash
git clone https://github.com/YOUR-USERNAME/erpnext.git
cd erpnext
```

### Step 3: Create Your Custom Branch
```bash
git checkout -b custom/production
```

### Step 4: Add Upstream Remote (Optional)
```bash
# To sync updates later
git remote add upstream https://github.com/abdulrahman-gaith-beep/erpnext.git

# Add original ERPNext (for major updates)
git remote add erpnext-upstream https://github.com/frappe/erpnext.git
```

## 📝 Essential Customizations

### Update Package Metadata

1. **Edit `package.json`**:
```bash
nano package.json  # or use your preferred editor
```
Change these fields:
- `name`: "your-company-erp"
- `description`: "Your custom description"
- `repository.url`: "https://github.com/YOUR-USERNAME/your-erp.git"
- `author`: "Your Company Name"

2. **Edit `pyproject.toml`**:
```bash
nano pyproject.toml
```
Change these fields:
- `name`: "your-company-erp"
- `authors`: Your company details
- `description`: Your description
- URLs section: Update all links

### Update README

1. **Save current README** (for reference):
```bash
mv README.md README.ERPNEXT.md
```

2. **Create your README**:
```bash
cat > README.md << 'EOF'
# Your Company ERP

Your custom ERP system based on ERPNext.

## About
This is a customized version of ERPNext for [your use case].

### Based On
- [ERPNext](https://github.com/frappe/erpnext) - Open Source ERP
- [Frappe Framework](https://github.com/frappe/frappe)

## License
GPL-3.0 (inherited from ERPNext)

## Installation
[Your installation instructions]

EOF
```

## 🎨 Branding (Quick)

### Replace Logo
```bash
# Backup original
mkdir -p .backup
cp -r erpnext/public/images .backup/

# Add your logo (replace with your files)
# cp /path/to/your/logo.svg erpnext/public/images/v16/erpnext.svg
# cp /path/to/your/favicon.ico erpnext/public/favicon.ico
```

## 💾 Commit Your Changes

```bash
# Check what you've changed
git status

# Add your changes
git add package.json pyproject.toml README.md

# Commit
git commit -m "Initial customization: rebrand for [Your Company]"

# Push to your fork
git push origin custom/production
```

## 🔄 Sync with Upstream (Later)

When you want to get updates:

```bash
# Fetch updates
git fetch upstream

# See what's new
git log HEAD..upstream/develop --oneline

# Merge (carefully!)
git merge upstream/develop

# Or cherry-pick specific commits
git cherry-pick <commit-hash>
```

## ⚠️ Important Reminders

### Legal
- ✅ Keep GPL-3.0 license
- ✅ Keep copyright notices
- ✅ Credit ERPNext in your README
- ❌ Don't use "ERPNext" in your product name

### Privacy
- ✅ **CAN be private** for internal company use
- ✅ **CAN be public** if you want to share
- ⚠️ Must share code if distributing to others
- 📖 See [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md) for full details

### Safety
- ✅ Your changes won't affect the original repository
- ✅ You have full control of your fork
- ✅ Original owner can't access your fork

## 📚 Next Steps

1. ✅ Complete basic setup (above)
2. 📋 Follow [CUSTOMIZATION_CHECKLIST.md](./CUSTOMIZATION_CHECKLIST.md)
3. 📖 Read [FORKING_GUIDE.md](./FORKING_GUIDE.md) for details
4. 🛠️ Start customizing features
5. 🧪 Test your changes
6. 🚀 Deploy to production

## 🆘 Need Help?

- **Detailed Guide**: [FORKING_GUIDE.md](./FORKING_GUIDE.md)
- **Privacy & Licensing**: [PRIVACY_AND_LICENSING.md](./PRIVACY_AND_LICENSING.md)
- **Saudi Agriculture**: [SAUDI_AGRICULTURE_GUIDE.md](./SAUDI_AGRICULTURE_GUIDE.md) ⭐ NEW!
- **Checklist**: [CUSTOMIZATION_CHECKLIST.md](./CUSTOMIZATION_CHECKLIST.md)
- **ERPNext Docs**: https://docs.erpnext.com/
- **Frappe Docs**: https://frappeframework.com/docs
- **Forum**: https://discuss.frappe.io/

## 📊 Customization Progress

Track your progress in [CUSTOMIZATION_CHECKLIST.md](./CUSTOMIZATION_CHECKLIST.md).

---

**Ready to customize?** Start with the checklist and you'll be ready in no time! 🎉
