# ScriptForge v0.0.2

## Overview

ScriptForge is a Bash-based interactive tool that helps automate and streamline the reconnaissance phase of penetration testing.

Instead of manually typing long Nmap commands, ScriptForge:

* Guides you through scan configuration
* Builds optimized commands
* Saves results in a structured format
* Begins basic analysis of scan output

---

## Features (v0.0.2)

* Interactive Nmap flag selection
* Supports multiple scan types (`-sT`, `-sS`)
* Smart handling of incompatible options
* Automatic output saving using `-oA`
* Organized scan directories (`scans/<target>/<timestamp>/`)
* Extracts open ports from scan results
* Detects web services (ports 80, 443)
* Colored terminal output
* Scan summary after execution

---

## Installation

```bash
git clone https://github.com/Aetherix29/ScriptForge.git
cd ScriptForge
chmod +x script.sh
```

---

## Usage

```bash
./script.sh
```

Follow the prompts to:

* Select scan type
* Enable/disable detection options
* Configure performance settings

---

## Output Structure

After each scan:

```
scans/
└── <target>/
    └── <timestamp>/
        ├── nmap.nmap
        ├── nmap.xml
        └── nmap.gnmap
```

---

## Example Workflow

1. Enter target
2. Choose scan type
3. Configure flags
4. Run scan
5. View:

   * Open ports
   * Detected services
   * Saved results

---

## Notes

* SYN scan (`-sS`) requires root privileges
* Tool is designed for **learning + controlled environments (CTFs, labs)**
* Not responsible for misuse

---

## Roadmap

### v0.0.3

* Auto-trigger tools (e.g., Gobuster for web ports)
* Improved port parsing
* Quick scan mode

### Future

* Modular architecture
* Service-based automation
* Full recon pipeline
* Report generation

---

## Contributing

This project is currently in early development.
Suggestions, ideas, and improvements are welcome.

---

## License

MIT License

---

## Author

Built by **Aditya Singh**
Aspiring Red Teamer | Bash + Recon Enthusiast

---
