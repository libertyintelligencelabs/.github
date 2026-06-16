# Liberty Intelligence Labs: House Style
**Liberty Intelligence Labs** is a modular research and development unit dedicated to building the future of secure and interconnected systems through iterative experimentation. This House Style Guide defines our standards for visual identity, file organization, and automated workflows to ensure all lab outputs maintain the cohesion, precision, and reproducibility necessary to support our work across both developmental projects and research initiatives.

## Visual Identity & Assets
We maintain a consistent visual identity to ensure our work is immediately recognizable as part of the Liberty Intelligence Labs collective. These standards apply to all public-facing and internal presentations.

| Color | Hex Code  | Purpose                 |
|-------|-----------|-------------------------|
| Red   | `#CD2726` | Titles and key emphasis |
| Black | `#2B2826` | Body text               |
| White | `#FFFFFF` | Background and contrast |

*The lab palette is designed to comply with the official brand colors of [Liberty College](https://libertycollege.edu.np/). When designing figures, slides, or infographics, use these three colors as the foundation of your work to ensure all lab outputs share a unified esthetic aligned with our institutional identity.*

| Category        | Font                                                                                                    | Usage                                 |
|-----------------|---------------------------------------------------------------------------------------------------------|---------------------------------------|
| Lab Branding    | [`Montserrat`](https://fonts.google.com/specimen/Montserrat)                                            | Logos, headlines, and UI labels       |
| Grant Proposals | [`Gentium Plus`](https://fonts.google.com/specimen/Gentium+Plus)                                        | External funding applications         |
| Presentations   | [`Inter`](https://fonts.google.com/specimen/Inter)/[`Roboto`](https://fonts.google.com/specimen/Roboto) | Slide decks, charts, and infographics |
| Documentation   | Platform-Native                                                                                         | Notion, GitHub, ACM/IEEE standards    |

***Note:** All plots and diagrams must use a white (`#FFFFFF`) background and utilize our palette for a cohesive look.*

## Naming Conventions
Apply the following case conventions to all new assets and code components to ensure easy repository navigation and to prevent merge conflicts:

| Items               | Case                   |
|---------------------|------------------------|
| Directories         | `kebab-case`           |
| Source Files        | `snake_case`           |
| Classes             | `PascalCase`           |
| Variables/Functions | `snake_case`           |
| Constants           | `SCREAMING_SNAKE_CASE` |

## Infrastructure & Automation
We use automated tooling to handle technical governance. Projects initialized from our [`project-template`](https://github.com/libertyintelligencelabs/project-template) repository are preconfigured to comply with the following industry standards:

| Category      | Tool                                                                                                                                                                |
|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Code Style    | [`Black`](https://black.readthedocs.io/en/stable/), [`Flake8`](https://flake8.pycqa.org/en/latest/), [`clang-format`](https://clang.llvm.org/docs/ClangFormat.html) |
| Formatting    | [`Prettier`](https://prettier.io/docs/)                                                                                                                             |
| Documentation | [`markdownlint`](https://github.com/markdownlint/markdownlint)                                                                                                      |
| Git History   | [`commitlint`](https://www.conventionalcommits.org/en/v1.0.0/)                                                                                                      |
| Security      | [`detect-secrets`](https://github.com/Yelp/detect-secrets)                                                                                                          |
| Environment   | [`venv`](https://docs.python.org/3/library/venv.html)                                                                                                               |

## Repository Structure
To ensure all members of the lab can independently navigate their peers' project, all repositories must adhere to the following structure:

| Path/Item    | Contents                                              |
|--------------|-------------------------------------------------------|
| `README.md`  | Project goals, setup, and external links              |
| `/docs`      | Architecture, logs, and methodology                   |
| `/src`       | Main source code and application logic                |
| `/firmware`  | Hardware-specific code and embedded configurations    |
| `/notebooks` | Jupyter notebooks and exploratory data analysis files |
| `/tests`     | Unit tests and validation scripts                     |

## Research & Language Standards
Research excellence relies on precision and consistency. All documentation and formal papers must be authored in American English, following [Merriam-Webster](https://www.merriam-webster.com/) dictionary conventions.

* **Templates:** Access the [`templates`](https://github.com/libertyintelligencelabs/templates) repository for project proposals, LaTeX files, and `references.bib`. To keep your workspace clean, do not clone the entire repository. Use the GitHub web interface to download individual files, or use `git sparse-checkout` to pull only the specific templates you need.

* **Submissions:** For papers focused on computer science or software theory, use the ACM templates. For papers focused on engineering, hardware, or applied systems, use the IEEE templates.

* **Citations:** Always use the shared `references.bib` from the `templates` repository to ensure consistency in bibliography.

## Final Implementation Notes

* If a `pre-commit` hook fails, your code is noncompliant. Review the error and address the standard.

* If you identify a structural need not covered by the provided templates, do not modify the directory structure locally. Instead, submit a proposal to the Directorate.

---
*Where intelligence meets security through disciplined experimentation.*

**Liberty Intelligence Labs: House Style | v1.0.0**

