<div align="center">
  <img src="./banner.svg" alt="Carlos Voliv Banner" width="100%" />
</div>

<br />

<div align="center">
  <a href="https://www.linkedin.com/in/carlosvoliv/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:vazkdu@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <img src="https://komarev.com/ghpvc/?username=carlosvoliv&style=flat-square&color=0878A6&label=Profile+Views" alt="Profile Views" />
</div>

---

### 🚀 About Me

I am a **Full-Stack Software Engineer** specializing in the design and development of complex **credit and financial-formalization systems**. My work sits at the intersection of business-critical operations, structured domains, and highly reliable code pipelines. 

With a strong foundation in **Domain-Driven Design (DDD)** and architectural patterns, I bridge the gap between robust backends (PHP/Laravel) and performant, intuitive frontends (Vue.js/TypeScript). I'm committed to code quality, maintaining an average of **~92% automated testing coverage** across the systems I design and own.

---

### 💼 What I Do (Day to Day)

At my day job within a private fintech, I design and build the automated pipeline that transforms a raw PDF credit document into a registered, securitized receivable. This complex flow involves:

1. **Document Extraction:** Parsing raw credit files (PDFs) and extracting clean, structured domain models.
2. **Clearinghouse Registry:** Orchestrating batch registrations with major clearinghouses (**B3**, **Núclea**).
3. **Bank Exchange (CNAB):** Standardizing communication with partner banks via CNAB file generation, reading, and validation.
4. **Operator UI:** Creating high-fidelity, reactive dashboards that operators use to audit and resolve exceptions.

Here is a visual map of how these components connect:

```mermaid
graph TD
    A[📄 Raw Credit Document] -->|Parsing| B["Document Extraction<br/>(credit-doc-extract)"]
    B -->|Structured Data| C{DDD Validation Engine}
    C -->|Invalid| D[❌ Rejected / Manual Audit]
    C -->|Valid| E[💼 Receivable]
    E --> F[🏦 Clearinghouse Registry]
    F -->|Batch Registration| F1(B3)
    F -->|Batch Registration| F2(Núclea)
    E --> G["CNAB Exchange<br/>(cnab-toolkit)"]
    G -->|Bank Files| H[🏦 Partner Banks]

    %% UI Layer
    I["🎨 Operator UI<br/>(facet-ui)"] -.->|Review| B
    I -.->|Dashboard| F
    I -.->|Manual Intervention| D

    style A fill:#141414,stroke:#4db3d4,stroke-width:2px,color:#fff
    style B fill:#0878A6,stroke:#065e91,stroke-width:2px,color:#fff
    style C fill:#334155,stroke:#64748b,stroke-width:2px,color:#fff
    style D fill:#7f1d1d,stroke:#ef4444,stroke-width:2px,color:#fff
    style E fill:#0d823c,stroke:#065f46,stroke-width:2px,color:#fff
    style I fill:#019ad8,stroke:#065e91,stroke-width:2px,color:#fff
    style F1 fill:#fbbf24,stroke:#b45309,stroke-width:2px,color:#111
    style F2 fill:#fbbf24,stroke:#b45309,stroke-width:2px,color:#111
    style G fill:#38bdf8,stroke:#065e91,stroke-width:2px,color:#111
    style H fill:#1e3a5f,stroke:#4db3d4,stroke-width:2px,color:#fff
```

*Note: The repositories highlighted below are open-source, generalized rebuilds of these exact fintech problem spaces.*

---

### 🛠️ Tech Stack & Toolkit

#### Backend & Database
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

#### Frontend & Tooling
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

#### Methodologies & Quality
![Domain-Driven Design](https://img.shields.io/badge/Domain--Driven_Design-DDD-blue?style=flat-square)
![Automated Testing](https://img.shields.io/badge/Automated_Testing-92%25_Coverage-green?style=flat-square&logo=phpunit&logoColor=white)
![Clean Architecture](https://img.shields.io/badge/Clean_Architecture-Solid-purple?style=flat-square)

---

### 📂 Featured Open-Source Projects

I extract the architectural concepts from my daily fintech tasks and rebuild them as modular, open-source packages:

#### 🏦 [cnab-toolkit](https://github.com/carlosvoliv/cnab-toolkit)
> Schema-driven PHP engine to read, write, and validate Brazilian CNAB bank files (supporting both CNAB 240 and 400 structures with strict verification).
> 
> * **Key Stacks:** PHP, OOP, Schema Validation

#### 📄 [credit-doc-extract](https://github.com/carlosvoliv/credit-doc-extract)
> A Laravel + DDD parsing system designed to ingest raw PDFs, perform rule-based structured extraction, and output clean domain objects.
> 
> * **Key Stacks:** Laravel, DDD, PDF Parsing, Test-Driven Development (TDD)

#### 🎨 [facet-ui](https://github.com/carlosvoliv/facet-ui)
> A lightweight Vue 3 design system equipped with tokens-as-data, native dark mode support, and 19+ highly customizable presets.
> 
> * **Key Stacks:** Vue 3, TypeScript, CSS Variables, TailwindCSS

---

### 📊 GitHub Activity & Stats

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=carlosvoliv&theme=tokyonight&hide_border=true" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=carlosvoliv&theme=default&hide_border=true" />
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=carlosvoliv&theme=default&hide_border=true" alt="GitHub Streak" />
  </picture>
</div>

---

### 🤖 Daily Workflow Note
I lean on AI tooling (such as Claude Code and Gemini-powered agents) as part of my daily engineering workflow. I treat it as an extension of my dev setup — not as a shortcut, but as a deliberate part of how I ship, refactor, and review high-quality code.

📫 Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/carlosvoliv/) or drop an email!
