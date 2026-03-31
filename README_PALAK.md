# The Open Source Audit — OSS Capstone Project

**Student:** Palak Rai
**Registration No.:** 24BCE10391
**Course:** Open Source Software (NGMC) | Units 1–5
**Slot:** F11
**Submission Date:** 31 March 2026
**Maximum Marks:** 100

---

## Overview

This repository contains the capstone project for the Open Source Software course at VITyarthi. The project is a structured, multi-part audit of **Git** — the world's most widely adopted distributed version control system — examined through both philosophical and technical lenses.

The audit investigates Git's origins, its GNU GPL v2 licence, its ethical significance, its Linux system footprint, its place in the FOSS ecosystem, and its standing relative to proprietary alternatives. Five original Bash shell scripts are also included as part of the technical demonstration.

---

## Repository Structure

```
.
├── README.md                        # This file
├── PalakRai_OSSCapstone.docx        # Full project report (12+ pages)
└── scripts/
    ├── script1_system_identity.sh   # System Identity Reporter
    ├── script2_foss_inspector.sh    # FOSS Package Inspector
    ├── script3_disk_auditor.sh      # Disk and Permission Auditor
    ├── script4_log_analyser.sh      # Log File Analyser
    └── script5_manifesto_gen.sh     # Open Source Manifesto Generator
```

---

## Project Structure

The report is divided into the following major sections:

| Section | Title |
|---------|-------|
| 1 | Introduction — The Open Source Paradigm |
| 2 | Part A — Origin and Philosophy |
| 3 | Part B — Linux System Footprint |
| 4 | Part C — The FOSS Ecosystem |
| 5 | Part D — Open Source vs. Proprietary Analysis |
| 6 | Technical Audit — Shell Script Tasks |
| 7 | Conclusion and References |

---

## Software Under Audit

**Git** — Distributed Version Control System
- **Licence:** GNU General Public License v2 (GPL v2)
- **Original Author:** Linus Torvalds (April 2005)
- **Current Maintainer:** Junio Hamano
- **Official Site:** https://git-scm.com
- **Source Repository:** https://github.com/git/git

---

## Audit Environment

| Property | Value |
|----------|-------|
| OS | Ubuntu 24.04.3 LTS |
| Platform | WSL2 (Windows Subsystem for Linux 2) |
| Package Manager | APT (Advanced Package Tool) |
| Install Command | `sudo apt install git -y` |
| Version Check | `git --version` |

---

## Shell Scripts — Quick Reference

### Script 1: System Identity Reporter
Displays a formatted system identity card using live kernel data.
```bash
bash script1_system_identity.sh
```
**Concepts:** Variables, `echo`, command substitution `$(…)`

---

### Script 2: FOSS Package Inspector
Checks if Git is installed and prints its philosophical significance.
```bash
bash script2_foss_inspector.sh
```
**Concepts:** `if-then-else`, `case` statements, `dpkg`, `grep`

---

### Script 3: Disk and Permission Auditor
Audits critical Linux directories for permissions and disk usage.
```bash
bash script3_disk_auditor.sh
```
**Concepts:** `for` loops, `[ -d ]` directory checks, `awk`, `cut`, `du`, `ls`

---

### Script 4: Log File Analyser
Counts occurrences of a keyword (e.g. "error") in a log file.
```bash
bash script4_log_analyser.sh /var/log/syslog error
```
**Concepts:** `while read` loops, counter arithmetic `$(( … ))`, positional arguments `$1 $2`

---

### Script 5: Open Source Manifesto Generator
Interactively generates a personalised FOSS manifesto and saves it to a `.txt` file.
```bash
bash script5_manifesto_gen.sh
```
**Concepts:** `read` prompts, string concatenation, output redirection `>`

---

## Key Findings

- Git was created in **April 2005** in direct response to the revocation of the Linux kernel community's free access to the proprietary BitKeeper tool.
- The **GNU GPL v2** licence grants four core freedoms: to run, study, redistribute, and improve the software — and mandates that these freedoms are preserved in all derivative works (copyleft).
- Git's filesystem presence follows the Linux **FHS** standard: binary at `/usr/bin/git`, system config at `/etc/gitconfig`, user config at `~/.gitconfig`.
- Git operates under the **Principle of Least Privilege** — it requires no root access for standard operations.
- Compared against **Perforce Helix Core**, Git is superior in cost, freedom, governance, and community support for the vast majority of development contexts.

---

## Comparison Summary: Git vs. Perforce

| Dimension | Git (Open Source) | Perforce Helix Core (Proprietary) |
|-----------|-------------------|-----------------------------------|
| Cost | Free | Per-user subscription |
| Source Access | Fully open | Closed / black box |
| Support | Community-driven | Corporate SLA |
| Freedom | Absolute (GPL v2) | None |
| Governance | Community meritocracy | Single corporate entity |

---

## References

1. Chacon, S. & Straub, B. (2014). *Pro Git* (2nd ed.). Apress. https://git-scm.com/book
2. Free Software Foundation. (1991). *GNU General Public License, Version 2.* https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
3. Torvalds, L. (2005). Initial Git commit message. Linux Kernel Mailing List. https://lkml.org/lkml/2005/4/6/121
4. Raymond, E.S. (1999). *The Cathedral and the Bazaar.* O'Reilly Media.
5. Stallman, R.M. (2002). *Free Software, Free Society.* GNU Press.
6. Open Source Initiative. (2023). *The Open Source Definition.* https://opensource.org/osd
7. Git Project. (2024). *Git Reference Manual.* https://git-scm.com/docs
8. Canonical Ltd. (2024). *Ubuntu 24.04 LTS Documentation.* https://ubuntu.com/server/docs

---

## Licence

This academic report and associated scripts are submitted for evaluation under the VITyarthi OSS course. All audited software (Git) is licenced under the **GNU General Public License v2**.

---

*Palak Rai — 24BCE10391 — VITyarthi | Open Source Software*
