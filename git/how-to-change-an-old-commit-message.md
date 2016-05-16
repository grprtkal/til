# How to Change an Old Commit Message That Has Already Been Pushed 

1. First, we list out the previous commits we want to see. In terminal, type git rebase -i @~n (n refers to how many previous commits we want to see). For example, git rebase -i @~3 will show the last 3 commits. This will open up your text editor (hopefully -- make sure you set your default text editor in your git config).
2. In your list of previous commits, change the "pick" to "reword" and write your new commit message. Save the file and close. 
3. You will be prompted to a new file that needs to be edited. Type your commit message again, save the file and close. 
4. In terminal, type "git push --force".


