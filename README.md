# ScriptForge
# Recon Tool (v0.0.1)

A simple interactive wrapper around Nmap that lets you build scans step-by-step instead of memorizing flags.

---

## Function

Nmap is insanely powerful, but remembering what every flag does (and which ones don’t work together) is annoying—especially when you're still learning or just want to move fast.

This tool asks you straightforward questions and builds the command for you, while making sure you don’t accidentally combine things that don’t make sense.

---

## ⚙️ What it does (so far)

* Walks you through scan setup using prompts
* Lets you choose scan types like `-sT` or `-sS` without conflict
* Optionally enables things like:

  * service detection (`-sV`)
  * OS detection (`-O`)
  * aggressive scan (`-A`)
* Supports timing templates and rate control
* Shows you the final command before running it

---

## Usage

```bash
chmod +x ScriptForge
./ScriptForge
```

Answer the questions, review the generated command, and run it if you're happy with it.

---

## Where this is going

Right now it’s just a smarter way to run Nmap.

The goal is to turn it into a full recon workflow, where:

* Nmap results are saved and parsed
* Services are detected automatically
* Other tools (like directory brute-forcing, service enumeration, etc.) run based on what’s found

Basically: from manual scanning → semi-automated recon.

---

## Note

Use this only on systems you own or have permission to test.

---

## License

MIT License

---

## Author

Aditya Pratap Singh

