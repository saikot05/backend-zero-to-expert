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

## 9. MongoDB Atlas

**English:** [MongoDB](https://www.mongodb.com/) is a **NoSQL** database. It stores data as flexible, JSON-like **documents** instead of rows and columns. [MongoDB Atlas](https://www.mongodb.com/atlas) is its cloud version, which has a free tier, so you do not need to install a database on your computer.

**বাংলা:** MongoDB একটা **NoSQL** database। এখানে data row-column এর বদলে JSON এর মতো flexible **document** আকারে থাকে। Atlas হলো এর cloud version, free tier আছে, তাই computer এ কিছু install করতে হয় না।

### Key terms

| SQL world | MongoDB world | বাংলা |
|---|---|---|
| Database | Database | database |
| Table | Collection | table এর মতো, documents এর group |
| Row | Document | একটা record (JSON আকারে) |
| Column | Field | document এর একটা property |

Example document:

```json
{
  "_id": "665f1c2a9b1e8a0012345678",
  "name": "Saikot",
  "email": "saikot@example.com",
  "skills": ["JavaScript", "Node.js"]
}
```

### Step 1: Create a free cluster

1. Sign up at [mongodb.com/cloud/atlas/register](https://www.mongodb.com/cloud/atlas/register)
2. Create a new **Project**, then click **Create** a cluster
3. Choose the **Free (M0)** plan
4. Choose a region close to you (for Bangladesh, a nearby Asian region is usually fastest)
5. Click **Create**

> 📝 Atlas menus and names change sometimes. If a button looks different, follow the [official Getting Started guide](https://www.mongodb.com/docs/atlas/getting-started/).

### Step 2: Create a database user

Go to **Database Access** → **Add New Database User**.

- Authentication: **Password**
- Choose a username and a **strong password** (save it safely)
- Privileges: **Read and write to any database**

> ⚠️ This is the **database user**, different from your Atlas login account.
> এটা database এর user, তোমার Atlas login account না।

### Step 3: Allow network access

Go to **Network Access** → **Add IP Address**.

- Best: click **Add Current IP Address**
- For learning only: `0.0.0.0/0` (allow from anywhere). **Never use this in real production.**

If you see a timeout error later, your IP changed. Add it again here.

### Step 4: Get the connection string

1. Go to **Database** → click **Connect** on your cluster
2. Choose **Drivers** (Node.js)
3. Copy the connection string:

```
mongodb+srv://<username>:<password>@cluster0.xxxxx.mongodb.net/?retryWrites=true&w=majority
```

Replace `<username>` and `<password>` with your database user. If the password has special characters (like `@` or `#`), [URL-encode them](https://developer.mozilla.org/en-US/docs/Glossary/Percent-encoding).

### Step 5: Visual check with MongoDB Compass

[MongoDB Compass](https://www.mongodb.com/products/tools/compass) is a free GUI. Install it, paste your connection string, and click **Connect**. If you can connect, your setup is correct.

> 🔐 **Golden rule:** Never put your password directly in code or push it to GitHub. We store it in a `.env` file (see Section 11).
>
> **সোনালি নিয়ম:** Password কখনো সরাসরি code এ লিখবে না বা GitHub এ push করবে না।

> 📚 **Learn more:** [Atlas Docs](https://www.mongodb.com/docs/atlas/) · [MongoDB Manual](https://www.mongodb.com/docs/manual/) · [MongoDB University (free courses)](https://learn.mongodb.com/)

---

## 10. PostgreSQL

**English:** [PostgreSQL](https://www.postgresql.org/) (Postgres) is a powerful open-source **relational (SQL)** database. Data lives in **tables** with rows and columns, and tables are connected through **relations**. It is widely used for apps where data is structured and connected, like users, orders and payments.

**বাংলা:** PostgreSQL একটা শক্তিশালী open-source **relational (SQL)** database। Data **table** এ row-column আকারে থাকে এবং table গুলো **relation** দিয়ে যুক্ত থাকে। User, order, payment এর মতো structured data এর জন্য এটা খুব জনপ্রিয়।

### Install (local)

1. Go to [postgresql.org/download](https://www.postgresql.org/download/) and choose your OS
2. On Windows, download the installer (from EDB) and run it
3. Keep the default port **5432**
4. Set a password for the `postgres` superuser and **remember it**
5. Keep **pgAdmin 4** and **Command Line Tools** ticked

### Verify

Open a **new** terminal:

```bash
psql --version
psql -U postgres
```

Enter your password. If you see `postgres=#`, you are inside the Postgres shell.

> If `psql` is not recognized on Windows, add the Postgres `bin` folder to your PATH (for example `C:\Program Files\PostgreSQL\<version>\bin`), then reopen the terminal.

### Your first database and table

Run these inside `psql`:

```sql
CREATE DATABASE backend_practice;
\l                        -- list all databases
\c backend_practice       -- connect to your database

CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(150) UNIQUE NOT NULL,
  created_at TIMESTAMP DEFAULT NOW()
);

INSERT INTO users (name, email) VALUES ('Saikot', 'saikot@example.com');
INSERT INTO users (name, email) VALUES ('Rahim', 'rahim@example.com');

SELECT * FROM users;
SELECT name FROM users WHERE id = 1;

UPDATE users SET name = 'Saikot Ahmed' WHERE id = 1;
DELETE FROM users WHERE id = 2;

\dt                       -- list tables
\q                        -- quit
```

### CRUD in SQL

| Operation | SQL | বাংলা |
|---|---|---|
| Create | `INSERT INTO` | নতুন row যোগ |
| Read | `SELECT` | data পড়া |
| Update | `UPDATE ... SET ... WHERE` | data বদলানো |
| Delete | `DELETE FROM ... WHERE` | data মোছা |

> ⚠️ **Always use `WHERE` with `UPDATE` and `DELETE`.** Without it, you change or delete every row.
> `UPDATE` আর `DELETE` এ সবসময় `WHERE` দেবে, না দিলে সব row বদলে যাবে বা মুছে যাবে।

### pgAdmin (visual tool)

Open **pgAdmin 4** (installed with Postgres), log in with your `postgres` password, then go to **Servers → PostgreSQL → Databases → backend_practice → Schemas → public → Tables** to see your `users` table. Right-click a table → **View/Edit Data → All Rows**.

### Connection string

```
postgresql://postgres:YOUR_PASSWORD@localhost:5432/backend_practice
```

Format: `postgresql://USER:PASSWORD@HOST:PORT/DATABASE`

### Prefer no local install? Cloud options

Free cloud Postgres exists, for example [Neon](https://neon.tech/) and [Supabase](https://supabase.com/). Free plans change, so check their pricing pages for the current limits.

> 📚 **Learn more:** [PostgreSQL Official Tutorial](https://www.postgresql.org/docs/current/tutorial.html) · [PostgreSQL Docs](https://www.postgresql.org/docs/) · [PostgreSQL Tutorial (beginner friendly)](https://www.postgresqltutorial.com/) · [pgAdmin Docs](https://www.pgadmin.org/docs/)

---

## 🧠 MongoDB vs PostgreSQL at a glance

| | MongoDB | PostgreSQL |
|---|---|---|
| Type | NoSQL (document) | SQL (relational) |
| Data shape | Flexible JSON documents | Fixed tables, rows, columns |
| Relations | Possible, but manual | Strong, built in (joins, foreign keys) |
| Best for | Changing data shape, fast prototypes | Structured, connected, transaction-heavy data |
| Query language | MongoDB Query API | SQL |
| Our tools | Mongoose (Module 06b) | `pg` and Prisma (Module 06c, 06d) |

**বাংলা:** কোনটা ভালো সেটা না, কোন কাজে কোনটা মানায় সেটাই আসল প্রশ্ন। আমরা দুটোই শিখব।

---

## 🚧 Coming next in this module

| Part | Topics |
|---|---|
| Part 5 | First Node.js server, `.env` and `.gitignore`, Common errors, Practice tasks, Interview questions, Resources |