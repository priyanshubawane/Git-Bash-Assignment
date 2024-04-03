# Git Excercise

## Master
Started the master exercise using ``git master``. Then, confirmed completion by running git verify.
```
 git start  or git start master
 git verify
````

## Commit-one-file
To begin this challenge, use either ``git start`` next or ``git start commit-one-file`` command

we have two files available, but we only want to include one of them in our commit. To do so, we can simply commit one file without including the other file. 

```
git add A.txt
git commit -m "Exercise 2"
git verify
```

## Commit-one-file-staged

There are two files added to the staging area but we need to commit one of them to do that we have two options, 1st one is to reset all and then add one of them to do that we have to do 
```
git reset
git add A.txt
git commit -m "Exercise 3"
git verify
```
And 2nd option is to unstage one file 
```
git restore --staged B.txt
git commit -m "Exercise 4"
git verify
```

## Ignore-them 
In this we have to ignore particular files and directories(Folders) in it.
 To do so firstly make an .``gitignore`` file and add the types that we wish to ignore ``.exe``  ``.o`` ``.jar`` extensions and ``library/`` directory.

```
touch .gitignore

*.exe
*.o
*.jar
library/

git add .gitignore
git commit -m "E4"
git verify
```

## Chase-branch 
The Problem is asking us to make the chase-branch point to the same commit as the escaped branch. To do so we have to merge chase branch to escaped branch using ``git merge.``

```
git merge escaped
git verify
```

## Merge-conflict 
In this problem we have to resolve the conflict while merging the branches given 

To do so, Execute The command git merge        ``another-piece-of-work`` . And we get the following result 
 git merge another-piece-of-work
```
Auto-merging equation.txt
CONFLICT (content): Merge conflict in equation.txt
Automatic merge failed; fix conflicts and then commit the result.
```
Now open the code editor and check the ``equation.txt``. Now you you can see 2 branches as mentioned below

```<<<<<<< HEAD
2 + ? = 5
=======
? + 3 = 5
>>>>>>> another-piece-of-work
``` 
Now we can resolve the conflict by editing the file to,
```
2 + 3 = 5 
```
Comment the changes as follows
```
git add equation.txt 
git commit -m "Resolved Merge Conflict"
git verify
```

## Save-your-work

In the problem, we need to save unfinished work temporarily and return to the last commit to fix a bug.

We can do so, by using ``git stash`` command.

git stash allows you to set aside the changes you've made to your files temporarily. This gives you the flexibility to work on something else and then return to your original changes later.

Now open the code editor and check bug.txt file and make changes mentioned in it. 
```
This file contains bug
It has to be somewhere.
I feel like I can smell it.
THIS IS A BUG - remove the whole line to fix it.
How this program could work with such bug?
```

Remove the 4th line as mentioned in it.
```
git add bug.txt
git commit -m "bug Fixed"
git stash pop
``` 
Finish it by adding a new line to bug.txt with
``Finally, finished it!``

```
git add .
git commit -m "Finally Fixed the bug"
git verify
```

## Change-branch-history 

In this problem, we need to change apply ``git rebase`` command to ensure that the modifications made on the 'hot-bugfix' branch are reflected in the 'change-branch-history' branch.

```
git rebase hot-bugfix
git verify
```
## Remove-ignored

The file ignored.txt is still being tracked, even though we have ignore it. This happened because we added the file before the ignoring rule was introduced. 

So we can Use ``git rm`` to remove files.
```
git rm ignored.txt
git add .
git commit -m "ignored file are not tracked anymore"
git verify
```

## Case-sensitive-filename

In this problem , we have to Remane a file from ``File.txt`` to ``file.txt``.

This can be done by ``git mv`` command.

```
git mv File.txt file.txt
git add .
git commit -m "Rename File.txt to file.txt
git verify
```

## Fix-typo 
 In this problem, there is a typo in ``file.txt``. 
 First, we will check the previous commit using ``git log``. In it, we can see that there is a typo in the word "World". 

 To resolve this issue, Use ``git commit --amend`` this will open up a text editor with the commit message which can be modified.
 Now you can edit the previous commit as mentioned.

 ```
git add .
git commit --amend -m "Fixed the typo"
git verify
```

## Forge-date
In this problem, we need to chnage the date of the commit. we can do this without modifying the commit message. 

To check the commit properties use ``git log``
for now it will show the of 2024 

To change the date to use ``--date`` option in ``git commit --amend``
```
git log
git commit --date=1987 --amend
git verify
```

## Fix-old-typo
This problem is quite like extended problem of `"Fix-typo"`. Here, you have made one more commit over that last wrong commit in which you made a mistake in spelling of `"world"`. to fix that you have to use ``git rebase``. And first of all, to check all that by using ``git log``.
After using ``git rebase -i`` a text area will open up in which you have you chenge ``pick`` with ``edit`` for ``"Hello wordl"`` as mentioned in instructions.
```
git log
git rebase -i
git commit --amend '-S'
git rebase --continue
```
This last command will take you to next option in which you have to modify your file first then do this as given below.
```
git add .
git rebase --continue
git verify
```

