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
## 5. Node.js

**English:** [Node.js](https://nodejs.org/) lets you run JavaScript outside the browser, so you can build servers and APIs. It uses Google's V8 engine to run your code. It also installs **npm** (Node Package Manager), a tool to download and manage packages (libraries written by other developers).

**বাংলা:** Node.js দিয়ে browser এর বাইরে JavaScript চালানো যায়, তাই এটা দিয়ে server ও API বানানো সম্ভব। ভেতরে Google এর V8 engine কাজ করে। Node এর সাথে **npm** (Node Package Manager) আসে, যা দিয়ে অন্যদের লেখা package (library) download ও manage করা যায়।

### Install

1. Go to [nodejs.org/en/download](https://nodejs.org/en/download)
2. Download the version marked **LTS** (Long Term Support), not "Current"
3. Run the installer and keep all default options
4. **Close and reopen** your terminal

> 💡 **Why LTS?** LTS gets security fixes and bug fixes for a long time, so it is stable and used by companies. See the [release schedule](https://nodejs.org/en/about/previous-releases).
>
> LTS মানে বেশি দিন bug fix ও security update পাওয়া যায়, তাই এটা stable।

### Verify

```bash
node -v
npm -v
```

Both should print a version number (for example `v24.x.x`). If you see `'node' is not recognized`, restart the terminal or reinstall Node.

### Try it

```bash
node
> 2 + 3
5
> console.log("Hello")
Hello
```

Press `Ctrl + C` twice (or type `.exit`) to leave the Node shell.

### What is npm?

| Command | What it does | বাংলা |
|---|---|---|
| `npm init -y` | Create a `package.json` | project এর ID card বানায় |
| `npm install express` | Install a package | package install করে |
| `npm install -D nodemon` | Install a dev-only package | শুধু development এর package |
| `npm uninstall express` | Remove a package | package মুছে ফেলে |
| `npm run dev` | Run a script from `package.json` | script চালায় |

> 📚 **Learn more:** [Node.js official learn page](https://nodejs.org/en/learn) · [npm Docs](https://docs.npmjs.com/)
>
> 🔧 **Optional (later):** Need multiple Node versions? Use [nvm](https://github.com/nvm-sh/nvm) (macOS/Linux) or [nvm-windows](https://github.com/coreybutler/nvm-windows).

---

## 6. Git

**English:** [Git](https://git-scm.com/) is a **version control system**. It saves snapshots (called **commits**) of your project, so you can go back in time, see what changed, and work in a team without overwriting each other.

**বাংলা:** Git হলো একটা **version control system**। এটা তোমার project এর snapshot (**commit**) জমিয়ে রাখে, যাতে পুরনো অবস্থায় ফেরা যায়, কী বদলেছে দেখা যায় এবং team এ একসাথে কাজ করা যায়।

### Install

1. Go to [git-scm.com/downloads](https://git-scm.com/downloads) and download for your OS
2. Run the installer and keep the default options (on Windows this also installs **Git Bash**)
3. Reopen the terminal and verify:

```bash
git --version
```

### One-time configuration

Tell Git who you are. Use the **same email** as your GitHub account:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
```

Check it:

```bash
git config --list
```

### The mental model: 3 areas

Think of sending a parcel:

```
Working Folder  ──git add──▶  Staging Area  ──git commit──▶  Local Repo  ──git push──▶  GitHub
 (your files)                 (put in the box)               (box sealed,                 (sent online)
                                                              saved in history)
```

**বাংলা:** Parcel পাঠানোর মতো ভাবো: কাজের folder → `git add` (box এ রাখা) → `git commit` (box seal করে history তে save) → `git push` (GitHub এ পাঠানো)।

### Everyday commands

| Command | What it does | বাংলা |
|---|---|---|
| `git status` | Show what changed | কী কী বদলেছে দেখাও |
| `git add .` | Stage all changes | সব change staging এ রাখো |
| `git add file.js` | Stage one file | একটা file staging এ রাখো |
| `git commit -m "message"` | Save a snapshot | snapshot save করো |
| `git log --oneline` | Show commit history | history দেখাও |
| `git diff` | Show exact line changes | কোন line বদলেছে দেখাও |
| `git push` | Upload commits to GitHub | GitHub এ পাঠাও |
| `git pull` | Download latest changes | GitHub থেকে নতুন change আনো |
| `git clone <url>` | Copy a repository | repository copy করো |

### Branches (quick intro)

A **branch** is a separate line of work. You try new things on a branch without breaking `main`.

```bash
git branch                 # list branches
git switch -c feature-x    # create and move to a new branch
git switch main            # go back to main
git merge feature-x        # bring feature-x into main
```

**বাংলা:** Branch হলো আলাদা একটা কাজের লাইন। `main` না ভেঙে নতুন কিছু try করা যায়।

### Writing good commit messages

Use a short prefix so history stays clean (this follows [Conventional Commits](https://www.conventionalcommits.org/)):

| Prefix | Use for | Example |
|---|---|---|
| `feat:` | new feature | `feat: add login route` |
| `fix:` | bug fix | `fix: handle empty email` |
| `docs:` | documentation | `docs: add setup guide` |
| `refactor:` | code cleanup | `refactor: split user service` |

> 📚 **Learn more:**
> - [Pro Git Book (free)](https://git-scm.com/book/en/v2)
> - [Learn Git Branching (interactive game)](https://learngitbranching.js.org/)
> - [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
> - [GitHub Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)

---

## 🚧 Coming next in this module

| Part | Topics |
|---|---|
| Part 3 | GitHub and Repository, Postman |
| Part 4 | MongoDB Atlas, PostgreSQL |
| Part 5 | First Node.js server, Common errors, Practice tasks, Interview questions, Resources |