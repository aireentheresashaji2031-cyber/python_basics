# Installation Steps

Follow the steps below based on your operating system.

## Windows

1. Go to the official Python website: [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Click **Download Python 3.x.x** (the latest version shown).
3. Run the downloaded `.exe` installer.
4. **Important:** On the first installer screen, check the box labeled **"Add Python to PATH"** before proceeding.
5. Click **Install Now** and wait for the installation to complete.
6. Once finished, click **Close**.

## macOS

1. Go to [https://www.python.org/downloads/](https://www.python.org/downloads/) and download the macOS installer (`.pkg` file).
2. Open the downloaded `.pkg` file.
3. Follow the on-screen installer instructions, agreeing to the license terms.
4. Enter your administrator password when prompted.
5. Wait for the installation to complete, then close the installer.

Alternatively, if you use **Homebrew**, you can install Python via terminal:

```bash
brew install python3
```

## Linux (Debian/Ubuntu-based)

Most Linux distributions come with Python pre-installed. To install or update it manually:

```bash
sudo apt update
sudo apt install python3 python3-pip -y
```

For Fedora-based systems:

```bash
sudo dnf install python3 python3-pip -y
```

---

# Verification Steps

After installation, verify that Python was installed correctly.

## Step 1: Open a Terminal or Command Prompt

- **Windows:** Open Command Prompt or PowerShell
- **macOS/Linux:** Open Terminal

## Step 2: Check the Python Version

Run the following command:

```bash
python --version
```

or, on some systems (especially macOS/Linux):

```bash
python3 --version
```

You should see output similar to:

```
Python 3.12.4
```

## Step 3: Check pip (Python Package Installer)

Python installations include `pip` by default. Verify it with:

```bash
pip --version
```

or

```bash
pip3 --version
```

## Step 4: Run a Test Script

Create a simple test to confirm Python runs correctly:

```bash
python -c "print('Python installed successfully!')"
```

If the message prints without errors, your installation is complete and working.

---

# Troubleshooting

## Issue 1: `'python' is not recognized as an internal or external command` (Windows)

**Cause:** Python was not added to the system PATH during installation.

**Solution:**
1. Reinstall Python and ensure **"Add Python to PATH"** is checked.
2. Or manually add Python to PATH:
   - Search **"Environment Variables"** in Windows Settings.
   - Edit the **Path** variable and add the folder where Python is installed (e.g., `C:\Users\<YourName>\AppData\Local\Programs\Python\Python312\`).

## Issue 2: `command not found: python` (macOS/Linux)

**Cause:** The system uses `python3` instead of `python` as the command name.

**Solution:** Use `python3` and `pip3` instead of `python` and `pip`, or create an alias:

```bash
alias python=python3
```

## Issue 3: Permission Denied Errors (macOS/Linux)

**Cause:** Insufficient privileges to install packages or software.

**Solution:** Use `sudo` for system-wide installations, or better, use a **virtual environment** to avoid permission issues:

```bash
python3 -m venv myenv
source myenv/bin/activate
```

## Issue 4: Multiple Python Versions Conflict

**Cause:** Older versions of Python installed alongside the new version cause conflicts.

**Solution:**
- Use `python3 --version` to confirm which version runs by default.
- Use version managers like **pyenv** to manage multiple Python versions cleanly.

## Issue 5: Installer Fails to Download or Run

**Solution:**
- Check your internet connection.
- Ensure you downloaded the installer for the correct operating system and architecture (32-bit vs 64-bit).
- Temporarily disable antivirus software that may block the installer, then re-enable it after installation.

---

# Conclusion

Installing Python is a straightforward process once the correct steps are followed for your operating system. This guide covered the software requirements, step-by-step installation instructions for Windows, macOS, and Linux, verification steps to confirm a successful setup, and solutions to common installation issues.

With Python successfully installed and verified, you are now ready to start writing and running Python programs. For further learning, consider exploring the official Python documentation at [https://docs.python.org/3/](https://docs.python.org/3/) or setting up a code editor such as VS Code to begin coding.
