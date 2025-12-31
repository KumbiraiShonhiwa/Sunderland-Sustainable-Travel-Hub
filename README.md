# 🌱 Sunderland Sustainable Travel Hub

A modern, student-friendly digital platform designed to help University of Sunderland students make **informed and sustainable travel choices**.
The project replaces an existing text-heavy SharePoint page with an **interactive, accessible, and maintainable travel hub**.

---

## 📌 Project Overview

The **Sunderland Sustainable Travel Hub** restructures and enhances existing sustainability travel content into an intuitive web-based hub. The solution is built **within SharePoint constraints** while allowing **frontend flexibility** through modern web technologies.

The project uses the **Sunderland Ticket Navigator** prototype as a design and user-flow reference to accelerate delivery and reduce unnecessary redesign.

---

## 🎯 Objectives

* Improve student access to clear, actionable travel information
* Promote sustainable travel options
* Replace static content with an interactive hub
* Ensure accessibility and ease of navigation
* Deliver a SharePoint-compatible, maintainable solution
* Provide real-world development experience for students

---

## 🏗️ System Architecture

### High-Level Architecture

```
React Frontend (Ant Design + GSAP)
            ↓
SharePoint Framework (SPFx)
            ↓
SharePoint REST API
            ↓
SharePoint Lists (Backend Data Layer)
```

This **platform-native, serverless architecture** ensures security, maintainability, and compatibility with university systems.

---

## 🧩 Technology Stack

### Frontend

* **React** + **TypeScript**
* **SharePoint Framework (SPFx)**
* **Ant Design** (UI components)
* **GSAP** (animations & transitions)

### Backend

* **SharePoint Online**
* **SharePoint Lists** (structured data storage)
* **SharePoint REST API** (data access)
* **Power Automate** (workflows & automation)
* **Microsoft Entra ID (Azure AD)** (authentication & permissions)

---

## 🔙 Backend Approach (No Custom API)

This project does **not** implement a traditional backend server or custom API.

Instead, the backend focuses on:

* Data modelling and structure (SharePoint Lists)
* Permissions and security configuration
* Automation and validation using Power Automate
* Enabling clean data access through SharePoint’s built-in REST API

This approach:

* Reduces technical risk
* Requires no server maintenance
* Supports long-term handover to non-technical staff

---

## 🎨 Frontend Approach

The frontend is a **fully flexible React application** hosted inside SharePoint via SPFx.

Key principles:

* Loose coupling between UI and data sources
* Service-layer abstraction for REST API calls
* Client-side filtering, sorting, and interactions
* Accessibility-first design
* Smooth animations using GSAP

This allows modern frontend development **without breaking SharePoint compatibility**.

---

## ♿ Accessibility & Usability

* Semantic HTML and accessible UI components
* Clear navigation and readable content structure
* Keyboard-friendly interactions
* Designed for a diverse student user base

---

## 📂 Project Scope

### In Scope

* Content restructuring and validation
* SharePoint-compatible frontend and backend
* Accessibility improvements
* Stakeholder feedback and refinement
* Final documentation and handover

### Out of Scope

* Real-time travel APIs
* Mobile application development
* Custom backend servers
* Ongoing maintenance after handover

---

## 👥 Team Structure

* **Project Manager** – Coordination, communication, delivery
* **Backend Team** – Data architecture, permissions, automation
* **Frontend Team** – UI, UX, animations, data presentation
* **Research & Content Team** – Travel research and sustainability focus

---

## 🧠 Key Learning Outcomes

* Platform-native backend development
* SharePoint as a headless CMS
* REST API consumption in SPFx
* Frontend–backend contract design
* Accessibility-aware web development
* Real-world project collaboration

---

## 📄 Documentation

Project documentation includes:

* Backend infrastructure guide
* Backend role definition
* Frontend architecture & documentation
* Architecture diagrams
* Handover notes for Sustainability Team

---

## ✅ Success Criteria

The project is successful if:

* Students can easily find relevant travel information
* The Sustainability Team confirms improved usability
* Accessibility and sustainability goals are met
* The solution is delivered within agreed timelines

---

## 🔄 Continuous Integration (GitHub Actions)

This project uses **GitHub Actions** to support a lightweight and reliable **Continuous Integration (CI)** workflow.
The goal is to maintain code quality and stability while respecting **SharePoint governance constraints**.

### Why GitHub Actions Are Used

* Validate frontend builds before merging
* Enforce consistent code style and quality
* Detect dependency vulnerabilities early
* Reduce integration issues in a student-led team
* Support collaborative development without automating deployment

Automated deployment is **intentionally excluded**, as SharePoint solutions require controlled, manual deployment.

---

### Active Workflows

#### ✅ Frontend Build & Lint

Runs on every push and pull request to ensure the React + SPFx frontend:

* Installs dependencies successfully
* Passes linting checks
* Builds without errors

This prevents broken SPFx builds from reaching the main branch.

---

#### 🧹 Code Quality Checks

Enforces consistent formatting and coding standards using ESLint and Prettier.
This improves readability, reduces merge conflicts, and ensures maintainable code.

---

#### 🔐 Dependency Security Scanning

Regularly scans project dependencies for known vulnerabilities.
This supports security best practices expected in institutional environments.

---

#### 📝 Documentation Validation (Optional)

Checks Markdown files for formatting issues to maintain professional documentation quality.

---

### What CI Does *Not* Do

* Deploy to SharePoint automatically
* Manage authentication secrets
* Provision infrastructure
* Modify SharePoint environments

All deployments are handled **manually** to ensure compliance and reduce risk.

---

## 📜 License

This project is developed for academic and institutional use by the **University of Sunderland Sustainability Team**.

---
