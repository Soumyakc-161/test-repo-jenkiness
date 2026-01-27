
---

# 🧪 test_22-01-2026 — Jenkins + Azure ARM Test Repository

## 📌 Purpose of this Branch

The **`test_22-01-2026`** branch is a **dedicated testing branch** used to validate **Jenkins CI/CD pipelines with Azure ARM templates**.

This branch allows safe experimentation **without impacting the main production codebase**.

---

## 🎯 What This Branch Is Used For

* ✅ Testing **Jenkins integration with GitHub**
* ✅ Validating **branch-based pipeline execution**
* ✅ Deploying Azure resources using **ARM templates**
* ✅ Verifying pipeline failure scenarios (syntax errors, missing files, wrong branch, etc.)
* ✅ End-to-end testing of **CI/CD flow before merging to main**

---

## 🚫 What This Branch Is NOT For

* ❌ No production deployments
* ❌ No changes to the `main` branch
* ❌ No direct use for live environments
* ❌ No direct use of `main` branch

> ⚠️ **Main branch must remain untouched** while testing is performed here.

---

## 🏗️ Resources Created From This Branch

ARM templates in this branch may create:(after creating resource take screenshort and delete them,)

* Resource Group 
* Storage Account
* Azure Data Factory
* Linked Services
* Datasets
* Pipelines
* Integration Runtimes

> All resources are **test resources only** and can be safely deleted after validation.

---

## 🔁 CI/CD Workflow (High Level)

1. Developer pushes changes to `test_22-01-2026`
2. Jenkins pipeline is triggered
3. Jenkins validates:

   * Correct branch name
   * ARM JSON syntax
   * Required files existence
4. ARM templates are deployed to Azure (test scope)
5. Pipeline succeeds or fails with clear error logs
6. No impact on `main` branch

---


---

## ✅ When to Use This Branch

Use `test_22-01-2026` when you need to:

* Test Jenkins pipeline logic
* Validate new ARM templates
* Debug Azure deployment issues
* Demonstrate CI/CD flow

---

## 👤 Ownership

This branch is maintained **only for CI/CD testing purposes**.
All validated changes must be reviewed before being applied to the `main` branch.

---


