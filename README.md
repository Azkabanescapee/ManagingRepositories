# Managing Repositories

Hopefully everyone has had some practice by now making copies of repositories on GitHub (forking) and on your local computer or HPC (cloning), but recently I've gotten several questions about the steps to submit assignment files so I wanted to walk through the process from start to finish. Please also see the attached slides for a graphical overview.

(1) Each repository will start by being available as part of the class organization on GitHub:

https://github.com/IntroToCompBioLSU-Spr20

(2) To make your own copy in your GitHub account, you can click on the "Fork" button in the upper right corner of a repository page. The new copy (the fork) will be stored remotely on the GitHub servers, but is owned by you.

(3) To make a local copy of the repository on your computer or your HPC account, we need to make a clone. It's best to clone _your_ fork of the repository, since you own it and can send (push) new files and edits back there later. To make a clone of your fork, go to the GitHub page for your fork, then click the green "Clone or download" button. After the pop-up box appears, click the clipboard icon to copy the path to your fork. The path should be of this form:

https://github.com/YourUserName/RepoName.git

Open Terminal on your computer or HPC, navigate to the location where you want to copy the repository, then run

git clone https://github.com/YourUserName/RepoName.git

YourUserName and RepoName will need to be changed to the names appropriate for your fork.

(4) Now you own both a local (clone) and remote (fork) copy of the repository! You should do whatever is necessary to complete the assignment for the week with the files in the local clone of the repository.

(5) Once you've completed the assignment, you should use "git add <filename>" and "git commit -m "commit message" " to commit your changes to your local clone.

(6) After your changes are committed locally, you can send them back to your fork by typing

git push

Since you cloned from your fork, git automatically knows to send your changes back there. It may prompt you for your GitHub username and password.

(7) Now look back at your account on GitHub. In your fork of the repository, you should see the changes you made and committed in your local clone of the repository. 

(8) Once the changes are in your fork, you can click the "Pull request" icon (just below the "Clone or download button") to create a pull request and send your changes back to the class repository. Assignment successfully submitted!

If you're unsure whether your pull request was successful, you can go to the class page for the repository and click on the "Pull requests" tab at the top. You should be able to see a pull request with your username.

If you have any questions, please let me know.
