# GitHub: Lecture Notes

> **Note on buttons:** GitHub changes its screens from time to time. If a button name here is slightly different on your screen, choose the closest match.

---

## 1. What is GitHub?

**GitHub** is a website where you keep project files online. It remembers every change made to those files. Many people can work on the same project.

GitHub is **cloud based**. This means your files live on GitHub's computers on the internet, not only on your laptop. You can open them from any device with a browser. GitHub going down is very, very rare.

### Why do people use GitHub?

**Reason 1: Code backup.**
Developers keep their code on GitHub. If a laptop breaks, the code is still safe online.

**Reason 2: Change control.**
Change control means: every change to a document is tracked and approved. This is useful for technical documents with many authors.

> **Remember:** Code is nothing but files. Text files that contain instructions are called code. GitHub works for any text file, not only code.

### Example: a steel plant

A steel plant has a technical document. It explains how to run a machine safely. Four or five people use this document:

- 1 operator
- 1 manager
- 2 to 3 staff members

Without GitHub, everyone edits their own copy. Nobody knows which copy is correct.

With GitHub:

1. The **operator proposes** a change to the document.
2. The **manager reviews** the change.
3. The manager **approves** it.
4. The change becomes **final**.

GitHub also records:

- **Who** made each change
- **What** was changed
- **When** it was changed

This is **change tracking**. The approval step is **change approval**.

---

## 2. Which files suit GitHub, and which do not?

### Files that suit GitHub: text files

A **text file** contains only letters, numbers, and symbols. You can open it in Notepad and read it. GitHub can show **exactly what changed** inside a text file, line by line.

Good examples:

- **Markdown files** (`.md`): documentation, notes, guides. Markdown is easy to learn.
- **CSV files** (`.csv`): data tables in plain text.
- **Text files** (`.txt`): plain notes.
- **Code files**: the programs developers write.

### Files that do not suit GitHub: binary files

A **binary file** is not plain text. If you open it in Notepad, you see strange symbols. GitHub cannot read inside it. It can store the file, but it **cannot show what changed**. It only knows that "the file changed".

Examples of binary files:

- Excel files, Word files, and PowerPoint files
- Videos
- Songs
- Images
- Apps that are already built

> **Simple test:** Can you open the file in Notepad and read it? If yes, GitHub is a good choice. If you see strange symbols, GitHub is not suitable.

For Word, Excel, and PowerPoint files, use OneDrive, SharePoint, or Google Drive instead.

---

## 3. Repository

A **repository** is your project. It is a folder on GitHub that holds your files and the full history of every change. People often say **repo** for short.

- Your account can have **many repositories**.
- When you create a repository, **you are the owner**.
- The owner can **add other people** to the project.

### Public and private repositories

| Type | Who can see it |
|---|---|
| **Public** | Anyone on the internet |
| **Private** | Only you and the people you invite |

> **Verify:** GitHub's rules for private repositories and paid plans can change. Check the current rules at `github.com/pricing` before you tell students the exact limits. Do not put private or sensitive files in a public repository.

---

## 4. Commit

A **commit** is a saved set of changes. Each commit has:

- A **title** (a short line that says what you did)
- A **description** (optional, for more detail)
- The **name** of the person who made it
- The **date and time**

### One commit can hold many files

Imagine a project with **5 files**. You change **3 of them**. You do not need three separate saves. You can club all three changes into **one commit**. You give it one title and one description.

Example:

- **Title:** `Update safety steps for machine 2`
- **Description:** `Changed the start-up steps in 3 documents. The old steps were unclear.`

### How to write a good commit title

- Start with a verb: *Add*, *Update*, *Fix*, *Remove*.
- Say what you did.
- Keep it short.

| Good | Not good |
|---|---|
| `Add safety checklist` | `update` |
| `Fix wrong price in price list` | `changes` |
| `Remove old contact number` | `asdf` |

---

## 5. Common files you will see in a repository

When you open a repository, you will often see these files. Each one has a purpose.

### README.md

- The **first page** of the project. GitHub shows it below the file list.
- It says what the project is, why it exists, and how to use it.
- The `.md` means it is written in Markdown.
- Think of it as the **cover page** of a file.

### Markdown files (`.md`)

- Text files that use simple symbols for formatting.
- `# Heading` makes a heading. `**bold**` makes bold text. `- item` makes a list.
- GitHub shows them in a neat, formatted way.
- Used for notes, guides, and documentation.

### CSV files (`.csv`)

- **CSV** means *comma-separated values*.
- It is a table saved as plain text. Each line is a row. Commas separate the columns.
- Excel can open it. GitHub shows it as a table.
- GitHub can show exactly which cell or row changed.

Example of what a CSV looks like inside:

```csv
item,price_in_rupees
Rice 1 kg,58
Sugar 1 kg,44
```

### Text files (`.txt`)

- The simplest file. Plain words, with no formatting.
- Good for short notes and lists.

### LICENSE

- A file that says **what other people are allowed to do** with your project.
- For example: can they copy it? Can they use it for money?
- Open projects usually have one. A small personal project may not.

### .gitignore

- A file that tells GitHub (and Git) **which files to leave out**.
- For example: temporary files or private files that should not be saved.
- The name starts with a dot. It is a normal file.
- It is more common in software projects.

### CONTRIBUTING.md

- Explains **how others can help** with the project.
- It lists the rules: how to propose a change, and what style to follow.

### CODE_OF_CONDUCT.md

- Explains **how people should behave** in the project.
- For example: be respectful and kind in comments.

### CHANGELOG.md

- A list of **important changes** over time, written for humans.
- Different from commit history: it is a short summary, not every small save.

### Code files

- Files that contain instructions for a computer. Examples: `.py` (Python), `.js` (JavaScript), `.html` (web pages).
- They are text files, so GitHub works very well with them.

### JSON files (`.json`)

- A text file that stores **data** in a structured way.
- Often used for settings and for sharing data between programs.

### Binary files (not recommended)

- Word (`.docx`), Excel (`.xlsx`), PowerPoint (`.pptx`), images, videos, and songs.
- They can be stored, but GitHub cannot show what changed inside.

---

## 6. Steps: Create a repository

1. Sign in to `github.com`.
2. Click the **+** icon at the top right, next to your profile picture.
3. Click **New repository**.
4. In the **Repository name** box, type a short name. Use small letters and dashes. Example: `plant-safety-docs`.
5. In the **Description** box, type one line about the project. (Optional.)
6. Choose **Public** or **Private**.
7. Turn **on** the switch **Add a README file**.
8. Click the green **Create repository** button at the bottom.
9. Wait for the page to load. You now see your repository. You are its **owner**.

---

## 7. Steps: Post (open) a pull request

A **pull request** is a request that says: *"Please add my changes to the project."* Someone reviews it before it is added. This is the **propose, review, approve** habit.

1. Open the repository and click the file you want to change.
2. Click the **pencil icon** at the top right of the file box.
3. Make your change in the text area.
4. Click the green **Commit changes...** button at the top right.
5. In the box that opens, type a short **commit message** (the title). You can add a **description** below it.
6. Choose the option **Create a new branch for this commit and start a pull request**. (Do not choose "Commit directly to the main branch".)
7. Click the green **Propose changes** button.
8. A new page opens. Check the title. Click the green **Create pull request** button.
9. The page now shows your pull request with the word **Open**. You have posted your request.

> **Verify:** The exact name of the button in step 7 may differ slightly. Use the button that proposes the change or opens the pull request.

---

## 8. Steps: Merge a pull request (as the owner)

To **merge** means to add the approved changes into the main project. Only the owner (or people the owner allows) can do this.

1. Open your repository.
2. Click the **Pull requests** tab, near the top of the page.
3. Click the title of the pull request you want to check.
4. Click the **Files changed** tab. Read the changes. **Green** lines are new. **Red** lines are removed.
5. Click the **Conversation** tab to go back.
6. Scroll down. Click the green **Merge pull request** button.
7. Click the green **Confirm merge** button.
8. The pull request now shows a purple **Merged** tag. The changes are now part of the main project.

---

## 9. Steps: See the commit history

**History** is the list of every saved change in the project.

### For the whole repository

1. Open the repository's main page.
2. Look above the file list. Find the link with a **clock icon** and a number, such as **12 Commits**.
3. Click it.
4. You see a list of commits. The **newest** is on top. Each line shows the **title**, the **person**, and **when**.

### For one file

1. Open the repository and click the file.
2. Click the **History** button at the top right of the file box. It has a clock icon.
3. You see all commits that changed this file.

---

## 10. Steps: See what changed in a commit

1. Open the commit history (see section 9).
2. Click the **title** of the commit you want to check.
3. A page opens showing the changes.
   - **Green lines** with a **+** were added.
   - **Red lines** with a **-** were removed.
4. If more than one file changed in that commit, scroll down. You will see each file one by one.

> This is why text files work so well on GitHub. You can see exactly who changed which line, and when.

---

## 11. Steps: Restore an earlier version

Nothing is lost on GitHub. Every old version is still in the history. To go back, we copy the old text and save it as a new commit.

1. Open the commit history of the file (see section 9, "For one file").
2. Find the **older** commit that has the version you want.
3. Click the **three dots** (**...**) at the right of that commit.
4. Click **View file**. You now see the file as it was at that time.
5. Click the **Copy raw file** icon at the top right of the file box. It looks like two small squares.
6. Go back to the repository. Click the file. Click the **pencil icon**.
7. Press **Ctrl + A** to select all the text. Press **Ctrl + V** to paste the old text.
8. Click the green **Commit changes...** button.
9. Type a clear message, such as `Restore earlier version`. Click the green **Commit changes** button.
10. The file now has the old text again. Open the history. You will see your new commit. **No older commit was deleted.**

> **Verify:** The menu names **View file** and **Copy raw file** may differ on your screen. Look for any option that shows the old file, then copy its text.

### Restore using the desktop app (mentioned only)

There is also a free app called **GitHub Desktop**. It can undo or go back to an earlier commit from your laptop. We did not demonstrate it. Check the exact menu name in the app before you teach it.

---

## 12. Quick revision

| Word | Meaning |
|---|---|
| **GitHub** | A website that stores project files and remembers every change |
| **Repository (repo)** | Your project folder on GitHub |
| **Owner** | The person who created the repository |
| **Commit** | A saved set of changes, with a title and description |
| **History** | The list of all commits |
| **Pull request** | A request to add your changes to the project |
| **Merge** | Adding approved changes to the main project |
| **Text file** | A file you can read in Notepad. Good for GitHub |
| **Binary file** | A file with strange symbols in Notepad. Not good for GitHub |
| **Public / Private** | Everyone can see it / only invited people can see it |

### Five things to remember

1. Code is nothing but files.
2. GitHub is best for **text files**: Markdown, CSV, and code.
3. Word, Excel, PowerPoint, images, videos, and songs are **binary files**. GitHub is not suitable for them.
4. A **commit** can club changes from many files into one saved version.
5. **Propose, review, approve.** This habit works for any team.
