[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![GitHub release](https://img.shields.io/github/v/release/matthewjgordon/CoWrite)](https://github.com/matthewjgordon/CoWrite/releases)
[![Contributions welcome](https://img.shields.io/badge/Contributions-welcome-lightgrey.svg)](https://github.com/matthewjgordon/CoWrite/issues)
![Made with Markdown](https://img.shields.io/badge/Made%20with-Markdown-lightgrey.svg)

# CoWrite

## Overview

CoWrite helps job seekers and professionals generate high-quality, job-tailored resumes and cover letters in collaboration with any large language model (LLM) that can handle structured reasoning and multi-step tasks. Examples include ChatGPT, Claude, Gemini, or a locally hosted model.

The system provides structure and clarity while keeping the process collaborative. It runs entirely inside the LLM chat. No extra tooling required. Use it whenever you are preparing or updating materials for a new job application.

📘 Full documentation and usage examples are in the **[CoWrite Wiki](https://github.com/matthewjgordon/CoWrite/wiki)**.

---

## Installation

You can access CoWrite in two ways.

* **Clone the repository**

  ```bash
  git clone https://github.com/matthewjgordon/CoWrite.git
  cd CoWrite
  ```

* **Or download as a ZIP**
  Click **Code → Download ZIP**, then extract the files locally.

---

## Setup

1. **Update your `User-Info.md` file**
   This file holds your personal details, professional experiences, and key skills. The system reads it to tailor materials for each role.

   > **Note:** The file `User-Info.md` contains personal data and is excluded from version control.
   > See [Privacy & Data Use](#privacy--data-use) for details.

2. **Create a new project or workspace**
   In your LLM platform (for example ChatGPT Projects or Claude Workspaces), create a project for CoWrite.

3. **Upload or paste your files**
   Add **System-Instructions.md** and your **User-Info.md** so the model can access them during each chat session.

4. **Start a new chat in that project**
   When you want to tailor materials for a new job, open a fresh chat and paste the full job listing to begin.

For other LLMs, make sure the documentation and user info are visible to the model at the start of each session.

---

## How It Works

Once setup is complete, tailoring for a specific posting is simple and repeatable.

1. **Start fresh** – Open a new chat and paste the full job listing.
2. **Parse** – The LLM analyzes the text and extracts requirements, skills, and entities.
3. **Skill check** – The system checks your Skills List for matches and gaps.
4. **Tailor** – The system drafts role-specific bullets from your Experience data.
5. **Finalize** – You review, refine, and copy finalized bullets into your resume.
6. **Additional skills** – The model creates a resume-ready skills block for the role.
7. **Cover letter (optional)** – The model drafts a letter aligned with the company’s tone and your verified achievements.

See the **[CoWrite Wiki](https://github.com/matthewjgordon/CoWrite/wiki)** for details on each stage.

> **Note:** Always review and verify model output for accuracy and truthfulness. Human oversight ensures everything reflects your real experience.

---

## Repository Structure

* **System-Instructions.md** – Workflow logic and modular behavior the LLM uses to parse, tailor, and finalize materials.
* **User-Info.md** – Your personal details, professional experiences, and key skills. Serves as the data source for tailored content.
* **System-Documentation.md** – Module design, schemas, and system architecture.
* **README.md** – This file. Setup, usage, and licensing information.
* **Wiki** – Complete documentation, guidance, and examples.

---

## Privacy & Data Use

The system does not store, share, or transmit your data. Everything stays within the active chat session.

That said, **your LLM provider may handle data differently**. Depending on your platform (ChatGPT, Claude, Gemini, or others), your session may be logged or reviewed per their privacy policy. You are responsible for what you share.

### Local Data (User-Info.md)

`User-Info.md` personalizes your experience and provides context during sessions.
This file lives on your device. It is never uploaded, transmitted, or synced by CoWrite.

For your protection, `User-Info.md` is excluded from version control (`.gitignore`). This prevents personal information from being committed or shared when using Git or GitHub. A template and an example are included so you can create and maintain your local copy safely.

---

## Feedback

If you find CoWrite useful or have ideas for improvement, please open an issue. Bug reports and enhancement suggestions are welcome.
Use the structured issue templates to keep feedback consistent.

---

## License

This project is licensed under **Creative Commons Attribution–NonCommercial–ShareAlike 4.0 International (CC BY-NC-SA 4.0)**.
You may copy, adapt, and share it for non-commercial purposes, with attribution and the same license on derivatives.

Full terms: [https://creativecommons.org/licenses/by-nc-sa/4.0](https://creativecommons.org/licenses/by-nc-sa/4.0)

For release history, see the **[Changelog](./CHANGELOG.md)**.
