# 00-setup: Backend Environment Setup from Zero

> **Backend Zero to Expert** · Module 00 · English + বাংলা

![Level](https://img.shields.io/badge/level-beginner-green)
![Time](https://img.shields.io/badge/time-2--3%20hours-blue)
![Language](https://img.shields.io/badge/language-English%20%7C%20বাংলা-orange)

---

## 1. Overview

### 🎯 Learning goals

**English:** By the end of this module you will be able to:

- Use the terminal for everyday tasks
- Install and configure VS Code, Node.js, Git and Postman
- Create a GitHub repository and push your first commit
- Set up MongoDB Atlas and PostgreSQL
- Run your first Node.js server

**বাংলা:** এই module শেষে তুমি পারবে:

- Terminal দিয়ে দৈনন্দিন কাজ করতে
- VS Code, Node.js, Git ও Postman install ও configure করতে
- GitHub repository বানিয়ে প্রথম commit push করতে
- MongoDB Atlas ও PostgreSQL setup করতে
- প্রথম Node.js server চালাতে

### ✅ Prerequisites

**English:** A computer (Windows, macOS or Linux), a stable internet connection and curiosity. No coding experience is required.

**বাংলা:** একটা computer (Windows, macOS বা Linux), ভালো internet connection আর শেখার আগ্রহ। আগে থেকে coding জানা লাগবে না।

---

## 2. Tools at a Glance

| Tool | Purpose | Download / Docs |
|---|---|---|
| VS Code | Code editor | [Download](https://code.visualstudio.com/) · [Docs](https://code.visualstudio.com/docs) |
| Node.js | Run JavaScript on the server | [Download](https://nodejs.org/) · [Docs](https://nodejs.org/en/learn) |
| Git | Version control | [Download](https://git-scm.com/) · [Pro Git Book](https://git-scm.com/book) |
| GitHub | Host repositories online | [Sign up](https://github.com/) · [Docs](https://docs.github.com/) |
| Postman | Test APIs | [Download](https://www.postman.com/downloads/) · [Learning Center](https://learning.postman.com/) |
| MongoDB Atlas | Cloud NoSQL database | [Sign up](https://www.mongodb.com/atlas) · [Docs](https://www.mongodb.com/docs/atlas/) |
| PostgreSQL | Relational SQL database | [Download](https://www.postgresql.org/download/) · [Docs](https://www.postgresql.org/docs/) |
| Prisma ORM | Database toolkit for Node.js | [Website](https://www.prisma.io/) · [Docs](https://www.prisma.io/docs) |

> 💡 **Note:** Prisma is installed inside a project with `npm`, so nothing to install now. We will use it in Module 06.
> Prisma project এর ভেতরে `npm` দিয়ে install হয়, তাই এখন কিছু install করতে হবে না। Module 06 এ ব্যবহার করব।

---

## 3. Terminal Basics

**English:** The terminal is a text window where you give commands to your computer. Backend developers use it every day.

- **Windows:** [PowerShell](https://learn.microsoft.com/powershell/) or [Git Bash](https://gitforwindows.org/) (installed with Git)
- **macOS:** [Terminal](https://support.apple.com/guide/terminal/welcome/mac)
- **Linux:** [Command line for beginners](https://ubuntu.com/tutorials/command-line-for-beginners)

**বাংলা:** Terminal হলো একটা text window, যেখানে command লিখে computer কে কাজ করানো হয়। Backend developer রা প্রতিদিন এটা ব্যবহার করে।

### Essential commands

| Command | Meaning | বাংলা |
|---|---|---|
| `pwd` | Show current folder | এখন কোন folder এ আছি |
| `ls` (PowerShell: `dir`) | List files | file এর list দেখাও |
| `cd folder-name` | Go into a folder | folder এ ঢোকো |
| `cd ..` | Go back one folder | এক ধাপ পেছনে যাও |
| `mkdir name` | Create a folder | নতুন folder বানাও |
| `clear` | Clean the screen | screen পরিষ্কার করো |

> 📚 **Learn more:** [The Odin Project: Command Line Basics](https://www.theodinproject.com/lessons/foundations-command-line-basics)

---

## 4. VS Code

**English:** [VS Code](https://code.visualstudio.com/) is a free, popular code editor. Download it, install it, and open it. You can also open a terminal inside it: see the [integrated terminal guide](https://code.visualstudio.com/docs/terminal/basics).

**বাংলা:** VS Code একটা free ও জনপ্রিয় code editor। Download করে install করো। VS Code এর ভেতরেই terminal খোলা যায়।

### Recommended extensions

| Extension | Why you need it |
|---|---|
| [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) | Finds mistakes in your code · কোডের ভুল ধরে |
| [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) | Formats code neatly · কোড সুন্দর করে সাজায় |
| [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) | Shows Git history inside the editor · Git history দেখায় |
| [MongoDB for VS Code](https://marketplace.visualstudio.com/items?itemName=mongodb.mongodb-vscode) | Browse your MongoDB data · database দেখার জন্য |
| [Prisma](https://marketplace.visualstudio.com/items?itemName=Prisma.prisma) | Syntax highlighting for Prisma schema · Prisma file এর জন্য |

---

## 🚧 Coming next in this module

| Part | Topics |
|---|---|
| Part 2 | Node.js, Git |
| Part 3 | GitHub and Repository, Postman |
| Part 4 | MongoDB Atlas, PostgreSQL |
| Part 5 | First Node.js server, Common errors, Practice tasks, Interview questions, Resources |