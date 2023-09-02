# Biology Data Science Project

My aim is to create a project that serves as a dynamic platform where biology students can delve into the world of coding and computing. I envision this space as a collaborative hub where individuals are excited to use programming as a means to further explore their scientific interests. To foster a sense of community and collective growth, I am committed to keeping the project as open-source and inclusive as possible, inviting contributions from anyone interested in enhancing its scope and impact. Ultimately, this initiative seeks to empower individuals to harness the capabilities of coding and computing to explore and expand their academic and personal interests.

# Lesson 1: Getting the data (Cloning the repository)

PS: if you know how to do this skip to lesson 2

Since this project is designed for people who are either new to coding or have never used types of version control such as `github`, `gitlab`, or `bitbucket`, I will be going over how to clone this repository to your computer.

## 1. Opening the terminal

The terminal is a way to interact with your computer using text commands. It is a very powerful tool that can be used to do many things. For this project we will be using it to clone the repository to your computer.

### Mac

To open the terminal on a mac, you can either search for it in spotlight by holding `⌘` and `space` and searching for `terminal` or you can go to `Applications` -> `Utilities` -> `Terminal` and click on the icon. This will open the terminal.

### Windows

To open the terminal on a windows computer, you can search for it in the search bar by clicking on the windows icon in the bottom left corner of your screen and searching for `cmd` or `command prompt`. This will open the terminal.

### Linux

To open the terminal on a linux computer, you can hold `Ctrl` and `Alt` and press `T`. This will open the terminal. If thi does not work you can right click on the desktop and click `Open in Terminal`. This will open the terminal.

## 2. Downloading git

To Clone the repository the first thing you need to do is install git. Git is a version control system that allows you to keep track of changes to your code. To install git, follow the instructions for your operating system below.

### Mac

If you do not have homebrew installed on your computer, you can install it by typing the following command into the terminal and pressing enter:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once you have homebrew installed, you can install git by typing the following command into the terminal and pressing enter:

```bash
brew install git
```

### Windows

To install git on windows, you can download the installer from [here](https://git-scm.com/download/win). Once you have downloaded the installer, you can run it and follow the instructions to install git.

### Linux

To install git on linux, you can type the following command into the terminal and press enter:

```bash
sudo apt install git
```

## 3. Cloning the repository

Now that you have git installed, you can clone the repository to your computer. To do this, type the following command into the terminal and press enter:

```bash
git clone https://github.com/MatthewEthanTam/biologyDataScienceProject.git
```

This will clone the repository to your computer. You can now move on to lesson 2.

### 🌟 If you would like to create a key to allow for cloning the repository using SSH key instead of https go to the Extra Section after the lessons 🌟

# Lesson 2: Setting up Python and Jupyter Notebook

PS: if you have python and jupyter notebook installed skip to lesson 3

Now that you have cloned the repository to your computer, you can start working on the project. The first thing you need to do is install python and jupyter notebook. To do this, follow the instructions for your operating system below.

## 1. Installing Python

### Mac

To install python on a mac, you can type the following command into the terminal and press enter:

```bash
brew install python
```

### Windows

To install python on a windows computer, you can download the installer from [here](https://www.python.org/downloads/). Once you have downloaded the installer, you can run it and follow the instructions to install python.

### Linux

To install python on a linux computer, you can type the following command into the terminal and press enter:

```bash
sudo apt install python3
```

## 2. Installing Jupyter Notebook

### Mac, Windows, and Linux

To install jupyter notebook, you can type the following command into the terminal and press enter:

```bash
pip install jupyter
```

You can now move on to lesson 3.

### 🌟If you want to learn how to setup Juypter Notebooks in VSCode go to the Extra Section🌟

# Lesson 3: creating a virtual environment

PS: if you know how to do this skip to lesson 4

A Virtual Environment is a tool to keep the dependencies required by different projects in separate places, by creating virtual Python environments for them. It solves the “Project X depends on version 1.x but, Project Y needs 4.x” dilemma, and keeps your global site-packages directory clean and manageable.

Now that you have python and jupyter notebook installed, you can create a virtual environment to install the packages you need for this project. To do this, follow the instructions for your operating system below.

## 1. Creating a virtual environment

In the termnial first navigate to the folder you cloned the repository to. To do this, type the following command into the terminal and press enter:

```bash
cd biologyDataScienceProject
```

To create a virtual environment, you can type the following command into the terminal and press enter:

```bash
python3 -m venv env
```

this will create a virtual environment called `env` in the folder you cloned the repository to. The `env` folder will contain all the packages you install for this project.

You can now move on to lesson 4.

### 🌟If you want to learn about how to not commit and push files to your git repo using .gitignore go to the Extra Section🌟

# Lesson 4: Installing the packages

PS: if you know how to do this skip to lesson 5

Now that you have created a virtual environment, you can install the packages you need for this project. To do this, follow the instructions for your operating system below.

## 1. Activating the virtual environment

To activate the virtual environment, you can type the following command into the terminal and press enter:

```bash
source env/bin/activate
```

## 2. Installing the packages

To install the packages, you can type the following command into the terminal and press enter:

```bash
pip install -r requirements.txt
```

This will install all the packages you need for this project.

## 3. Deactivating the virtual environment (When you need to)

To deactivate the virtual environment, you can type the following command into the terminal and press enter:

```bash
deactivate
```

You can now move on to lesson 5.

### 🌟If you want to learn how to install packages from scratch into an environment and create a requirements.txt file from that go to the Extra Section🌟

# Lesson 5: Adding the virtual environment to Jupyter Notebook and Opening Jupyter Notebook 

PS: if you know how to do this skip to lesson 6

Now that you have installed the packages, and created a virtual environment, you can add the virtual environment to jupyter notebook. To do this, follow the instructions for your operating system below.

## 1. Adding the virtual environment to Jupyter Notebook

To add the virtual environment to jupyter notebook, you can type the following command into the terminal and press enter:

```bash
python -m ipykernel install --user --name=env
```

## 2. Opening Jupyter Notebook

To open jupyter notebook, you can type the following command into the terminal and press enter:

```bash
jupyter notebook
```

This will open jupyter notebook in your browser. You can now move on to lesson 6 in the following folder:

```bash
src/lessons/LS06-Microbiome_ASD.ipynb
```

## 3. Opening Jupyter Notebook in a specific folder

To open jupyter notebook in a specific folder, you can type the following command into the terminal and press enter:

```bash
jupyter notebook <folder>
```

## 4. Opening Jupyter Notebook in a specific folder with a specific virtual environment

To open jupyter notebook in a specific folder with a specific virtual environment, you can type the following command into the terminal and press enter:

```bash
jupyter notebook --notebook-dir=<folder> --kernel=env
```


