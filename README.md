# 🚀 BuildMatrix

> **Transform raw Jenkins build history into enterprise-ready Build & Release reports in minutes.**

BuildMatrix is a browser-based DevOps productivity tool that automates the generation of monthly Build & Release Reports from Jenkins build history.

Instead of manually reviewing hundreds of Jenkins builds across multiple servers and environments, simply paste the copied build history, map each job once, and let BuildMatrix generate a structured deployment matrix and Excel report in seconds.

---

# ✨ Features

* 📋 Paste raw Jenkins build history directly from the Jenkins UI
* ⚡ Automatically parse job names, build numbers, timestamps, and statuses
* ✅ Correctly classify successful builds

  * **Stable**
  * **Back to Normal**
* ❌ Track unsuccessful builds separately

  * Broken
  * Aborted
  * Failed
  * Unknown/Unclassified
* 🗂 Persistent project mapping using browser storage
* 🏗 Support for multi-module projects
* 📊 Automatic Build Matrix generation
* 📄 Export to Excel (`.xlsx`)
* 📁 Includes Raw Records and Summary sheets
* 🌐 Runs entirely in the browser
* 🔒 No backend or database required

---

# 📈 Problem Statement

Managing Build & Release reports manually is repetitive, time-consuming, and prone to human error.

A typical monthly workflow involved:

* Opening multiple Jenkins servers
* Copying build history
* Identifying projects
* Determining deployment environments
* Counting successful deployments
* Filling an Excel dashboard manually

Across **46+ enterprise projects**, this process could take several hours every month.

BuildMatrix reduces this to just a few minutes.

---

# 🏛 How It Works

```
Jenkins Build History
          │
          ▼
Copy Build History
          │
          ▼
Paste into BuildMatrix
          │
          ▼
Auto Parse
(Job • Build • Status)
          │
          ▼
Project Mapping
(One-time setup)
          │
          ▼
Environment Detection
          │
          ▼
Build Matrix Generation
          │
          ▼
Excel Dashboard Export
```

---

# ✅ Build Classification Logic

Only the following statuses are considered **Successful Builds**:

* Stable
* Back to Normal

These builds are included in the deployment matrix.

All other statuses are considered unsuccessful and are only counted in the summary.

Examples include:

* Broken
* Aborted
* Failed
* Unknown

---

# 📊 Output

BuildMatrix generates an Excel report containing:

### Dashboard

| Project | Dev | Test | Stg | Prod | Audit | UAT | Total |
| ------- | --: | ---: | --: | ---: | ----: | --: | ----: |

---

### Summary

* Total Successful Builds
* Total Unsuccessful Builds
* Failed Builds
* Aborted Builds
* Unknown Status Builds

---

### Raw Records

Every parsed Jenkins record is preserved for auditing and verification.

---

# 🏗 Multi-Module Project Support

Projects containing multiple Jenkins jobs are automatically grouped.

Example:

```
CSM Africa
├── Admin API
├── Frontend Admin
└── Website
```

The dashboard displays:

* Parent project total
* Individual module breakdown
* Combined deployment count

Single-module projects remain as a single row.

---

# 💾 Persistent Mapping

The first time a Jenkins job appears, BuildMatrix asks for:

* Project
* Module
* Environment

The mapping is stored locally in the browser.

Future reports automatically recognize previously mapped jobs.

---

# 🛠 Tech Stack

* Vanilla JavaScript (ES6)
* HTML5
* CSS3
* SheetJS (Excel Export)
* LocalStorage
* Browser APIs

No frameworks.

No backend.

No database.

No installation required.

---

# 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/yourusername/buildmatrix.git
```

Navigate to the project:

```bash
cd buildmatrix
```

Open:

```
index.html
```

or host it using any static web server.

---

# 📋 Usage

### Step 1

Open Jenkins.

---

### Step 2

Copy the Build History.

---

### Step 3

Paste it into BuildMatrix.

---

### Step 4

Review or update project mappings (only required once).

---

### Step 5

Generate the Build Matrix.

---

### Step 6

Export the Excel report.

Done.

---

# 🎯 Use Cases

* DevOps Teams
* Release Engineers
* Build Engineers
* CI/CD Reporting
* Deployment Tracking
* Enterprise Build Audits
* Monthly Release Reports

---

# 📷 Screenshots

Add screenshots such as:

* Home Screen
* Mapping Screen
* Generated Matrix
* Excel Export
* Summary Dashboard

---

# 🔮 Future Enhancements

* Jenkins API integration
* Authentication support
* CSV import
* PDF report generation
* Build trend analytics
* Deployment charts
* Release history
* GitLab CI support
* GitHub Actions support
* Azure DevOps support
* TeamCity support
* Bamboo support

---

# 🤝 Contributing

Contributions, suggestions, and feature requests are welcome.

Feel free to open an issue or submit a pull request.

---

# 📄 Screenshots

<img width="955" height="346" alt="Home" src="https://github.com/user-attachments/assets/b6638037-3937-4158-a52d-90abc3c71336" />


---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

It helps others discover the project and motivates further improvements.

---

## 👨‍💻 Author

**Shohail Parwej**

DevOps • CI/CD • Cloud • Linux • Automation

Passionate about building practical tools that eliminate repetitive engineering work and improve developer productivity.



