## Summary of the workflow
Generally you have two types of operation.
1. Getting changes from other users - this is updating your local copy of the repository to one that matches the one on github (this is our remote)
2. Saving your changes to the remote - this updates the remote copy to reflect your changes. **Important:** you need to make sure that you are working from a up-to-date copy of the remote so make sure that you pull before you push!

## 1. Using git with cockatrice
1.1 Open the git bash terminal. 
	(!) If you don't have it on your machine you can download it [here](https://gitforwindows.org/). 

1.2 Before you can submit your changes or pull new changes you need your shell (bash) to be in the working directory of the repository. To do this type the following command into the terminal:
```
cd ~/AppData/Local/Cockatrice/Cockatrice/decks
```

1.2a This should be the path to the cockatrice folder on your machine. 
	(!) If it isn't, find the path to your cockatrice folder through the "Load Deck" menu in Cockatrice" 
	
1.2b Your terminal should now indicate to your that you're in a git repository by stating "(master)" at the end of the prompt, for example: 
my prompt is: BAN@BAN-TOP MINGW64 ~/AppData/Local/Cockatrice/Cockatrice/decks (master)
	(!) If you don't see a word in parentheses then you need to clone (download) the repository onto your machine. Chat to BAN or JAM about this. 
	
1.3 Type in the terminal:
```
git status
```
This will list any changes to files that you have in the repository. E.g. any modifications to existing files and, separately, any new files

## Getting changes from other users
In the terminal run the following command:
```git pull```

## Saving your changes to the remote
Remember to pull before saving changes to the remote.

1. First "stage" your changes in the repository by running the following command in the terminal.
```
git add .
``` 
Note that the "." means everything in the current directory. 
2. Now type the following into the terminal, replacing the "Insert message here" with your commit message:
```
git commit -m "Insert message here"
```
3. Finally to push your changes to the remote in github
```
git push
```

### Troubleshooting
1. If you end up in vim. 
```
Press escape
Press : 
Press q
Press enter
```
