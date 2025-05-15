# Source Control with GitHub for Websites, Power Platform, and SQL.
**Improving Collaboration, Version History, and Deployment Confidence**  
**Presented by:** Bryan Barker
**Date:** Next Wednesday

---

## Current State – Website & Power Apps Development

**Web Development:**
- Developers manage everything locally or directly on the host server.
- No version history or tracking of changes.
- Risk of overwriting each other’s work or losing prior versions.

**Power Apps Development (Pipelines):**
- Power Platform Pipelines move apps from Dev → Test → Prod.
- Click-to-deploy approach with strong governance.
- Great for simplicity and control, but lacks file-based source tracking.

**Challenge:**  
No centralized record of what changed, who changed it, or why.

---

## What We're Missing Without GitHub

Without GitHub integration, we lose out on:

- Version history: No audit trail of who made changes and when.
- Team collaboration: No pull requests, peer reviews, or approvals.
- Branching strategies: Difficult to test or hotfix features independently.
- Backups outside the platform: No rollback options beyond last deployment.
- CI/CD integration: Can’t plug into modern pipelines like GitHub Actions or Azure DevOps.

---

## What GitHub Enables

GitHub combined with Power Platform or Web Development allows us to:

- Track changes and ensure accountability.
- Experiment safely with branching and merging strategies.
- View organized, readable file versions of Power Apps and website code.
- Introduce code reviews and approval processes.
- Capture institutional knowledge through commit messages and pull requests.
- Integrate with automation tools to improve consistency and speed.

---

## Hybrid Setup – Best of Both Worlds

| Task                      | Tool                                      |
|---------------------------|-------------------------------------------|
| Local Dev / Testing       | Power Apps Studio / Local Dev Environment |
| Deploy to Test / Prod     | Power Platform Pipelines                  |
| Version Control / History | GitHub (unpacked solution format)         |
| Backup / Collaboration    | GitHub                                    |
| Optional Automation       | GitHub Actions or Azure DevOps            |

---

## Next Step Options

**Option 1 – Minimal Lift**
- Continue using Power Platform Pipelines for deployment.
- Introduce GitHub for version control and change tracking.
- Requires little change to current workflows but adds major value.

**Option 2 – Full ALM Integration**
- Use GitHub Actions to automate export, unpacking, validation, and deployment.
- Build approval gates and version bumping into the pipeline.
- Supports scalability and stronger governance over time.

---

## Why Now?

- Growing complexity in apps and websites.
- Increasing collaboration across departments.
- Need for accountability, version tracking, and rollback capabilities.
- A modern DevOps approach aligns with long-term scalability and enterprise readiness.

---
## Web Development Integration with GitHub

**Current State:**
- Developers manage websites locally or directly on the host server
- No version history or audit trail
- Risk of accidental overwrites, missed changes, or miscommunication
- Manual file transfers without peer review

**What We Can Do:**
- Move web source files (HTML, CSS, JS, PHP, etc.) into GitHub repositories
- Use branches to isolate feature work or bug fixes
- Enable pull requests and peer reviews before changes are published
- Track all edits with meaningful commit messages

**Outcome:**
- Improved collaboration and communication across developers
- Reduced deployment risk through versioned, peer-reviewed changes
- Faster troubleshooting and rollback capabilities

---
## Power Platform Integration with GitHub

**Current State:**
- Using Power Platform Pipelines for Dev → Prod deployment
- No source control or version history for apps, flows, or solution components
- Hard to track changes, who made them, or when
- No rollback or structured testing process

**What We Can Do:**
- Export unmanaged Power Platform solutions and unpack them into GitHub
- Track all Power Apps, flows, tables, and variables as readable files
- Use GitHub branches to simulate environments (dev, test, prod)
- Optionally add GitHub Actions for solution validation and deployment

**Outcome:**
- Full visibility into changes made to Power Platform components
- Collaboration and peer review processes aligned with modern DevOps
- Gradual path toward automated CI/CD for Power Platform

---

## SQL & Azure Integration with GitHub

**Current State:**
- No dev/prod split for SQL or Azure services
- Manual deployment of scripts or configuration
- No version control for database changes

**What We Can Do:**
- Store and track SQL scripts and Azure configuration in GitHub
- Use branches to simulate environments and approve changes
- Begin scripting repeatable deployments (PowerShell, Azure CLI)
- Prepare for GitHub Actions automation

**Outcome:**
- Enables version control, collaboration, and rollback
- Positions us for DevOps maturity when we're ready to split environments

---


## Slide 7: Recommendation

Begin GitHub adoption for both Power Platform and website projects:

- Start with one solution and one repository as a pilot.
- Use GitHub for source control and documentation.
- Continue using current deployment tools to maintain continuity.
- Expand automation and DevOps practices as comfort and maturity grow.

**Outcome:**  
Improved collaboration, reduced operational risk, and better visibility across teams.
