# CertifiedSloperator
Just some markdown describing recent projects with coding agents.

## ChatGPT

I used this in 2024 to generate silly profile photos for API accounts that would show in Chatter feeds, to add whimsy.

## Gemini

Syntax help across Powershell, Okta Language Syntax, MuleSoft, RHEL9, OpenSSL, jq parsing, JSON filtering.

## Claude Code

Chronological list of 11 projects built with Claude's assistance, ordered by creation date.

---

## 1. **SF API Tool** - Mutual TLS Salesforce Authenticator
`/sf_api_tool/` | **Created:** Feb 20, 2026 3:29 PM

A secure Rust-based tool for Salesforce authentication using JWT Bearer Flow with optional (but not yet functioning) mutual TLS (mTLS).

**Key Features:**
- Self-signed certificate generation (OpenSSL)
- JWT Bearer Token authentication (RS256)
- Interactive command confirmation
- SOQL query execution
- SetupEntityAccess permission auditing with tree visualization
- Concurrent SOQL queries using Tokio async runtime

**Technology:** Rust, Salesforce API v59.0, OpenSSL, mTLS, Tokio, ascii_tree

---

## 2. **ALRAD** - Enterprise RADIUS Authentication
`/alrad/` | **Created:** Feb 22, 2026 10:50 PM

A FreeRADIUS server implementation using Perl.

**Key Features:**
- Documentation of flow  functions to better visualize what-happens-when

**Technology:** FreeRADIUS 3.x with Perl modules, Okta API

---

## 3. **DataWeave Name Capitalization** - Identity Provisioning Transformer
`/dataweave_allcaps/` | **Created:** Feb 23, 2026 10:14 PM

A MuleSoft DataWeave transformation that normalizes all-caps names from Workday resumé imports for identity management systems.

**Key Features:**
- Detects and transforms ALL CAPS names → Proper Case
- Preserves intentional mixed-case formatting
- Multiple script variants (single Name field vs. FirstName/LastName)
- Logging variants for audit trails

**Technology:** DataWeave 2.0, Mule 4/MuleSoft Composer

---

## 4. **Okta App Naming Convention** - Provisioning Workflow Designer
`/okta_app_naming_convention/` | **Created:** Feb 25, 2026 12:26 PM

A workflow design for generating optimal Okta application labels upfront during provisioning (Slack/API integration).

**Key Features:**
- Label generator algorithm (production-ready Python)
- Analysis of existing Okta apps
- Three naming convention proposals (Strict/Relaxed/Prefix-Based)
- Slack workflow templates and questionnaire design
- Emphasizes user-facing names vs. technical details in admin notes

**Technology:** Python 3, Okta API, workflow design documentation

---

## 5. **Ratty Refactor** - OAuth Device Flow Integration
`/ratty_refactor/` | **Created:** Feb 25, 2026 3:59 PM

OAuth Device Code Flow integration into the ratty tool (Salesforce CLI) for External Client Application authentication.

**Key Features:**
- OAuth device flow implementation
- Automatic token refresh (5 min before expiration)
- Password fallback for legacy support
- 100% backwards compatible
- Multi-source configuration (CLI/env/file)

**Technology:** Python 3, Salesforce OAuth 2.0 Device Flow

---

## 6. **PowerShell Okta Module** - Native Okta CRUD Operations
`/powershell_okta_crud_ops/` | **Updated:** Feb 26, 2026 10:56 AM

A PowerShell module providing 100+ native cmdlets for Okta's REST APIs.

**Key Features:**
- User and group management

**Technology:** PowerShell 5+, Okta REST API

---

## 7. **Salesforce Case Creation** - Database Patching Automation
`/dbcreation_py/` | **Created:** Feb 26, 2026 1:31 PM

Python scripts for automated Salesforce case creation for database ops.

**Key Features:**
- Parses CSV spreadsheets with schedules
- Creates Change Cases with implementation plans
- SF CLI authentication (OAuth)
- Supports multiple case types
- Automatic infrastructure type detection

**Technology:** Python 3.9+, Salesforce API, gus library

---

## 8. **Hammer Tools** - Salesforce Release Automation
`/hammer_tools/` | **Created:** Feb 26, 2026 5:22 PM

A Python CLI tool for automating Salesforce tasks.

**Key Features:**
- Generates implementation plans from templates
- SF CLI authentication support

**Technology:** Python 3.9+, Salesforce API

---

## 9. **Permission Dependencies Finder** - Permission Set XML Analyzer
`/findingpermissiondependencies/` | **Created:** Feb 26, 2026 9:42 PM

Taking the PermissionDependency mapping and making a tree directory structure of Salesforce Permissions.

**Key Features:**
- "DependentOnWhat" Permission Set
- Contains objectPermissions and userPermissions entries
- Analyzes system-level permissions (AICreateInsightObjects, AccessCMC, ActivateContract, etc.)

**Technology:** GoLang, Bash scripting, Salesforce API

---

## 10. **Sandbox Dashboard** - Salesforce Admin Tool
`/sandbox_dashboard/` | **Created:** Feb 26, 2026 10:48 PM

A Ruby on Rails application providing quick access to Salesforce sandbox information and login URLs (faster alternative to slow Setup page).

**Key Features:**
- Derives sandbox My Domain URLs from production org
- Queries Salesforce Tooling API (SandboxProcess, SandboxInfo)
- Displays sandbox status, type, activation dates
- Direct login links for each sandbox

**Technology:** Ruby 3.3.10, Rails, Salesforce API

---

## 11. **BusinessProcess Extractor** - Salesforce Picklist Scraper
`/businessprocess_extract/` | **Created:** Feb 27, 2026 12:18 AM

A Python tool that extracts picklist values from Salesforce BusinessProcess records by scraping the web UI (data not available via API).

**Key Features:**
- Queries BusinessProcess and RecordType via SOQL
- Uses SF CLI session auth to scrape web pages
- Parses HTML dueling picklists to extract selected values
- Outputs consolidated JSON and CSV reports

**Technology:** Python 3.7+, Salesforce CLI

---

## Summary Statistics

- **Total Projects:** 11 directories
- **Languages Used:** Python (5), Rust (2), PowerShell (1), Ruby (1), DataWeave (1), Perl (1)
- **Primary Domains:**
  - Salesforce automation & tooling (7 projects)
  - Okta integration & identity (3 projects)
  - Enterprise authentication (1 project)
- **Documentation Created:** 40+ comprehensive markdown files
- **Authentication Methods Implemented:** JWT Bearer Flow, OAuth Device Flow, RADIUS, SAML, mTLS
