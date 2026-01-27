

---

# main — Azure ARM Infrastructure (Production-Ready)

##  Purpose of the Main Branch

The **`main`** branch represents the **stable, production-ready source of truth** for Azure infrastructure defined using **ARM templates**.

This branch contains **approved, tested, and validated code only** and is used for **controlled deployments** via Jenkins CI/CD pipelines.

---

##  What This Branch Is Used For

*  Production-ready Azure ARM templates
*  Jenkins CI/CD deployments to stable environments
*  Infrastructure consistency across environments
*  Audit-friendly and version-controlled deployments
*  Long-term maintenance and enhancements

---

##  What This Branch Is NOT For

* No experimental changes
* No pipeline testing
* No ad-hoc debugging
* No direct commits without review

>  **All changes must be tested in a dedicated test branch before merging into `main`.**

---

##  Azure Resources Managed From `main`

ARM templates in this branch can deploy and manage:

* Resource Groups
* Storage Accounts
* Azure Data Factory
* Linked Services
* Datasets
* Pipelines
* Integration Runtimes

> All deployments are **idempotent and controlled** through Jenkins.

---

##CI/CD Workflow (Production)

1. Changes are developed and validated in a test branch
2. Pull Request is created to merge into `main`
3. Code review and approval are completed
4. Jenkins pipeline is triggered for `main`
5. ARM templates are validated
6. Azure resources are deployed/updated safely
7. Deployment status is logged and auditable

---

##  Quality & Safety Controls

The `main` branch enforces:

* Branch-based pipeline execution
* ARM template validation before deployment
* Secure handling of secrets (`secureString` parameters)
* Clear error reporting for failures
* Controlled deployment scope (Prod / Stable environments)

---

##  Relationship With Test Branches

| Branch            | Purpose                       |
| ----------------- | ----------------------------- |
| `test_22-01-2026` | CI/CD testing & validation    |
| `main`            | Stable, production-ready code |

>  **Only validated code from test branches is merged into `main`.**

---

## Why This Branch Matters

Using a protected `main` branch ensures:

*  Infrastructure stability
*  Clear change history
*  Repeatable deployments
*  Confidence in automation
*  Enterprise-grade DevOps practices

---

## 👤 Ownership & Governance

* All changes to `main` must go through:

  * Pull Request
  * Review
  * Approval
* Direct commits are **strongly discouraged**

---

##  When to Use the Main Branch

Use `main` when you need to:

* Deploy stable Azure infrastructure
* Promote tested changes to production
* Demonstrate enterprise CI/CD workflows
* Maintain long-term infrastructure code

---


