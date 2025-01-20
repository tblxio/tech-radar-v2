# How to use the Technology Radar

## Introduction
tb.lx Tech Radar is our technology portfolio management tool. It reflects both established and emerging technologies being evaluated, adopted, or deprecated within our company. This tool supports teams in choosing the right technologies for future products and projects, fostering informed and consistent decision-making.

These guidelines outline the process for maintaining and updating the Tech Radar, ensuring it remains relevant, transparent, and collaborative. They aim to:
- Keep the Tech Radar current and accurate.
- Promote transparency in tech decisions.
- Encourage open collaboration and contributions from all team members.
- Streamline decision-making through a structured review process.

---

## Roles and Responsibilities
- **Core Engineering Leadership Team:** Responsible for conducting a full review of the Tech Radar every 3 months. Provides final approval on significant changes.
- **Tech Radar Maintainers:** Principal Engineers are responsible for reviewing incoming Pull Requests (PRs). This group ensures that contributions comply with guidelines and maintain overall Radar quality.
- **Contributors:** All tblxers are encouraged to propose new technologies or suggest changes to existing technology statuses. Contributors submit PRs, following the repository's guidelines and providing the necessary supporting documentation.

---

## Technology Statuses and Adoption process
The Tech Radar classifies technologies into four categories, reflecting their maturity and adoption level within tb.lx:

- **ASSESS:**
  - The technology is under evaluation by a team.
  - An ADR is required to ensure the evaluation is transparent, aligned with engineering principles, and documented

- **TRIAL:**
  - The technology is being tested in production by at least one product
  - The goal is to determine if it should be promoted as a tb.lx standard.
  - A proven track record in a production environment is essencial before advancing.

- **ADOPT:**
  - The technology has demonstrated clear value in production use-cases.
  - It is considered a tb.lx standard and is widely recommended for use.

- **HOLD:**
  - The technology is being deprecated at tb.lx.
  - Its usage is not recommended, and it should be phased out over time.
  - A deprecation ADR is required.

---

## Technology Categories (Quadrants)
To help organize and understand our technology ecosystem, the Tech Radar is divided into quadrants. These quadrants group technologies by their primary purpose and domain:

- **1. Programming Languages & Frameworks:**
  - General-purpose or domain specific languages used to write application code, alongside essential frameworks that implement common patterns and functionalities.
  - Examples: TypeScript, Kotlin, Scala, Rust, React, Next.js, Spring Boot.

- **2. Platforms & Infrastructure:**
  - Hosted environments, cloud services, container platforms, or foundational managed solutions upon which applications are deployed or run.
  - Examples: AKS, Azure B2C, MongoDB Atlas, Node.js

- **3. Developer Tools:**
  - Tools, services, or utilities that help us build, test, secure, and maintain our applications. Used mostly for development, CI/CD, monitoring, or operational tasks.
  - Examples: Terraform, Docker, GitHub Actions, Grafana.

- **4. Methods & Patterns:**
  - Key Software development methods and Design Patterns, covering everything from Continuous Integration and testing, to Architecture.
  - Examples: TDD, DevSecOps, GitOps, Component-driven Development, etc.

---

## Contributing to the Tech Radar

- **Before Opening a PR:**
  - Review the contributing guidelines in the repository's README file
  - Determine the right category (quadrant) for your technology by reviewing the definitions above.
  - Ensure your contribution does not contain sensitive or proprietary information, as the repository is public.

- **Adding a New Technology (ASSESS):**
  - Submit a PR to introduce the technology as "ASSESS", in the relevant quadrant (e.g. Programming Languages, Frameworks & Libraries, etc.).
  - The PR should include a description detailing why the technology is relevant.

- **Moving from ASSESS to TRIAL:**
  - Only move a technology to "TRIAL" after it has been successfully evaluated and tested.
  - The PR should include a summary of findings and a link to the ADR.

- **Moving from TRIAL to ADOPT:**
  - Promote a technology to "ADOPT" once it has clearly proven its value in production environments.
  - Include evidence of successful implementations, or other supporting data in the PR.

- **Marking a technology as HOLD:**
  - If the technology no longer aligns with tb.lx goals or is being phase out, submit a PR to mark it as "HOLD".
  - Provide a brief explanation for the decision to deprecate.

---

## Open-Source considerations
Since the Tech Radar is public, contributors must:
- Omit sensitive, internal, or private company information from all code submitted in PRs.
- When writing PR descriptions, consider providing only high-level rationales suitable for an external audience.

By following these guidelines, we ensure that tb.lx Tech Radar remains a reliable, and transparent tool that evolves with our technological landscape. All tblxers are encouraged to collaborate, contributing to a shared understanding of our engineering direction and helping drive informed, and strategic decisions. 
