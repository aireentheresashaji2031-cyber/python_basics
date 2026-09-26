# Frequently Asked Questions (FAQ)

**Q1: Which version of Python should I install?**
A: You should install the latest stable release of **Python 3**. Python 2 is no longer supported or maintained.

**Q2: Do I need to pay for Python?**
A: No. Python is free and open-source software, available for download at [python.org](https://www.python.org/downloads/).

**Q3: What is the difference between `python` and `python3` commands?**
A: On many macOS and Linux systems, `python` may point to an older version or may not exist at all, while `python3` explicitly refers to Python 3. It is safest to use `python3` and `pip3` unless you have confirmed which version `python` refers to on your system.

**Q4: What is pip, and do I need to install it separately?**
A: `pip` is Python's package manager, used to install additional libraries. It is included automatically with Python 3.4 and later, so no separate installation is usually needed.

**Q5: Can I have multiple versions of Python installed at once?**
A: Yes. Multiple versions can coexist on the same system. Tools like **pyenv** (macOS/Linux) or the **Python Launcher** (Windows) help manage and switch between versions.

**Q6: What is a virtual environment, and why should I use one?**
A: A virtual environment is an isolated workspace for a Python project, keeping its dependencies separate from other projects. It is created using:
```bash
python3 -m venv myenv
```
This helps avoid conflicts between different projects' package requirements.

**Q7: I installed Python, but my terminal still doesn't recognize it. What should I do?**
A: This usually means Python was not added to your system's PATH. Refer to the **Troubleshooting** section in `Installation.md` for step-by-step instructions to fix this.

**Q8: How do I update Python to a newer version?**
A: Download the latest installer from the official website and run it. On Windows and macOS, the installer will typically upgrade the existing installation. On Linux, use your package manager (e.g., `apt`, `dnf`) to update.

**Q9: How do I uninstall Python?**
A:
- **Windows:** Go to *Settings > Apps > Installed Apps*, find Python, and click Uninstall.
- **macOS:** Remove the Python framework folder from `/Library/Frameworks/Python.framework` (advanced users only) or use Homebrew: `brew uninstall python3`.
- **Linux:** Use `sudo apt remove python3` (not usually recommended, as many system tools depend on Python).

**Q10: Where can I learn Python after installing it?**
A: The official Python documentation ([docs.python.org](https://docs.python.org/3/)) is an excellent starting point, along with tutorials on platforms like W3Schools, Codecademy, and Real Python.
