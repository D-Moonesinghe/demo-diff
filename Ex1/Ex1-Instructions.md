File: Ex1-Instructions.md

#__Ex1-Instructions.md__

This file contains instructions on how use the git diff command to see the output between the current working directory and the index (what is staged).

The following steps recreates the demo.
Steps:
1. Save the  __1-Old-Index-README.md__ to root directory as README.md
2. Add the file to staging. 
3. Commit the file.
4. From now on what you commited shows up on your index.

5.  Now open README.md in your working directory and overwrite line 9 through 13 with line 9-15 from __2-New-WorkDir-README.md__ file.
6.  Now add the modifications to the readme.md to index.
7.  Now do __"git diff --staged"__

Now what you are seeing is
    1. the README.md copy in the repo is called a/readme.md.
    2. the newly changed copy of READMEmd in the index is called b/readme.md
    3. ---- indicates lines a/readme
    4. ++++ indicates lines in b/readme.
    5. White text is common to both versions a/readme.md and b/readme.md
    6. Red text is previous text that was only seen on a/readme.md but now missing from the newer version.
    7. Green text is newly added text that is only see on the updated b/readme.md.