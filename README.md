Git \& GitHub Configuration and Workflow

Notes

1\. Repository Setup \& Initialization

Step 1: Create a new empty repository on GitHub named Hello-world.

Step 2: Navigate to your desired parent directory and clone the project:

cd ..

git clone https://github.com/.../Hello-world.git

Result: This downloads the remote repository files into your local desktop environment.

Step 3: Move inside the newly created project folder:

cd Hello-world

Step 4: (Optional) Explicitly configure or update your remote URL:

git remote set-url origin https://github.com/.../Hello-world.git

2\. Project Modifications \& Stream Redirection

Use echo commands to create files and save content:

echo Hello-world >> README.md

Note: The double arrow (>>) appends a new line or creates the file if it does not exist.

3\. Tracking Changes \& Git Lifecycle Diagram

Your notes highlight a continuous cycle for managing modifications safely:

Command / Step

Action \& Explanation

git status

git add .

Check current status and find out which changes are

untracked/unstaged.

Gather any new modifications or isolated files into the correct

compartment to get ready to save.

git commit -m "..."

git push

Save those specific files permanently into local repository history.

Send local commits up to the remote cloud repository on GitHub.

4\. Managing Untracked Files (.gitignore Rules)

The Absolute Truth: Git understands not to track a file if it is declared inside .gitignore.

Create a brand new text file named notes.txt and write project notes inside it:

echo Project notes and ideas > notes.txt

Prevent sensitive environment variables or credentials from being uploaded:

echo secrets.env > .gitignore

Ignore all system log outputs globally within the repository using wildcards:

echo \*.log >> .gitignore

