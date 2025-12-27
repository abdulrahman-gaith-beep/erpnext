# Saudi Arabia Agricultural ERP Deployment Guide

This guide provides comprehensive information for deploying and customizing ERPNext for agricultural businesses in Saudi Arabia, including regulatory compliance, licensing, and operational setup.

---

## Table of Contents

1. [Overview](#overview)
2. [Saudi Agricultural Regulatory Framework](#saudi-agricultural-regulatory-framework)
3. [Licensing and Permits](#licensing-and-permits)
4. [Labor Law Compliance](#labor-law-compliance)
5. [Project Implementation Phases](#project-implementation-phases)
6. [Task List with Roles and Assignments](#task-list-with-roles-and-assignments)
7. [Entity Structure and SPV Creation](#entity-structure-and-spv-creation)
8. [Farmer Company Formation](#farmer-company-formation)
9. [MEWA and NCEC Compliance](#mewa-and-ncec-compliance)
10. [ERP Configuration for Agriculture](#erp-configuration-for-agriculture)

---

## Overview

This guide helps agricultural businesses in Saudi Arabia implement ERPNext while ensuring full compliance with Saudi laws and regulations. It covers:

- 🏛️ Regulatory compliance (MEWA, NCEC, labor laws)
- 📋 Required licenses and permits
- 👥 Team structure and assignments
- 🏢 Company formation and SPV setup
- ⚖️ Legal framework compliance
- 🌾 Agriculture-specific ERP features

---

## Saudi Agricultural Regulatory Framework

### Key Regulatory Bodies

#### 1. **MEWA (Ministry of Environment, Water and Agriculture)**
**Arabic**: وزارة البيئة والمياه والزراعة

**Responsibilities**:
- Agricultural licensing
- Water resource management
- Environmental compliance
- Food safety standards
- Plant and animal health
- Agricultural development programs

**Website**: https://www.mewa.gov.sa/
**Contact**: 920000911

**Key Departments**:
- Agricultural Affairs
- Water Affairs
- Environment Affairs
- National Center for Agriculture Technology (NCAT)

#### 2. **NCEC (National Center for Environmental Compliance)**
**Arabic**: المركز الوطني للامتثال البيئي

**Responsibilities**:
- Environmental compliance monitoring
- Environmental permits and licenses
- Inspection and enforcement
- Environmental impact assessments
- Pollution control

**Website**: https://ncec.gov.sa/
**Portal**: https://eservices.ncec.gov.sa/

#### 3. **MOCI (Ministry of Commerce)**
**Arabic**: وزارة التجارة

**Responsibilities**:
- Commercial registration
- Business licensing
- Company formation
- Trade regulations

**Website**: https://mc.gov.sa/

#### 4. **HRSD (Ministry of Human Resources and Social Development)**
**Arabic**: وزارة الموارد البشرية والتنمية الاجتماعية

**Responsibilities**:
- Labor regulations
- Work permits
- Employment contracts
- Social insurance (GOSI)
- Saudization (Nitaqat)

**Website**: https://www.hrsd.gov.sa/

#### 5. **GOSI (General Organization for Social Insurance)**
**Arabic**: المؤسسة العامة للتأمينات الاجتماعية

**Responsibilities**:
- Social insurance registration
- Employee contributions
- Benefits administration

**Website**: https://www.gosi.gov.sa/

#### 6. **ZATCA (Zakat, Tax and Customs Authority)**
**Arabic**: هيئة الزكاة والضريبة والجمارك

**Responsibilities**:
- VAT (15%)
- Zakat collection
- Tax compliance
- E-invoicing (FATOORA)

**Website**: https://zatca.gov.sa/

---

## Licensing and Permits

### Agricultural Licenses Required

#### 1. **Agricultural Production License**
**Issued by**: MEWA

**Requirements**:
- Land ownership or lease documentation
- Water source approval
- Environmental compliance certificate
- Business plan
- Technical qualifications

**Application Process**:
1. Register on MEWA portal: https://eservices.mewa.gov.sa/
2. Submit land documents
3. Obtain water permit
4. Submit environmental assessment
5. Pay applicable fees
6. Await inspection
7. Receive license

**Timeline**: 30-90 days
**Validity**: Renewable annually
**Fees**: Varies by project size (SAR 500-5,000)

#### 2. **Water Extraction Permit**
**Issued by**: MEWA - Water Affairs

**Requirements**:
- Hydrogeological study
- Water quality assessment
- Sustainable usage plan
- Drilling specifications
- Meter installation plan

**Application Process**:
1. Submit hydrogeological report
2. Pay assessment fees
3. Obtain drilling permit
4. Install approved meters
5. Submit completion report
6. Receive operating permit

**Timeline**: 60-120 days
**Fees**: Based on extraction volume

#### 3. **Environmental Permit**
**Issued by**: NCEC

**Requirements**:
- Environmental Impact Assessment (EIA)
- Pollution control plan
- Waste management plan
- Emergency response plan
- Monitoring program

**Application Process**:
1. Register on NCEC portal: https://eservices.ncec.gov.sa/
2. Submit EIA report
3. Pay assessment fees
4. Respond to queries
5. Implement required measures
6. Pass inspection
7. Receive permit

**Timeline**: 90-180 days
**Validity**: 3-5 years
**Fees**: SAR 10,000-100,000 (project-dependent)

#### 4. **Commercial Registration (CR)**
**Issued by**: MOCI

**Requirements**:
- Company name reservation
- Memorandum of Association
- Lease agreement (office/facility)
- Capital deposit proof
- Partner identification

**Application Process**:
1. Reserve name on https://cr.mc.gov.sa/
2. Prepare company documents
3. Notarize at MOJ
4. Submit online application
5. Pay fees
6. Receive CR certificate

**Timeline**: 1-7 days
**Fees**: SAR 200-1,200
**Validity**: Renewable annually

#### 5. **Food Safety License** (if applicable)
**Issued by**: SFDA (Saudi Food and Drug Authority)

**Requirements**:
- Food safety management system
- HACCP compliance
- Facility specifications
- Quality control procedures
- Staff training certificates

**Application Process**:
1. Register on SFDA portal
2. Submit facility plans
3. Implement food safety system
4. Pass inspection
5. Receive license

**Timeline**: 60-90 days
**Fees**: SAR 5,000-15,000

#### 6. **Organic Certification** (optional)
**Issued by**: SASO (Saudi Standards, Metrology and Quality Organization)

**Requirements**:
- Organic production plan
- 3-year transition period
- No synthetic inputs
- Record keeping system
- Annual inspections

**Timeline**: 3+ years for full certification

---

## Labor Law Compliance

### Saudi Labor Law Overview

**Primary Legislation**: Saudi Labor Law (Royal Decree No. M/51, 2005)
**Amendments**: Updated 2015, 2021

### Key Requirements

#### 1. **Employment Contracts**

**Mandatory Elements**:
- Contract type (definite/indefinite)
- Job title and duties
- Salary and benefits
- Working hours
- Probation period (max 90-180 days)
- Notice period
- Arabic language (primary)

**Types**:
- **Indefinite term**: No end date
- **Definite term**: Specific period (max 4 years)
- **Part-time**: Less than full working hours
- **Seasonal**: Agricultural seasonal work

**Digital Platform**: Qiwa (https://qiwa.sa/)

#### 2. **Working Hours and Overtime**

**Standard Hours**:
- 8 hours/day or 48 hours/week
- Ramadan: 6 hours/day for Muslims
- Agricultural work: May vary seasonally

**Overtime**:
- Rate: 150% of hourly wage
- Maximum: Limited by law

**Rest Periods**:
- Daily: 30-60 minutes
- Weekly: 1 full day (usually Friday)
- Annual leave: 21-30 days (tenure-based)

#### 3. **Saudization (Nitaqat Program)**

**Purpose**: Increase Saudi employment

**Categories**:
- Platinum: Highest Saudi ratio
- Green: Compliant
- Yellow: Low compliance
- Red: Non-compliant

**Agriculture Sector Requirements**:
- Target: Variable by company size
- Check current rates: https://qiwa.sa/

**Benefits of Compliance**:
- Access to government contracts
- Visa processing priority
- Reduced inspection frequency

#### 4. **Wage Protection System (WPS)**

**Requirements**:
- Register with HRSD
- Pay through approved banks
- Submit payroll records monthly
- Use SADAD payment system

**Timeline**: Salaries due by 7th of following month

**Penalties for Non-Compliance**:
- SAR 3,000 per violation
- Visa services suspension
- Inability to renew CR

#### 5. **GOSI Registration**

**Mandatory Coverage**:
- All Saudi employees
- Optional for expats (with agreement)

**Contribution Rates (2024)**:
- **Saudi employees**: 21.5% (employer: 11.5%, employee: 10%)
- **Expat employees**: 2% (employer only, for occupational hazards)

**Registration Process**:
1. Register employer: https://online.gosi.gov.sa/
2. Add employees within 15 days of hiring
3. Submit monthly contributions
4. File quarterly reports

**Penalties**: 2% per month on late payments

#### 6. **Work Permits and Visas**

**For Expat Agricultural Workers**:

**Types**:
- Work visa (sponsored by company)
- Temporary agricultural visa (seasonal)

**Requirements**:
- Valid passport
- Medical fitness certificate
- No criminal record
- Educational certificates (as required)
- Job offer letter

**Process via MOL/HRSD**:
1. Company applies for visa allocation
2. Submit worker details
3. Pay fees
4. Worker obtains visa at embassy
5. Complete medical examination in KSA
6. Issue Iqama (residence permit)

**Costs**: SAR 2,000-5,000 per worker

#### 7. **End of Service Benefits (ESB)**

**Calculation**:
- First 5 years: Half month salary per year
- After 5 years: Full month salary per year

**Payment**: Due within 2 weeks of termination

**Gratuity**: Prorated for resignation (2-10 years service)

---

## Project Implementation Phases

### Phase 1: Planning and Consulting (Weeks 1-4)

**Objectives**:
- Assess business requirements
- Define project scope
- Identify regulatory requirements
- Establish timelines and budget

**Deliverables**:
- Business requirements document
- Regulatory compliance checklist
- Project charter
- Resource allocation plan

### Phase 2: Legal Setup (Weeks 3-12)

**Objectives**:
- Form legal entities
- Obtain licenses and permits
- Register with authorities
- Establish compliance frameworks

**Deliverables**:
- Company registration
- All required licenses
- Authority registrations
- Compliance procedures

### Phase 3: System Design (Weeks 8-12)

**Objectives**:
- Design ERP architecture
- Customize for agriculture
- Plan integrations
- Design reporting framework

**Deliverables**:
- System architecture document
- Customization specifications
- Integration plan
- Report templates

### Phase 4: Development and Configuration (Weeks 12-20)

**Objectives**:
- Install and configure ERPNext
- Develop customizations
- Integrate systems
- Configure workflows

**Deliverables**:
- Configured ERP system
- Custom modules
- Integration connections
- Workflow automations

### Phase 5: Testing and Training (Weeks 18-24)

**Objectives**:
- Test all functionality
- Train users
- Document procedures
- Prepare for go-live

**Deliverables**:
- Test reports
- Trained users
- User manuals
- Standard operating procedures

### Phase 6: Operations and Support (Week 24+)

**Objectives**:
- Go live with system
- Provide ongoing support
- Monitor compliance
- Continuous improvement

**Deliverables**:
- Live production system
- Support tickets resolution
- Compliance reports
- Enhancement roadmap

---

## Task List with Roles and Assignments

### Project Organization Structure

```
Project Governance
├── Steering Committee (Client Senior Management)
├── Project Manager (Overall Coordination)
├── Business Stream
│   ├── Legal & Compliance Team
│   ├── Operations Team
│   └── Finance Team
└── Technical Stream
    ├── Solution Architects
    ├── Developers
    └── QA/Testing Team
```

### Detailed Task List

#### **PHASE 1: CONSULTING & PLANNING**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| C-001 | Conduct initial stakeholder meeting | Project Manager | 1 day | None | ⬜ Not Started |
| C-002 | Document business requirements | Business Analyst | 5 days | C-001 | ⬜ Not Started |
| C-003 | Map current processes | Process Consultant | 5 days | C-002 | ⬜ Not Started |
| C-004 | Identify pain points and gaps | Business Analyst | 3 days | C-003 | ⬜ Not Started |
| C-005 | Define project scope and objectives | Project Manager | 2 days | C-004 | ⬜ Not Started |
| C-006 | Create project charter | Project Manager | 2 days | C-005 | ⬜ Not Started |
| C-007 | Develop project plan and timeline | Project Manager | 3 days | C-006 | ⬜ Not Started |
| C-008 | Resource planning and allocation | Project Manager | 2 days | C-007 | ⬜ Not Started |
| C-009 | Budget estimation and approval | Financial Analyst | 3 days | C-008 | ⬜ Not Started |
| C-010 | Risk assessment and mitigation plan | Risk Manager | 3 days | C-007 | ⬜ Not Started |
| C-011 | Regulatory requirements analysis | Legal Consultant | 5 days | C-002 | ⬜ Not Started |
| C-012 | Stakeholder approval of plan | Steering Committee | 2 days | C-009 | ⬜ Not Started |

#### **PHASE 2: LEGAL & REGULATORY SETUP**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| L-001 | Reserve company name with MOCI | Legal Officer | 1 day | C-012 | ⬜ Not Started |
| L-002 | Draft Memorandum of Association | Corporate Lawyer | 3 days | L-001 | ⬜ Not Started |
| L-003 | Notarize company documents at MOJ | Legal Officer | 2 days | L-002 | ⬜ Not Started |
| L-004 | Submit CR application to MOCI | Legal Officer | 1 day | L-003 | ⬜ Not Started |
| L-005 | Obtain Commercial Registration | Legal Officer | 3 days | L-004 | ⬜ Not Started |
| L-006 | Open corporate bank account | Finance Manager | 2 days | L-005 | ⬜ Not Started |
| L-007 | Register with ZATCA for VAT/Zakat | Tax Consultant | 3 days | L-005 | ⬜ Not Started |
| L-008 | Register with GOSI | HR Manager | 2 days | L-005 | ⬜ Not Started |
| L-009 | Prepare hydrogeological study | Environmental Consultant | 15 days | L-005 | ⬜ Not Started |
| L-010 | Apply for water extraction permit | Environmental Officer | 5 days | L-009 | ⬜ Not Started |
| L-011 | Conduct Environmental Impact Assessment | Environmental Consultant | 20 days | L-005 | ⬜ Not Started |
| L-012 | Apply for NCEC environmental permit | Environmental Officer | 5 days | L-011 | ⬜ Not Started |
| L-013 | Prepare agricultural business plan | Agricultural Consultant | 10 days | C-002 | ⬜ Not Started |
| L-014 | Apply for MEWA agricultural license | Agricultural Officer | 5 days | L-013 | ⬜ Not Started |
| L-015 | Arrange site inspection (MEWA) | Operations Manager | 2 days | L-014 | ⬜ Not Started |
| L-016 | Obtain agricultural production license | Agricultural Officer | 10 days | L-015 | ⬜ Not Started |
| L-017 | Apply for food safety license (SFDA) | Quality Manager | 5 days | L-016 | ⬜ Not Started |
| L-018 | Setup compliance monitoring system | Compliance Officer | 5 days | L-008 | ⬜ Not Started |

#### **PHASE 3: SPV & ENTITY CREATION**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| S-001 | Define SPV structure and purpose | Corporate Lawyer | 3 days | C-006 | ⬜ Not Started |
| S-002 | Determine capitalization requirements | Financial Advisor | 2 days | S-001 | ⬜ Not Started |
| S-003 | Draft SPV governance framework | Corporate Lawyer | 5 days | S-001 | ⬜ Not Started |
| S-004 | Register SPV with MOCI | Legal Officer | 5 days | S-003 | ⬜ Not Started |
| S-005 | Open SPV bank account | Finance Manager | 2 days | S-004 | ⬜ Not Started |
| S-006 | Transfer initial capital | Finance Manager | 1 day | S-005 | ⬜ Not Started |
| S-007 | Appoint SPV board of directors | Shareholders | 1 day | S-004 | ⬜ Not Started |
| S-008 | Register SPV with ZATCA | Tax Consultant | 3 days | S-004 | ⬜ Not Started |
| S-009 | Register SPV with GOSI | HR Manager | 2 days | S-004 | ⬜ Not Started |
| S-010 | Setup SPV accounting system | Accountant | 5 days | S-005 | ⬜ Not Started |

#### **PHASE 4: FARMER COMPANY FORMATION**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| F-001 | Identify farmer groups/cooperatives | Agricultural Extension Officer | 10 days | L-016 | ⬜ Not Started |
| F-002 | Conduct farmer awareness sessions | Agricultural Consultant | 5 days | F-001 | ⬜ Not Started |
| F-003 | Assist farmers with documentation | Legal Assistant | 10 days | F-002 | ⬜ Not Started |
| F-004 | Form farmer companies/cooperatives | Corporate Lawyer | 15 days | F-003 | ⬜ Not Started |
| F-005 | Register farmer entities with MOCI | Legal Officer | 5 days | F-004 | ⬜ Not Started |
| F-006 | Obtain farmer licenses from MEWA | Agricultural Officer | 10 days | F-005 | ⬜ Not Started |
| F-007 | Setup farmer banking facilities | Finance Officer | 5 days | F-005 | ⬜ Not Started |
| F-008 | Establish supply agreements | Commercial Manager | 5 days | F-006 | ⬜ Not Started |
| F-009 | Train farmers on compliance | Training Coordinator | 5 days | F-006 | ⬜ Not Started |
| F-010 | Setup farmer payment systems | Finance Manager | 3 days | F-007 | ⬜ Not Started |

#### **PHASE 5: SYSTEM DESIGN**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| D-001 | Define system architecture | Solution Architect | 5 days | C-012 | ⬜ Not Started |
| D-002 | Design database schema | Database Architect | 7 days | D-001 | ⬜ Not Started |
| D-003 | Design user interface mockups | UX Designer | 10 days | C-002 | ⬜ Not Started |
| D-004 | Define custom modules requirements | Business Analyst | 7 days | C-002 | ⬜ Not Started |
| D-005 | Design workflow automations | Process Designer | 7 days | D-004 | ⬜ Not Started |
| D-006 | Plan integration points | Integration Architect | 5 days | D-001 | ⬜ Not Started |
| D-007 | Design reporting framework | BI Consultant | 7 days | C-002 | ⬜ Not Started |
| D-008 | Security and access control design | Security Architect | 5 days | D-001 | ⬜ Not Started |
| D-009 | Design data migration strategy | Data Architect | 5 days | D-002 | ⬜ Not Started |
| D-010 | Create technical specifications | Technical Writer | 7 days | D-008 | ⬜ Not Started |
| D-011 | Review and approve design | Technical Lead | 2 days | D-010 | ⬜ Not Started |

#### **PHASE 6: DEVELOPMENT & CONFIGURATION**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| V-001 | Setup development environment | DevOps Engineer | 3 days | D-011 | ⬜ Not Started |
| V-002 | Install ERPNext base system | System Administrator | 2 days | V-001 | ⬜ Not Started |
| V-003 | Configure company settings | ERP Consultant | 2 days | V-002, L-005 | ⬜ Not Started |
| V-004 | Configure chart of accounts | Accountant | 3 days | V-003 | ⬜ Not Started |
| V-005 | Setup tax configuration (VAT/Zakat) | Tax Consultant | 2 days | V-004 | ⬜ Not Started |
| V-006 | Configure HR and payroll | HR Consultant | 5 days | V-003 | ⬜ Not Started |
| V-007 | Develop agriculture custom modules | Senior Developer | 20 days | D-004 | ⬜ Not Started |
| V-008 | Develop farm management module | Developer | 15 days | V-007 | ⬜ Not Started |
| V-009 | Develop crop planning module | Developer | 10 days | V-007 | ⬜ Not Started |
| V-010 | Develop water management module | Developer | 10 days | V-007 | ⬜ Not Started |
| V-011 | Develop farmer management module | Developer | 10 days | V-007 | ⬜ Not Started |
| V-012 | Develop compliance tracking module | Developer | 10 days | V-007 | ⬜ Not Started |
| V-013 | Configure workflows and approvals | ERP Consultant | 5 days | V-007 | ⬜ Not Started |
| V-014 | Develop custom reports | BI Developer | 15 days | D-007 | ⬜ Not Started |
| V-015 | Develop ZATCA e-invoice integration | Integration Developer | 10 days | V-005 | ⬜ Not Started |
| V-016 | Develop GOSI integration | Integration Developer | 7 days | V-006 | ⬜ Not Started |
| V-017 | Setup email and notification system | System Administrator | 3 days | V-003 | ⬜ Not Started |
| V-018 | Configure print formats (Arabic/English) | ERP Consultant | 5 days | V-003 | ⬜ Not Started |
| V-019 | Implement data migration scripts | Data Engineer | 10 days | D-009 | ⬜ Not Started |
| V-020 | Execute data migration | Data Engineer | 5 days | V-019 | ⬜ Not Started |

#### **PHASE 7: TESTING**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| T-001 | Prepare test cases and scenarios | QA Lead | 7 days | D-010 | ⬜ Not Started |
| T-002 | Setup test environment | DevOps Engineer | 2 days | V-020 | ⬜ Not Started |
| T-003 | Unit testing of custom modules | QA Engineer | 10 days | V-012 | ⬜ Not Started |
| T-004 | Integration testing | QA Engineer | 10 days | V-016 | ⬜ Not Started |
| T-005 | User acceptance testing (UAT) | Business Users | 15 days | T-004 | ⬜ Not Started |
| T-006 | Performance testing | Performance Tester | 5 days | T-004 | ⬜ Not Started |
| T-007 | Security testing | Security Tester | 5 days | T-004 | ⬜ Not Started |
| T-008 | Compliance testing (regulations) | Compliance Officer | 5 days | T-004 | ⬜ Not Started |
| T-009 | Bug fixing and retesting | Development Team | 10 days | T-005 | ⬜ Not Started |
| T-010 | Final UAT sign-off | Business Owner | 2 days | T-009 | ⬜ Not Started |

#### **PHASE 8: TRAINING**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| R-001 | Develop training materials | Training Specialist | 10 days | V-018 | ⬜ Not Started |
| R-002 | Create user manuals (Arabic/English) | Technical Writer | 10 days | V-018 | ⬜ Not Started |
| R-003 | Create video tutorials | Training Specialist | 7 days | R-001 | ⬜ Not Started |
| R-004 | Conduct admin training | ERP Trainer | 5 days | R-001 | ⬜ Not Started |
| R-005 | Conduct finance user training | Finance Trainer | 3 days | R-001 | ⬜ Not Started |
| R-006 | Conduct HR user training | HR Trainer | 3 days | R-001 | ⬜ Not Started |
| R-007 | Conduct operations user training | Operations Trainer | 5 days | R-001 | ⬜ Not Started |
| R-008 | Conduct farmer portal training | Agricultural Trainer | 3 days | R-001 | ⬜ Not Started |
| R-009 | Training assessment and certification | Training Manager | 2 days | R-008 | ⬜ Not Started |
| R-010 | Create support documentation | Technical Writer | 5 days | R-002 | ⬜ Not Started |

#### **PHASE 9: GO-LIVE & OPERATIONS**

| Task ID | Task Description | Assigned Role | Duration | Dependencies | Status |
|---------|-----------------|---------------|----------|--------------|--------|
| O-001 | Prepare go-live checklist | Project Manager | 2 days | T-010 | ⬜ Not Started |
| O-002 | Setup production environment | DevOps Engineer | 3 days | T-010 | ⬜ Not Started |
| O-003 | Deploy system to production | DevOps Engineer | 1 day | O-002 | ⬜ Not Started |
| O-004 | Final data migration to production | Data Engineer | 2 days | O-003 | ⬜ Not Started |
| O-005 | Go-live announcement and cutover | Project Manager | 1 day | O-004 | ⬜ Not Started |
| O-006 | Hypercare support (2 weeks) | Support Team | 10 days | O-005 | ⬜ Not Started |
| O-007 | Monitor system performance | System Administrator | Ongoing | O-005 | ⬜ Not Started |
| O-008 | Setup backup and disaster recovery | DevOps Engineer | 3 days | O-005 | ⬜ Not Started |
| O-009 | Establish support ticketing system | Support Manager | 2 days | O-005 | ⬜ Not Started |
| O-010 | Regular compliance monitoring | Compliance Officer | Ongoing | O-005 | ⬜ Not Started |
| O-011 | Monthly performance review | Project Manager | Monthly | O-006 | ⬜ Not Started |
| O-012 | Continuous improvement planning | Business Analyst | Quarterly | O-011 | ⬜ Not Started |

---

## Entity Structure and SPV Creation

### Special Purpose Vehicle (SPV) in Saudi Arabia

#### What is an SPV?

A Special Purpose Vehicle (SPV) is a subsidiary company created for a specific business purpose, typically to:
- Isolate financial risk
- Facilitate project financing
- Separate assets and liabilities
- Enable joint ventures
- Access specific financing mechanisms

#### SPV Structures for Agriculture in KSA

##### Option 1: Limited Liability Company (LLC)
**Arabic**: شركة ذات مسؤولية محدودة

**Characteristics**:
- Minimum 2 partners (max 50)
- Minimum capital: SAR 500,000 (agricultural projects may vary)
- Limited liability to capital contribution
- Flexible management structure

**Best For**: Medium to large agricultural projects

**Formation Steps**:
1. Name reservation (MOCI)
2. Draft Articles of Association
3. Notarize documents
4. Deposit capital in bank
5. Register with MOCI
6. Obtain CR
7. Register with ZATCA, GOSI

**Timeline**: 2-4 weeks
**Cost**: SAR 5,000-15,000

##### Option 2: Closed Joint Stock Company
**Arabic**: شركة مساهمة مقفلة

**Characteristics**:
- Minimum 2 shareholders
- Minimum capital: SAR 500,000
- Shares not publicly traded
- Board of directors required

**Best For**: Large agricultural ventures, investor groups

**Formation Steps**: Similar to LLC but requires:
- Founding committee
- Prospectus
- CAMA approval
- Auditor appointment

**Timeline**: 3-6 months
**Cost**: SAR 20,000-50,000

##### Option 3: Agricultural Cooperative
**Arabic**: جمعية تعاونية زراعية

**Characteristics**:
- Minimum 5 members
- Democratic governance
- Profit sharing among members
- Tax benefits

**Best For**: Farmer collectives, community projects

**Registration**: MEWA + MOCI

**Timeline**: 4-8 weeks
**Cost**: SAR 2,000-10,000

#### SPV Capitalization

**Minimum Requirements**:
- LLC: SAR 500,000
- JSC: SAR 500,000
- Cooperative: SAR 50,000

**Recommended Capitalization for Agriculture**:
- Small farm (< 50 hectares): SAR 1-2 million
- Medium farm (50-200 hectares): SAR 5-10 million
- Large farm (> 200 hectares): SAR 20-50 million

#### SPV Governance

**Board Structure**:
- Chairman
- Managing Director/CEO
- Board Members (3-7 typical)
- Secretary

**Key Committees**:
- Audit Committee
- Risk Committee
- Compliance Committee

**Decision Making**:
- Major decisions: Board approval
- Day-to-day: Management authority
- Shareholder approval: Capital changes, dissolution

#### SPV Tax Treatment

**VAT**: Standard 15% (some agricultural inputs zero-rated)
**Zakat**: 2.5% of Zakat base
**Corporate Income Tax**: N/A for Saudi-owned companies
**Withholding Tax**: On payments to non-residents

---

## Farmer Company Formation

### Supporting Farmer Entrepreneurship

#### Farmer Company Models

##### Model 1: Individual Farmer Company
**Structure**: Single owner LLC or sole proprietorship
**Suitable For**: Individual landowners
**Capital**: SAR 100,000 minimum
**Process**: Simplified CR registration

##### Model 2: Farmer Group Company
**Structure**: Multi-partner LLC
**Suitable For**: 2-10 farmers pooling resources
**Capital**: SAR 500,000+
**Benefits**: Shared costs, combined expertise

##### Model 3: Agricultural Cooperative
**Structure**: Registered cooperative
**Suitable For**: 5+ farmers
**Capital**: SAR 50,000+
**Benefits**: Democratic control, tax advantages

##### Model 4: Contract Farming Partnership
**Structure**: Supply agreement with main entity
**Suitable For**: Farmers without capital for company
**Benefits**: Guaranteed market, technical support

### Step-by-Step Farmer Company Formation

#### Step 1: Pre-Formation (Week 1-2)

**Tasks**:
- [ ] Identify farmer participants
- [ ] Conduct feasibility study
- [ ] Determine company structure
- [ ] Calculate capital requirements
- [ ] Secure land rights/leases
- [ ] Identify water sources

**Required Documents**:
- ID copies of all partners
- Land ownership/lease documents
- Water source documentation
- Business plan outline

**Support Needed**:
- Agricultural extension officer
- Legal advisor
- Financial advisor

#### Step 2: Name Reservation (Week 2)

**Tasks**:
- [ ] Choose company name (Arabic + English)
- [ ] Check name availability on MOCI portal
- [ ] Reserve name

**Platform**: https://cr.mc.gov.sa/
**Cost**: SAR 200
**Validity**: 60 days

#### Step 3: Documentation (Week 2-3)

**Tasks**:
- [ ] Draft Memorandum of Association
- [ ] Define partner shares
- [ ] Specify company activities
- [ ] Set governance rules
- [ ] Notarize at Ministry of Justice

**Required Documents**:
- Articles of Association
- Partner agreements
- Lease agreement (office address)
- Capital contribution proof

**Professional Help**: Corporate lawyer

#### Step 4: Capital Deposit (Week 3)

**Tasks**:
- [ ] Open temporary bank account
- [ ] Partners deposit capital
- [ ] Obtain bank certificate

**Minimum Amounts**:
- Individual: SAR 100,000
- LLC: SAR 500,000
- Cooperative: SAR 50,000

#### Step 5: Commercial Registration (Week 3-4)

**Tasks**:
- [ ] Submit online CR application
- [ ] Upload required documents
- [ ] Pay registration fees
- [ ] Receive CR certificate

**Platform**: https://cr.mc.gov.sa/
**Timeline**: 1-7 days
**Cost**: SAR 200-1,200

#### Step 6: Post-Registration (Week 4-6)

**Tasks**:
- [ ] Convert to permanent bank account
- [ ] Register with ZATCA (VAT/Zakat)
- [ ] Register with GOSI (if hiring)
- [ ] Obtain municipal license
- [ ] Apply for MEWA agricultural license

**Timeline**: 2-4 weeks
**Costs**: SAR 1,000-5,000

#### Step 7: Operational Setup (Week 6-8)

**Tasks**:
- [ ] Setup accounting system
- [ ] Hire initial staff
- [ ] Obtain required equipment
- [ ] Establish supplier relationships
- [ ] Begin agricultural operations

### Farmer Support Programs

#### MEWA Support

**Programs**:
- Agricultural Development Fund (ADF) loans
- Subsidized inputs (seeds, fertilizers)
- Technical training
- Extension services

**Contact**: ADF - https://www.adf.gov.sa/

#### SIDF Support

**Saudi Industrial Development Fund**:
- Project financing
- Feasibility study support
- Technical consultation

**Contact**: https://www.sidf.gov.sa/

#### Government Grants

**Available Programs**:
- Small farm development grants
- Technology adoption incentives
- Water conservation subsidies
- Organic certification support

### Farmer Training and Capacity Building

**Training Areas**:
- Business management
- Financial literacy
- Marketing and sales
- Quality control
- Compliance and record keeping
- ERP system usage

**Training Providers**:
- MEWA extension services
- Agricultural cooperatives
- Private consultants
- Online platforms

---

## MEWA and NCEC Compliance

### Ongoing Compliance Requirements

#### MEWA Compliance

**Annual Requirements**:
1. License renewal (30 days before expiry)
2. Production reports (quarterly)
3. Water usage reports (monthly)
4. Pesticide usage reports (quarterly)
5. Inspection compliance (as scheduled)

**Reporting Platform**: https://eservices.mewa.gov.sa/

**Key Metrics to Track**:
- Crop yields
- Water consumption
- Fertilizer/pesticide use
- Land utilization
- Workforce numbers

**Penalties for Non-Compliance**:
- Warning letter
- Fine: SAR 1,000-100,000
- License suspension
- License revocation

#### NCEC Compliance

**Regular Submissions**:
1. Environmental monitoring reports (quarterly)
2. Waste management reports (annually)
3. Emissions data (if applicable)
4. Incident reports (within 24 hours)
5. Compliance certificates (annually)

**Monitoring Requirements**:
- Water quality testing
- Soil testing
- Air quality (if applicable)
- Waste characterization

**Inspection Frequency**:
- High risk: Quarterly
- Medium risk: Semi-annually
- Low risk: Annually

**Digital Compliance**:
- Register on: https://eservices.ncec.gov.sa/
- Upload reports digitally
- Track inspection schedules
- Receive alerts

#### Labor Law Compliance

**Monthly Requirements**:
- [ ] Pay salaries through WPS by 7th
- [ ] Submit GOSI contributions by 15th
- [ ] Update employee records on Qiwa
- [ ] Maintain time and attendance records

**Quarterly Requirements**:
- [ ] Review Nitaqat status
- [ ] Submit GOSI reports
- [ ] Conduct safety inspections
- [ ] Review employment contracts

**Annual Requirements**:
- [ ] Renew work permits/iqamas
- [ ] Annual leave reconciliation
- [ ] Safety training refresher
- [ ] Policy updates

**Record Keeping (5 years minimum)**:
- Employment contracts
- Salary records
- Leave records
- Disciplinary actions
- Training records

### Compliance Monitoring in ERP

**ERP Modules for Compliance**:

1. **Regulatory Compliance Tracker**
   - License expiry alerts
   - Renewal reminders
   - Compliance calendar
   - Document repository

2. **Environmental Monitoring**
   - Water usage tracking
   - Chemical usage logs
   - Waste management records
   - Emission tracking

3. **HR Compliance**
   - WPS integration
   - GOSI reporting
   - Contract management
   - Leave management
   - Nitaqat monitoring

4. **Quality Compliance**
   - Testing schedules
   - Lab results
   - Certification tracking
   - Audit trails

5. **Financial Compliance**
   - VAT reporting
   - Zakat calculation
   - E-invoicing (FATOORA)
   - ZATCA integration

---

## ERP Configuration for Agriculture

### Agriculture-Specific Modules

#### 1. Farm Management
- Farm/plot registration
- Soil data management
- Irrigation scheduling
- Equipment tracking
- Maintenance planning

#### 2. Crop Planning
- Crop rotation planning
- Planting schedules
- Harvest forecasting
- Yield tracking
- Variety management

#### 3. Water Management
- Water source tracking
- Consumption monitoring
- Irrigation efficiency
- MEWA reporting integration
- Cost allocation

#### 4. Farmer Portal
- Contract management
- Payment tracking
- Quality reporting
- Communication platform
- Training materials

#### 5. Compliance Dashboard
- License tracker
- Inspection scheduler
- Report generator
- Alert system
- Document manager

#### 6. Quality Control
- Testing schedules
- Lab integration
- Certificate tracking
- Traceability
- Recall management

#### 7. Supply Chain
- Procurement
- Inventory (seeds, fertilizers, chemicals)
- Logistics
- Cold chain monitoring
- Supplier management

### Saudi-Specific Customizations

1. **Arabic Language Support**
   - RTL interface
   - Arabic reports
   - Bilingual data entry

2. **ZATCA E-Invoice Integration**
   - Phase 1 compliance (XML generation)
   - Phase 2 compliance (API integration)
   - QR code generation
   - Archive management

3. **GOSI Integration**
   - Employee registration
   - Monthly contributions
   - Wage calculations
   - Report generation

4. **Hijri Calendar**
   - Dual calendar system
   - Hijri-Gregorian conversion
   - Reporting in both calendars

5. **Qiwa Integration**
   - Employee sync
   - Visa management
   - Contract submission
   - Nitaqat monitoring

---

## Additional Resources

### Government Portals

- **MEWA**: https://www.mewa.gov.sa/
- **NCEC**: https://ncec.gov.sa/
- **MOCI**: https://mc.gov.sa/
- **HRSD**: https://www.hrsd.gov.sa/
- **ZATCA**: https://zatca.gov.sa/
- **GOSI**: https://www.gosi.gov.sa/
- **Qiwa**: https://qiwa.sa/

### Useful Contacts

- **MEWA Helpline**: 920000911
- **NCEC**: 8001220002
- **MOCI**: 920000667
- **HRSD**: 19911
- **ZATCA**: 19993
- **GOSI**: 8001243344

### Legal References

- Saudi Labor Law: Royal Decree No. M/51 (2005)
- Companies Law: Royal Decree No. M/3 (2015)
- Environmental Law: Royal Decree No. M/34 (2001)
- Agriculture Law: Royal Decree No. M/8 (2019)
- VAT Law: Royal Decree No. M/113 (2017)

---

## Implementation Timeline Summary

| Phase | Duration | Key Deliverables |
|-------|----------|------------------|
| Consulting & Planning | 4 weeks | Project charter, requirements |
| Legal & Regulatory | 8-12 weeks | All licenses and registrations |
| SPV & Entity Creation | 4-8 weeks | Company formation complete |
| Farmer Companies | 6-10 weeks | Farmer entities established |
| System Design | 4 weeks | Technical specifications |
| Development | 8-12 weeks | Configured ERP system |
| Testing | 4-6 weeks | UAT sign-off |
| Training | 3-4 weeks | Trained users |
| Go-Live | 2 weeks | Production system live |
| **Total** | **24-30 weeks** | **Fully operational system** |

---

## Notes

- All timelines are estimates and may vary based on specific circumstances
- Regulatory requirements may change - always verify current requirements
- Consult with licensed legal and financial professionals for specific advice
- This guide is for informational purposes and does not constitute legal or professional advice

---

**Last Updated**: December 2024  
**Next Review**: March 2025

For questions or updates, please contact the project team.
