[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![GitHub release](https://img.shields.io/github/v/release/<your-username>/CoWrite)](https://github.com/<your-username>/CoWrite/releases)
[![Contributions welcome](https://img.shields.io/badge/Contributions-welcome-lightgrey.svg)](https://github.com/<your-username>/CoWrite/issues)
![Made with Markdown](https://img.shields.io/badge/Made%20with-Markdown-lightgrey.svg)

# CoWrite

> **Note:** The file `User-Info.md` contains personal data and is excluded from version control.  
> See [Privacy & Data Use](#privacy--data-use) for details on how it’s handled.

## Overview

This system helps job seekers and professionals generate high-quality, job-tailored resumes and cover letters in collaboration with any large language model (LLM) capable of structured reasoning and multi-step task execution — such as ChatGPT, Claude, Gemini, or a locally hosted model.

The system provides structure and clarity while keeping the process collaborative. It runs entirely within the LLM chat, with no extra tooling or setup required. Use it whenever you’re preparing or updating materials for a new job application.

Full documentation is available in the [System Wiki](./wiki/Overview.md).

---

## Repository Structure

* **System-Instructions.md** – Defines the workflow logic and modular behavior used by the LLM to parse, tailor, and finalize resume materials.
* **User-Info.md** – Contains your personal details, professional experiences, and key skills. This serves as the data source for tailored content.
* **System-Documentation.md** – Explains module design, schemas, and overall system architecture.
* **README.md** – This file. Provides setup, usage, and licensing information.
* **Wiki** – Complete documentation, guidance, and examples for using and customizing the system.

---

## Setup

1. **Update your `User-Info.md` file** – This is where you’ll list your personal details, professional experiences, and key skills. The system references this file to tailor your materials accurately for each role.

2. **Create a new project or workspace** – In your LLM platform (e.g., ChatGPT Projects, Claude Workspaces), create a new project for your resume tailoring system.

3. **Upload or paste your files** – Add both **System-Instructions.md** and your **User-Info.md** to the project so the system can access them during each chat session.

4. **Start a new chat inside the project** – Whenever you want to tailor materials for a new job, open a fresh chat in that same project and paste in the full job listing to begin.

For other LLMs, simply ensure your documentation and user information are visible to the model at the start of each session.

---

## How It Works

Once setup is complete, you can begin tailoring materials for a specific job posting. The process is simple and repeatable:

1. **Start Fresh** – Open a new chat and paste in the full job listing.
2. **Parse** – The LLM analyzes the text and extracts requirements, skills, and entities.
3. **Skill Check** – The system checks your maintained Skills List for matches and gaps.
4. **Tailor** – The system drafts role-specific bullets from your Experience data.
5. **Finalize** – You review, refine, and copy finalized bullets into your resume.
6. **Additional Skills** – The LLM creates a resume-ready skills block tailored to the role.
7. **Cover Letter (optional)** – The LLM drafts a letter aligned with the company’s tone and your verified achievements.

For a detailed explanation of each module and workflow stage, visit the [System Wiki](./wiki/Overview.md).

> **Note:** As with any LLM, always review and verify the content it produces for accuracy and truthfulness. The system aims for precision, but human oversight ensures everything reflects your real experience.

---

## Privacy & Data Use

The system doesn’t store, share, or transmit any of your data. Everything stays within the active chat session.

That said, **your LLM provider likely handles data differently.** Depending on your platform (ChatGPT, Claude, Gemini, or others), your session may be logged or reviewed per their privacy policy. You are responsible for what you share.

### Local Data (User-Info.md)
CoWrite also includes a local file, `User-Info.md`, used to personalize your experience and provide context during sessions.  
This file lives entirely on your device — it is never uploaded, transmitted, or synced.  

For your protection, `User-Info.md` is excluded from version control (`.gitignore`), ensuring personal information cannot be committed or shared if you use Git or GitHub.  
A template and example version are provided so you can safely create and maintain your local copy.

---

## Feedback

If you find this system useful or have ideas for improvement, please open an issue in the repository. Feedback, bug reports, and enhancement suggestions are all welcome.

---

## License

*Current version: v1.0 – Initial public release*

This project is shared under a **Creative Commons Attribution–NonCommercial–ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.
You’re free to copy, adapt, and share it for non-commercial purposes, as long as you provide appropriate credit and license any derivative works under the same terms.

For full terms, visit [creativecommons.org/licenses/by-nc-sa/4.0](https://creativecommons.org/licenses/by-nc-sa/4.0).
