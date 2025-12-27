# ERPNext Customization Checklist

Use this checklist to track your customization progress when forking ERPNext for your own use.

## Phase 1: Initial Setup

### Repository Setup
- [ ] Forked repository to my GitHub account
- [ ] Cloned fork to local development environment
- [ ] Added upstream remote: `git remote add upstream <original-repo-url>`
- [ ] Created custom branch: `git checkout -b custom/my-branch-name`
- [ ] Verified I cannot accidentally push to upstream repository

### Development Environment
- [ ] Installed Frappe bench
- [ ] Created new site for development
- [ ] Installed app on development site
- [ ] Verified app runs successfully
- [ ] Set up database backups

---

## Phase 2: Metadata & Configuration

### Package Metadata
- [ ] Updated `package.json`:
  - [ ] Changed `name` field
  - [ ] Updated `description`
  - [ ] Updated `repository.url`
  - [ ] Updated `homepage`
  - [ ] Updated `author`
  - [ ] Updated `bugs.url`
  
- [ ] Updated `pyproject.toml`:
  - [ ] Changed `name` field
  - [ ] Updated `authors`
  - [ ] Updated `description`
  - [ ] Updated `project.urls.Homepage`
  - [ ] Updated `project.urls.Repository`
  - [ ] Updated `project.urls["Bug Reports"]`

### Documentation
- [ ] Created custom README.md
  - [ ] Added project description
  - [ ] Credited ERPNext as base
  - [ ] Documented custom features
  - [ ] Added installation instructions
  - [ ] Included license information
  
- [ ] Created/Updated CONTRIBUTING.md with my guidelines
- [ ] Created DEPLOYMENT.md with deployment instructions
- [ ] Created CUSTOMIZATION_NOTES.md to document changes

---

## Phase 3: Branding & UI

### Visual Identity
- [ ] Designed new logo
- [ ] Created favicon
- [ ] Designed app icons
- [ ] Chose color scheme/theme

### Asset Replacement
- [ ] Replaced logo in `erpnext/public/images/`
- [ ] Replaced favicon
- [ ] Replaced app icons
- [ ] Updated splash screen (if applicable)
- [ ] Updated email header images

### Application Configuration
- [ ] Updated app title in hooks.py
- [ ] Modified app description
- [ ] Updated website settings
- [ ] Customized login page
- [ ] Customized desktop icons/layout

### Styling
- [ ] Created custom CSS/SCSS for brand colors
- [ ] Updated primary color scheme
- [ ] Updated secondary color scheme
- [ ] Updated button styles (if needed)
- [ ] Updated navigation styling (if needed)

---

## Phase 4: Email & Communications

### Email Templates
- [ ] Updated email header/footer
- [ ] Customized welcome email
- [ ] Customized password reset email
- [ ] Customized notification emails
- [ ] Updated email signatures
- [ ] Updated support contact information

### Print Formats
- [ ] Customized invoice template
- [ ] Customized quotation template
- [ ] Customized purchase order template
- [ ] Customized delivery note template
- [ ] Added company letterhead
- [ ] Updated footer information

---

## Phase 5: Feature Customization

### Core Features
- [ ] Reviewed all modules
- [ ] Identified modules to keep
- [ ] Identified modules to remove/disable
- [ ] Identified modules to modify

### Custom Modules
- [ ] Created custom module directory structure
- [ ] Added custom module 1: _________________
- [ ] Added custom module 2: _________________
- [ ] Added custom module 3: _________________
- [ ] Registered custom modules in hooks.py

### Custom DocTypes
- [ ] Created custom doctype 1: _________________
- [ ] Created custom doctype 2: _________________
- [ ] Created custom doctype 3: _________________
- [ ] Added custom fields to existing doctypes

### Custom Reports
- [ ] Created custom report 1: _________________
- [ ] Created custom report 2: _________________
- [ ] Created custom report 3: _________________
- [ ] Modified existing reports as needed

### Custom Dashboards
- [ ] Created custom dashboard 1: _________________
- [ ] Created custom dashboard 2: _________________
- [ ] Modified homepage dashboard
- [ ] Added custom charts/widgets

---

## Phase 6: Business Logic

### Custom APIs
- [ ] Created custom API endpoint 1: _________________
- [ ] Created custom API endpoint 2: _________________
- [ ] Created custom API endpoint 3: _________________
- [ ] Documented API endpoints

### Workflows
- [ ] Customized workflow 1: _________________
- [ ] Customized workflow 2: _________________
- [ ] Created new workflow 1: _________________
- [ ] Created new workflow 2: _________________

### Validations
- [ ] Added custom validation 1: _________________
- [ ] Added custom validation 2: _________________
- [ ] Modified existing validations

### Integrations
- [ ] Integrated with service 1: _________________
- [ ] Integrated with service 2: _________________
- [ ] Set up webhooks
- [ ] Configured API keys securely

---

## Phase 7: Data & Settings

### Default Settings
- [ ] Configured default company settings
- [ ] Set up default user roles
- [ ] Configured default permissions
- [ ] Set up default email accounts
- [ ] Configured default print settings

### Master Data
- [ ] Imported initial customers (if applicable)
- [ ] Imported initial suppliers (if applicable)
- [ ] Imported initial items (if applicable)
- [ ] Set up chart of accounts
- [ ] Configured tax templates

### System Settings
- [ ] Configured regional settings
- [ ] Set up currency
- [ ] Configured fiscal year
- [ ] Set up number series
- [ ] Configured notification settings

---

## Phase 8: Testing

### Functionality Testing
- [ ] Tested all core modules
- [ ] Tested custom modules
- [ ] Tested workflows
- [ ] Tested reports
- [ ] Tested dashboards
- [ ] Tested API endpoints

### Integration Testing
- [ ] Tested email functionality
- [ ] Tested print formats
- [ ] Tested external integrations
- [ ] Tested webhooks
- [ ] Tested imports/exports

### User Acceptance Testing
- [ ] Created test scenarios
- [ ] Conducted user testing
- [ ] Documented issues
- [ ] Fixed critical issues
- [ ] Verified fixes

### Performance Testing
- [ ] Tested with sample data
- [ ] Tested database queries
- [ ] Optimized slow operations
- [ ] Tested concurrent users (if applicable)

---

## Phase 9: Deployment

### Environment Setup
- [ ] Set up production server
- [ ] Configured database
- [ ] Set up backup system
- [ ] Configured SSL/TLS
- [ ] Set up monitoring

### Deployment Process
- [ ] Created deployment scripts
- [ ] Documented deployment process
- [ ] Created rollback procedure
- [ ] Set up CI/CD pipeline (optional)
- [ ] Configured automatic backups

### Security
- [ ] Changed default passwords
- [ ] Configured firewall rules
- [ ] Set up fail2ban (or similar)
- [ ] Enabled HTTPS
- [ ] Configured security headers
- [ ] Set up regular security updates

---

## Phase 10: Documentation

### User Documentation
- [ ] Created user guide
- [ ] Documented custom features
- [ ] Created video tutorials (optional)
- [ ] Created FAQ section
- [ ] Documented common workflows

### Technical Documentation
- [ ] Documented architecture
- [ ] Documented custom modules
- [ ] Documented API endpoints
- [ ] Created database schema documentation
- [ ] Documented deployment process

### Training Materials
- [ ] Created training presentations
- [ ] Created hands-on exercises
- [ ] Created admin guide
- [ ] Created troubleshooting guide

---

## Phase 11: Maintenance Plan

### Version Control
- [ ] Set up branching strategy
- [ ] Created tagging convention
- [ ] Documented git workflow
- [ ] Set up code review process

### Update Strategy
- [ ] Documented update process from upstream
- [ ] Created testing checklist for updates
- [ ] Set up staging environment for updates
- [ ] Defined update schedule

### Backup Strategy
- [ ] Automated database backups
- [ ] Automated file backups
- [ ] Tested restore procedure
- [ ] Documented backup locations
- [ ] Set up off-site backups

### Monitoring
- [ ] Set up uptime monitoring
- [ ] Set up error logging
- [ ] Set up performance monitoring
- [ ] Configured alerts
- [ ] Created monitoring dashboard

---

## Phase 12: Legal & Compliance

### License Compliance
- [ ] Kept GPL-3.0 license file
- [ ] Added attribution to ERPNext
- [ ] Documented all modifications
- [ ] Made source code available (if distributing)
- [ ] Reviewed license requirements

### Trademark Compliance
- [ ] Removed ERPNext from product name
- [ ] Updated branding to avoid confusion
- [ ] Added proper attribution where needed
- [ ] Reviewed trademark policy

### Privacy & Data
- [ ] Created privacy policy
- [ ] Implemented data protection measures
- [ ] Set up GDPR compliance (if applicable)
- [ ] Configured data retention policies
- [ ] Documented data handling procedures

---

## Custom Features Tracker

### Feature 1: [Feature Name]
- **Description**: 
- **Status**: [ ] Planning [ ] In Progress [ ] Testing [ ] Complete
- **Files Modified**: 
- **Notes**: 

### Feature 2: [Feature Name]
- **Description**: 
- **Status**: [ ] Planning [ ] In Progress [ ] Testing [ ] Complete
- **Files Modified**: 
- **Notes**: 

### Feature 3: [Feature Name]
- **Description**: 
- **Status**: [ ] Planning [ ] In Progress [ ] Testing [ ] Complete
- **Files Modified**: 
- **Notes**: 

---

## Issues & Resolutions

### Issue 1
- **Date**: 
- **Description**: 
- **Resolution**: 
- **Status**: [ ] Open [ ] Resolved

### Issue 2
- **Date**: 
- **Description**: 
- **Resolution**: 
- **Status**: [ ] Open [ ] Resolved

---

## Version History

### Version 1.0.0 (Custom Release)
- **Date**: 
- **Base ERPNext Version**: 
- **Changes**: 
- **Notes**: 

### Version 1.1.0
- **Date**: 
- **Base ERPNext Version**: 
- **Changes**: 
- **Notes**: 

---

## Notes & Reminders

Add any important notes, reminders, or decisions made during customization:

1. 
2. 
3. 

---

## Contact Information

**Project Lead**: 
**Technical Contact**: 
**Support Email**: 
**Repository**: 

---

**Last Updated**: [Date]
**Current Version**: [Your Version]
**Base ERPNext Version**: [ERPNext Version]
