# Learn-Git
Exercises for learning how to use git. This is part of Tech Start UCalgary's git tutorial. You can see our slides here: https://docs.google.com/presentation/d/1VirWHkI8QHIFB2E71R-vqGcnvhAHgFaG7yQ2FHZ677w/edit?usp=sharing

## Exercise A
Goal: Practice staging and committing changes

#### A1: Setting up

1. Clone this repository on to your computer.
2. Once you have cloned it, open up git bash or another command line interface in the folder you created. Type `git status` into your git console. If you are in the right place, then git should print a message like this:
``` 
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```
Once you see this output, you're good to continue!

#### A2: First commit

1. Edit the file called `song.md`. There are multiple blank spots - denoted by the brackets with capitalized words like [NOUN]. Fill in these spots with the words of your choosing. Save it. Type git status - confirm that resume.md shows up as a "unstaged change" before continuing.
2. Follow the process we outlined in the slides to add this change and create a commit for it. Name your commit "Fill in the blanks". Type git status afterwards - you should see the same "nothing to commit" message as in A1, but this time your file is saved with the changes you made.
3. Replace the first line of `song.md` with a bunch of garbage (ex: iadjnigb21ehqpe;aifw3thr2npq;aneflr). Then, stage your change, but don't commit it. Verify it this git status: you should see the file listed under staged changes.
4. Use the commands we learnt to take away the change from the staging area without getting rid of the change. Use git status to verify this worked (it should not be in staged files anymore, but you should still see your nonsense in the file itself). This means if you made other commits now, they would not include your change, but it's still there if you need it!
5. Use the commands we learnt to get rid of your change entirely, restoring the file to how it was at the most recent commit. Use git status to verify this.

#### A3: Gitignore
1. Create a folder called secrets in your repository. Create a .txt file in the secrets folder that contains your deepest darkest secret (like what you had for lunch yesterday)
2. Save [this image](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.framerated.co.uk%2Ffrwpcontent%2Fuploads%2F2020%2F02%2Fbettercallsaul507_01.jpg&f=1&nofb=1&ipt=921d402872fd79317cfe9a7bcee5253244e174d8301e25a4a9b5a175b6e59076&ipo=images) as jimmy.jpeg in your root folder.
3. Using git status, you should see indications of the new folder and files you added under untracked files. Once you do, continue to the next step.
4. Create a file called `.gitignore`. Your challenge is to add entries to this gitignore to achieve the following goals:
- Nothing from the secrets folder should be committed
- No image files that end with the exension .jpeg should be committed
Hint: you can use flags like *
5. Type git status. If you did the previous step correctly, the only file you should see now is your gitignore file. Once this is true, add it, and create a commit with it. Name this commit "Add gitignore".

## Exercise B
Goal: Practice branching

1. Pick a short alias for yourself. For example, if your name was Dwayne Johnson, your alias could be dwayne, dwajo, or therock. 
2. Create a new branch called YOUR_ALIAS_HERE/addFrog. ex: dwayne/addFrog
3. Switch to that branch. Make sure you are on that branch (type git status)
4. Add the following ASCII art at the end of `song.md`, or add any ASCII art of your choosing:
```
            _   _
           (.)_(.)
        _ (   _   ) _
       / \/`-----'\/ \
     __\ ( (     ) ) /__
     )   /\ \._./ /\   (
      )_/ /|\   /|\ \_(
```
5. Stage and commit your changes.
6. Switch back to your main branch. Is your ASCII art still there? Why or why not?
7. If you created a new branch from main, would it contain the frog? What about if you created a new branch while you were currently in YOUR_ALIAS/addFrog? If it helps you, try it out for yourself.
8. Create a new branch with a name of your choosing. Then try deleting it. If you deleted it successfully, you should not be able to switch to it. 

## Exercise C
Goal: Practice pushing and pulling

## Exercise D
Goal: Practice merge conflicts, whole workflow 