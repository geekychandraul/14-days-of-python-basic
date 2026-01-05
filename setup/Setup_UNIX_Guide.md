# 🐧 Day 0: Developer Setup Guide (Linux/Unix Edition)

Welcome to Day 0. Today we are setting up your "Command Center." Follow these steps strictly in order. It can be challenging. But I really hope these instructions are bullet-proof!

If you hit problems, please don't hesitate to reach out. I am here to get you up and running quickly. There's nothing worse than feeling _stuck_. DM me on LinkedIn message and I will unstick you quickly!

LinkedIn: https://www.linkedin.com/in/bhaskarchandraul/  

_If you're looking at this in Cursor/VS Code, please right click on the filename in the Explorer on the left, and select "Open preview", to view the formatted version._

*Note: Since there are many distributions of Linux, this guide assumes you are using **Ubuntu** or a **Debian-based** system, which is standard for beginners. If you are on Fedora or Arch, adjust the package manager commands (`dnf` or `pacman`) accordingly.*

---

## Part 1. VS Code Setup (The Editor)

We use **Visual Studio Code (VS Code)**, the industry-standard editor.

### **Installation:**

*Open your Terminal (`Ctrl + Alt + T`) and choose one method:*

**Method A: Using Snap (Recommended for Ubuntu)**

```bash
sudo snap install code --classic
```

**Method B: Using `.deb` file (Debian/Kali/Mint)**

1. **Download:** Go to [code.visualstudio.com](https://code.visualstudio.com/) and download the `.deb` file.
2. **Install:** Open terminal in your downloads folder and run:
```bash
sudo apt install ./<filename>.deb
```

### **Configuration:**

1. Open VS Code (Type `code` in terminal or find it in your menu).
2. On the left vertical bar, click the **Extensions** icon.
3. Search for **"Python"** (published by Microsoft) and click **Install**.

---

## Part 2. Python Setup (The Brain)

Linux usually comes with Python installed, but we need to ensure you have the full toolkit (pip and venv).

### **Installation:**

Open your Terminal and run this single command to update and install the necessary components:

```bash
sudo apt update && sudo apt install python3 python3-pip python3-venv -y
```

* `python3`: The language itself.
* `python3-pip`: The tool to install libraries (like pandas).
* `python3-venv`: The tool to create isolated environments.

---

## Part 3. Git Setup (The Time Machine)

Select the level that fits your comfort level. **Choose only one option.**

### **🟢 Option 1: GitHub Desktop**

*Note: GitHub Desktop does not have an official Linux version. We will use the specific Linux fork.*

1. **Download:** Go to the [Linux Fork Project](https://www.google.com/search?q=https://github.com/shiftkey/desktop/releases).
2. **Install:** Download the `.deb` file from the latest release.
3. **Run:** Right-click the file and "Open with Software Install" OR run `sudo apt install ./<filename>.deb`.
4. **Setup:** Open "GitHub Desktop" from your apps menu and sign in.

### **🟡 Option 2: VS Code Integration**

*Best if you want to manage code directly inside your editor (Highly Recommended for Linux users).*

1. **Install Git Engine:**
Open Terminal and run:
```bash
sudo apt install git -y
```

2. **Open VS Code:** Click the **Source Control** icon on the left sidebar (looks like a graph node).
3. **Action:** You can stage changes (+) and commit directly from this sidebar without typing commands.

---

## Part 4. Jupyter Notebook Setup (The Lab)

We will use "Notebooks" for our lessons.

### **Step A: Install the Extension**

1. Open VS Code.
2. Go to **Extensions**.
3. Search for **"Jupyter"** (published by Microsoft) and click **Install**.

### **Step B: Install the Backend**

1. In VS Code, open a new Terminal (`Ctrl + ~`).
2. Type the following command and press Enter:
```bash
pip3 install notebook
```

*(If you get a permission error, try adding `--user` at the end: `pip3 install notebook --user`).*

---

## ✅ Final Sanity Check

Let's verify everything is connected.

1. Open VS Code.
2. Open a New Terminal (`Ctrl + ~`).
3. Type `python --version` -> Should see `Python 3.12.x`.
4. Type `git --version` -> Should see `git version 2.x.x`.
5. Type `pip show notebook` -> Should see details about the notebook package.

**If you see all three, you are ready for next steps. Go back to README.md to complete rest of it! 🚀**