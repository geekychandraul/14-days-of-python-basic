# 🪟 Day 0: Developer Setup Guide (Windows Edition)

Welcome to Day 0. Today we are setting up your "Command Center." Follow these steps strictly in order to ensure your machine is ready for code. It can be challenging. But I really hope these instructions are bullet-proof!

If you hit problems, please don't hesitate to reach out. I am here to get you up and running quickly. There's nothing worse than feeling _stuck_. DM me on LinkedIn message and I will unstick you quickly!

LinkedIn: https://www.linkedin.com/in/bhaskarchandraul/  

_If you're looking at this in Cursor/VS Code, please right click on the filename in the Explorer on the left, and select "Open preview", to view the formatted version._

---

## Part 1. VS Code Setup (The Editor)

We don't write code in Notepad. We use **Visual Studio Code (VS Code)**, the industry-standard editor.

### **Installation:**

1. **Download:** Go to [code.visualstudio.com](https://code.visualstudio.com/) and download the "Windows" installer.
2. **Install:** Run the installer. Keep all default settings **checked**.
3. **Launch:** Open VS Code after installation.

### **Configuration:**

1. Open VS Code.
2. On the left vertical bar, click the **Extensions** icon (looks like four squares).
3. Search for **"Python"** (published by Microsoft).
4. Click **Install**.

---

## Part 2. Python Setup (The Brain)

Your computer needs to understand the Python language.

### **Installation:**

1. **Download:** Go to [python.org/downloads](https://www.python.org/downloads/).
2. Click the big button to download the latest version (e.g., Python 3.12.x).
3. **⚠️ CRITICAL STEP:** When the installer opens, look at the bottom. **Check the box that says "Add python.exe to PATH".**
* *If you miss this step, Python will not work.*


4. Click **"Install Now"**.

---

## Part 3. **Git Installation (The Time Machine)**

Select the level that fits your comfort level. **Choose only one option.**

#### **🟢 Option 1: GitHub Desktop**

*Best if you want a visual app with buttons and no commands.*

1. **Download:** Go to [desktop.github.com](https://desktop.github.com/).
2. **Install:** Run the installer.
3. **Setup:** Open the app and sign in with your GitHub account.
4. **Action:** You will use this app to "Clone", "Commit", and "Push" your code.

#### **🟡 Option 2: VS Code Integration**

*Best if you want to manage code directly inside your editor / terminal.*

1. **Install Git Engine:** Download and install "Git for Windows" from [git-scm.com/download/win](https://git-scm.com/download/win). (Click "Next" through all options).
2. **Open VS Code:** Click the **Source Control** icon on the left sidebar (looks like a graph node).
3. **Action:** You can stage changes (+) and commit directly from this sidebar without typing commands.

---

## Part 4. Jupyter Notebook Setup (The Lab)

We will use "Notebooks" for our lessons. This allows us to run code one block at a time.

### **Step A: Install the Extension**

1. Open VS Code.
2. Go to **Extensions** (on the left sidebar).
3. Search for **"Jupyter"** (published by Microsoft).
4. Click **Install**.

### **Step B: Install the Backend**

1. In VS Code, open a new Terminal (`Ctrl + ~`).
2. Type the following command and press Enter:
```bash
pip install notebook
```

*This downloads the engine that powers the notebooks.*

---

## ✅ Final Sanity Check

Let's verify everything is connected.

1. Open VS Code.
2. Open a New Terminal (`Ctrl + ~`).
3. Type `python --version` -> Should see `Python 3.12.x`.
4. Type `git --version` -> Should see `git version 2.x.x`.
5. Type `pip show notebook` -> Should see details about the notebook package.

**If you see all three, you are ready for next steps. Go back to README.md to complete rest of it! 🚀**