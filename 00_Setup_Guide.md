Before starting Day 01, make sure you have your environment ready:

### ✅ Before You Begin
Make sure you’ve completed the setup instructions for your system:
- For Windows users check out [Windows_Setup_Guide](setup/Setup_Windows_Guide.md)
- For Mac users checkout [Mac_Setup_Guide](setup/Setup_MAC_Guide.md)
- For UNIX users checkout [UNIX_Setup_Guide](setup/Setup_UNIX_Guide.md)

Also, be sure to launch this Jupyter Lab **from the root directory of the project**, with your virtual environment **properly activated**. This helps all the magic work smoothly behind the scenes. ✨

### Setps to setup virtual env:
1. **Open Terminal in VS code:**

Select View >> Terminal, to see a Terminal window within VS Code.  

2. **Navigate to your projects folder:**

If you have a specific folder for projects, navigate to it using the cd command. For example:  
`cd C:\Users\YourUsername\projects`  
Replacing YourUsername with your actual Windows user

If you don't have a projects folder, you can create one:
```
mkdir C:\Users\YourUsername\projects
cd C:\Users\YourUsername\projects
```

3. **Clone the repository:**

Enter this in the command prompt in the Projects folder:

`git clone https://github.com/geekychandraul/14-Days-of-Python-Basics.git`

This creates a new directory `14-Days-of-Python-Basics` within your Projects folder and downloads the code for the class. This `14-Days-of-Python-Basics` directory is known as the "project root directory". 

4. **Change Directory to Project Root Directory**
    ```sh
   cd 14-Days-of-Python-Basics
   ```
5. **Creating Virtual Env:**  
  ```sh
   python -m venv .venv
   ```
6. **Activating Virtual Env:**  
  ```sh
   source .venv/bin/activate
   ```

---

## If you're new to the Command Line

Please checkout this awesome guide from our AI friend [Command Line Guide](guides/02_command_line.ipynb).

---

## If you're new to the GIT 

Please checkout this detailed guide [GIT & GitHub Guide](guides/03_git_and_github.ipynb).

---

## 👋 New to JupyterLab?

Welcome to the wonderful world of **data science experimentation**! Once you start using JupyterLab, you’ll wonder how you ever worked without it.

Here are a few quick tips to get started:

* **Run a Cell**: Click inside any code cell and press `Shift + Return` or `Ctrl + Return` to execute it.
* **Add a New Cell**: Click the **`+`** button in the toolbar or press `Alt + Return` to insert a new cell below.

To help you get more comfortable, I’ve created a notebook titled [**Guide to Jupyter**](guides/04_guide_to_jupyter.ipynb). It covers essentials like:

* Writing **Markdown comments**
* Using **`!` commands** to run shell commands from within cells
* Leveraging **`tqdm`** to display progress bars in loops

Dive in and start experimenting — JupyterLab is an incredibly powerful and flexible tool for learning, prototyping, and exploring ideas.