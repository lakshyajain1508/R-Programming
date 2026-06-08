# Complete R Setup Guide

## Introduction

This guide will help you install and configure everything required to learn R Programming using:

* R
* VS Code
* Jupyter Notebook
* IRKernel
* Environment Variables (PATH)

After completing this setup, you will be able to run R code from:

* Command Prompt
* PowerShell
* VS Code
* Jupyter Notebook

---

# Step 1: Install R

Visit:

```text
https://cran.r-project.org
```

Download the latest version of R for your operating system.

Complete the installation using the default settings.

---

# Step 2: Find Your R Installation Path

After installation, R is usually located at:

### Windows

```text
C:\Program Files\R\R-4.x.x\
```

Example:

```text
C:\Program Files\R\R-4.5.1\
```

Inside this folder you will find:

```text
bin
```

Example:

```text
C:\Program Files\R\R-4.5.1\bin
```

And:

```text
C:\Program Files\R\R-4.5.1\bin\x64
```

This is the folder we need to add to the system PATH.

---

# Step 3: Add R to Environment Variables

## Method (Windows)

Press:

```text
Windows + S
```

Search:

```text
Edit the system environment variables
```

Open it.

---

Click:

```text
Environment Variables
```

---

Under:

```text
System Variables
```

Find:

```text
Path
```

Select it.

Click:

```text
Edit
```

---

Click:

```text
New
```

Add:

```text
C:\Program Files\R\R-4.5.1\bin
```

and

```text
C:\Program Files\R\R-4.5.1\bin\x64
```

Use your installed version if different.

---

Click:

```text
OK
```

Save all windows.

---

# Step 4: Verify PATH Configuration

Close all terminals.

Open a new Command Prompt.

Run:

```bash
R --version
```

Expected output:

```text
R version 4.x.x
```

If you see the version number, PATH is configured correctly.

---

# Step 5: Install VS Code

Download:

```text
https://code.visualstudio.com
```

Install normally.

---

# Step 6: Install Python

Jupyter requires Python.

Download:

```text
https://www.python.org/downloads/
```

During installation:

✅ Check

```text
Add Python to PATH
```

before clicking Install.

---

# Step 7: Verify Python Installation

Open Command Prompt.

Run:

```bash
python --version
```

Example:

```text
Python 3.13.0
```

Also verify:

```bash
pip --version
```

Example:

```text
pip 25.x.x
```

---

# Step 8: Install Jupyter Notebook

Run:

```bash
pip install notebook
```

Verify:

```bash
jupyter --version
```

---

# Step 9: Install VS Code Extensions

Open VS Code.

Go to:

```text
Extensions
```

Install:

### R Extension

```text
R
```

Publisher:

```text
REditorSupport
```

---

### Jupyter Extension

```text
Jupyter
```

Publisher:

```text
Microsoft
```

---

### Python Extension

```text
Python
```

Publisher:

```text
Microsoft
```

---

# Step 10: Install IRKernel

Open R.

Run:

```r
install.packages("IRkernel")
```

Wait for installation.

---

# Step 11: Register R Kernel

Still inside R:

```r
IRkernel::installspec()
```

Expected:

```text
Installed kernelspec ir
```

Now Jupyter can execute R notebooks.

---

# Step 12: Test R from Command Prompt

Run:

```bash
R
```

You should enter the R Console.

Example:

```r
print("Hello")
```

Output:

```text
[1] "Hello"
```

Exit:

```r
q()
```

---

# Step 13: Run R Script from Terminal

Create:

```text
hello.R
```

Add:

```r
print("Hello R")
```

Run:

```bash
Rscript hello.R
```

Output:

```text
[1] "Hello R"
```

---

# Step 14: Configure R Path in VS Code

Open VS Code.

Press:

```text
Ctrl + Shift + P
```

Search:

```text
Preferences: Open User Settings (JSON)
```

Add:

```json
{
    "r.rterm.windows": "C:\\Program Files\\R\\R-4.5.1\\bin\\x64\\R.exe"
}
```

Replace the version number if necessary.

Save the file.

Restart VS Code.

---

# Step 15: Test R in VS Code

Create:

```text
test.R
```

Write:

```r
print("VS Code is Ready")
```

Run:

```text
Ctrl + Enter
```

Output:

```text
[1] "VS Code is Ready"
```

---

# Step 16: Create R Notebook in VS Code

Create:

```text
example.ipynb
```

Select Kernel:

```text
R
```

Add:

```r
print("Notebook Working")
```

Run:

```text
Shift + Enter
```

Output:

```text
[1] "Notebook Working"
```

---

# Common PATH Errors

## Error

```text
'R' is not recognized as an internal or external command
```

Cause:

R is not added to PATH.

Solution:

Recheck:

```text
Environment Variables → Path
```

Ensure:

```text
C:\Program Files\R\R-4.5.1\bin
```

exists.

---

## Error

```text
'python' is not recognized
```

Cause:

Python PATH missing.

Solution:

Reinstall Python and enable:

```text
Add Python to PATH
```

---

## Error

```text
No Kernel Found
```

Cause:

IRKernel not installed.

Solution:

```r
install.packages("IRkernel")
IRkernel::installspec()
```

---

# Recommended Development Setup

For this tutorial repository, use:

```text
R
+
VS Code
+
Python
+
Jupyter Extension
+
IRKernel
```

Benefits:

✔ Modern Interface

✔ Notebook Support

✔ Professional Workflow

✔ Data Visualization

✔ Easy Package Management

✔ Cross Platform

---

# Final Verification Checklist

```text
✓ R Installed

✓ R Added to PATH

✓ Python Installed

✓ Python Added to PATH

✓ VS Code Installed

✓ R Extension Installed

✓ Jupyter Extension Installed

✓ IRKernel Installed

✓ R Kernel Registered

✓ R Scripts Running

✓ R Notebooks Running
