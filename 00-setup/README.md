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

## 7. GitHub and Repository

**English:** [GitHub](https://github.com/) is a website that stores your Git repositories online. It is your public portfolio, your backup, and the place where teams collaborate. Recruiters often check it.

**বাংলা:** GitHub এমন একটা website যেখানে তোমার Git repository online এ থাকে। এটা তোমার portfolio, backup, আর team এর কাজের জায়গা। Recruiter রা প্রায়ই GitHub profile দেখে।

### Step 1: Create an account

Sign up at [github.com/signup](https://github.com/signup). Choose a **professional username** (your real name works best), because it appears in your profile link.

### Step 2: Create a repository

1. Click **+** (top right) → **New repository**
2. Fill **Repository name** and **Description**
3. Choose **Public** (so others can learn from it)
4. Turn on **Add README**, choose **Node** for `.gitignore`, and choose **MIT License**
5. Click **Create repository**

### Step 3: Clone it to your computer

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
code .
```

**বাংলা:** Repository এর page এ সবুজ **Code** button চেপে HTTPS URL copy করো, তারপর `git clone` দাও।

### Step 4: The daily workflow

```bash
# 1. make changes in your files, then:
git status
git add .
git commit -m "docs: describe what you changed"
git push
```

The first `git push` opens a browser window to log in to GitHub. Log in once and Git remembers you.

> 🔐 **Authentication options**
> - **HTTPS + browser login** (default, easiest for beginners)
> - **SSH keys** (optional, more convenient later): [GitHub SSH guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
> - **Personal Access Token** if a password is asked: [Creating a token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)
>
> GitHub এ এখন account password দিয়ে `git push` হয় না, browser login বা token লাগে।

### Make your repository look professional

| Item | Why it matters |
|---|---|
| Clear `README.md` | First thing visitors read |
| **Topics** (About → ⚙️) | People can find your repo in search |
| `LICENSE` | Tells others how they can use your work |
| `.gitignore` | Keeps secrets and junk out of Git |
| Small, meaningful commits | Shows how you work |

> 💡 **Bonus:** Create a special repo named exactly like your username to get a [profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme) on your GitHub home page. Also **pin** your best repos.

### Common Git and GitHub problems

| Problem | Fix |
|---|---|
| `git push` rejected (non-fast-forward) | Run `git pull`, then `git push` again |
| `Authentication failed` | Log in again via browser, or use a token or SSH |
| `fatal: not a git repository` | You are in the wrong folder, `cd` into the repo |
| Pushed `.env` by mistake | Rotate (change) the secrets immediately, then remove the file from Git |

> 📚 **Learn more:** [GitHub Docs: Get started](https://docs.github.com/en/get-started) · [GitHub Skills (free interactive courses)](https://skills.github.com/) · [First Contributions](https://github.com/firstcontributions/first-contributions)

---

## 8. Postman

**English:** [Postman](https://www.postman.com/) is a tool to send HTTP requests to a server and see the response, without writing any frontend code. Backend developers use it to test APIs every day.

**বাংলা:** Postman দিয়ে frontend না লিখেই server এ request পাঠিয়ে response দেখা যায়। Backend developer রা প্রতিদিন API test করতে এটা ব্যবহার করে।

### Install

1. Download from [postman.com/downloads](https://www.postman.com/downloads/)
2. Install and open it (you can skip sign-in or create a free account)

> 🔧 **Alternative:** [Thunder Client](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client) works inside VS Code if you prefer one window.

### Your first request (GET)

1. Click **New → HTTP** (or the **+** tab)
2. Method: **GET**
3. URL: `https://jsonplaceholder.typicode.com/posts/1`
4. Click **Send**

You should see JSON data and status **200 OK**. ([JSONPlaceholder](https://jsonplaceholder.typicode.com/) is a free fake API made for practice.)

### Your first POST request

1. Method: **POST**, URL: `https://jsonplaceholder.typicode.com/posts`
2. Open **Body → raw → JSON** and write:

```json
{
  "title": "My first post",
  "body": "Learning backend with Postman",
  "userId": 1
}
```

3. Click **Send**. You should get status **201 Created** and your data back with an `id`.

### HTTP methods (CRUD)

| Method | Purpose | CRUD | বাংলা |
|---|---|---|---|
| `GET` | Read data | Read | data আনো |
| `POST` | Create new data | Create | নতুন data বানাও |
| `PUT` | Replace data fully | Update | পুরো data বদলাও |
| `PATCH` | Update part of data | Update | আংশিক বদলাও |
| `DELETE` | Remove data | Delete | data মুছো |

### Important status codes

| Code | Meaning | বাংলা |
|---|---|---|
| `200 OK` | Success | সফল |
| `201 Created` | New data created | নতুন data তৈরি হয়েছে |
| `400 Bad Request` | Wrong data sent by client | client এর ভুল data |
| `401 Unauthorized` | Not logged in | login করা নেই |
| `403 Forbidden` | Logged in but not allowed | অনুমতি নেই |
| `404 Not Found` | Data or route not found | খুঁজে পাওয়া যায়নি |
| `500 Internal Server Error` | Server crashed or bug | server এর ভুল |

> 📚 **Learn more:** [MDN: HTTP methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods) · [MDN: HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) · [Postman Learning Center](https://learning.postman.com/)

### Good habits in Postman

- Save requests in a **Collection** (example: `backend-zero-to-expert`)
- Use **Environment variables** (like `{{baseUrl}}`) instead of repeating `http://localhost:3000`
- Always check both the **status code** and the **response body**

---

## 🚧 Coming next in this module

| Part | Topics |
|---|---|
| Part 4 | MongoDB Atlas, PostgreSQL |
| Part 5 | First Node.js server, Common errors, Practice tasks, Interview questions, Resources |