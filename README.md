📌 Step 2: git push and git pull Explained

Git push and pull are used to synchronize your local repository with a remote repository (e.g., GitHub).

⸻

🔹 git push – Send Local Changes to Remote

🚀 What Happens When You Run git push origin main?
	1.	Finds Differences – Git compares your local main branch with the remote main branch.
	2.	Uploads New Commits – If your local branch has new commits that the remote doesn’t have, Git sends them to GitHub.
	3.	Updates Remote Repository – The remote branch gets updated with your latest code.

✅ When to Use git push?
	•	After making changes and committing them (git commit -m "message")
	•	When you want to update the remote repository with your local changes.


 git add .
git commit -m "Fixed a bug"
git push origin main

🔹 git pull – Get Remote Changes Locally

⬇️ What Happens When You Run git pull origin main?
	1.	Fetches Latest Changes – Git checks if the remote repository (origin/main) has new commits.
	2.	Merges Them Locally – If there are changes, Git downloads them and merges them into your local branch.

✅ When to Use git pull?
	•	Before making new changes to ensure your local repo is up to date.
	•	When collaborating with others to get their latest changes.
	•	If Git tells you “Your branch is behind ‘origin/main’”, meaning the remote has new commits.

git pull origin main

📌 Step 3: Checking for Local and Remote Changes

Before pushing or pulling, check your status:

git status  # See local changes
git branch  # Ensure you're on the correct branch
git log --oneline --graph --all  # See commit history
Now you can decide whether to git push (send changes) or git pull (get updates). 🚀
