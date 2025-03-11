--exercise 5 history--





gymuruhimbi@uruhimbis-iMac squashing % git init
Initialized empty Git repository in /Users/gymuruhimbi/Documents/squashing/.git/
gymuruhimbi@uruhimbis-iMac squashing % git remote add origin https://github.com/bdushime/Git-Advanced-Exercise.git
gymuruhimbi@uruhimbis-iMac squashing % touch firstFile.txxt
gymuruhimbi@uruhimbis-iMac squashing % touch firstFile.txt 
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the first file' > firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating first file'
[main (root-commit) 24165b9] Creating first file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push -u origin main                      
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 254 bytes | 254.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymuruhimbi@uruhimbis-iMac squashing % touch secondFile.txt                         
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the second file' > secondFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add secondFile.txt                       
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating second file'           
[main f6cad50] Creating second file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 secondFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push                                       
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
   24165b9..f6cad50  main -> main
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
f6cad50 (HEAD -> main, origin/main) Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2
fatal: invalid upstream 'HEAD~2'
gymuruhimbi@uruhimbis-iMac squashing % touch thirdFile.txt                            
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the third file' > thirdFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add thirdFile.txt                          
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating third file'          
[main 8acb35c] Creating third file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 thirdFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push                                     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 343 bytes | 343.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
   f6cad50..8acb35c  main -> main
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2                         
[detached HEAD 7d636cb] Creating second file
 Date: Tue Mar 4 11:04:49 2025 +0200
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 2 insertions(+)
 create mode 100644 secondFile.txt
 create mode 100644 thirdFile.txt
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline

7d636cb (HEAD -> main) Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2
fatal: invalid upstream 'HEAD~2'
gymuruhimbi@uruhimbis-iMac squashing % touch fourthFile.txt                         
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the fourth file' > fouthFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add fourthFile.txt                        
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating fourth file'          
[main 4727fcb] Creating fourth file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 fourthFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2                          
[detached HEAD 41a590a] Creating third and  fourth file
 Date: Tue Mar 4 11:04:49 2025 +0200
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 3 files changed, 2 insertions(+)
 create mode 100644 fourthFile.txt
 create mode 100644 secondFile.txt
 create mode 100644 thirdFile.txt
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git add .
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
41a590a (HEAD -> main) Creating third and  fourth file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % 





 --exercise 6 and 7 history --










 gymuruhimbi@uruhimbis-iMac squashing % git init
Initialized empty Git repository in /Users/gymuruhimbi/Documents/squashing/.git/
gymuruhimbi@uruhimbis-iMac squashing % git remote add origin https://github.com/bdushime/Git-Advanced-Exercise.git
gymuruhimbi@uruhimbis-iMac squashing % touch firstFile.txxt
gymuruhimbi@uruhimbis-iMac squashing % touch firstFile.txt 
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the first file' > firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating first file'
[main (root-commit) 24165b9] Creating first file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 firstFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push -u origin main                      
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 254 bytes | 254.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymuruhimbi@uruhimbis-iMac squashing % touch secondFile.txt                         
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the second file' > secondFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add secondFile.txt                       
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating second file'           
[main f6cad50] Creating second file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 secondFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push                                       
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
   24165b9..f6cad50  main -> main
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
f6cad50 (HEAD -> main, origin/main) Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2
fatal: invalid upstream 'HEAD~2'
gymuruhimbi@uruhimbis-iMac squashing % touch thirdFile.txt                            
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the third file' > thirdFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add thirdFile.txt                          
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating third file'          
[main 8acb35c] Creating third file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 thirdFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git push                                     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 343 bytes | 343.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/bdushime/Git-Advanced-Exercise.git
   f6cad50..8acb35c  main -> main
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2                         
[detached HEAD 7d636cb] Creating second file
 Date: Tue Mar 4 11:04:49 2025 +0200
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 2 insertions(+)
 create mode 100644 secondFile.txt
 create mode 100644 thirdFile.txt
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline

7d636cb (HEAD -> main) Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2
fatal: invalid upstream 'HEAD~2'
gymuruhimbi@uruhimbis-iMac squashing % touch fourthFile.txt                         
gymuruhimbi@uruhimbis-iMac squashing % echo 'This is the fourth file' > fouthFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git add fourthFile.txt                        
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Creating fourth file'          
[main 4727fcb] Creating fourth file
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 fourthFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2                          
[detached HEAD 41a590a] Creating third and  fourth file
 Date: Tue Mar 4 11:04:49 2025 +0200
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 3 files changed, 2 insertions(+)
 create mode 100644 fourthFile.txt
 create mode 100644 secondFile.txt
 create mode 100644 thirdFile.txt
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git add .
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
41a590a (HEAD -> main) Creating third and  fourth file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 2 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   fouthFile.txt

gymuruhimbi@uruhimbis-iMac squashing % git push
To https://github.com/bdushime/Git-Advanced-Exercise.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/bdushime/Git-Advanced-Exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gymuruhimbi@uruhimbis-iMac squashing % git pull --rebase origin main
error: cannot pull with rebase: Your index contains uncommitted changes.
error: please commit or stash them.
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'trying to push after squashing'
[main b58b274] trying to push after squashing
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 fouthFile.txt
gymuruhimbi@uruhimbis-iMac squashing % git pull --rebase origin main                 
From https://github.com/bdushime/Git-Advanced-Exercise
 * branch            main       -> FETCH_HEAD
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 622 bytes | 622.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/bdushime/Git-Advanced-Exercise.git
   8acb35c..5ea932b  main -> main
gymuruhimbi@uruhimbis-iMac squashing % echo "This is an uwanted file" > unwanted.txt
gymuruhimbi@uruhimbis-iMac squashing % git add unwanted.txt
gymuruhimbi@uruhimbis-iMac squashing % git commit -m "Unwanted commit"
[main 922dccd] Unwanted commit
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 unwanted.txt
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
922dccd (HEAD -> main) Unwanted commit
5ea932b (origin/main) trying to push after squashing
2762a99 Creating third and  fourth file
8acb35c Creating third file
f6cad50 Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~2
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline   
5ea932b (HEAD -> main, origin/main) trying to push after squashing
2762a99 Creating third and  fourth file
8acb35c Creating third file
f6cad50 Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~3
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~5
fatal: invalid upstream 'HEAD~5'
gymuruhimbi@uruhimbis-iMac squashing % git rebase -i HEAD~4
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
9f2d18b (HEAD -> main) trying to push after squashing
baa713f Creating third and  fourth file
4c6443e Creating second file
6c2afa4 Creating third file
24165b9 Creating first file








--exercise,8,9 and 10 --









gymuruhimbi@uruhimbis-iMac squashing % git checkout -b ft/branch
Switched to a new branch 'ft/branch'
gymuruhimbi@uruhimbis-iMac squashing % git branch
* ft/branch
  main
gymuruhimbi@uruhimbis-iMac squashing % echo "Adding test 5" > test5.txt
gymuruhimbi@uruhimbis-iMac squashing % git add test5.txt
gymuruhimbi@uruhimbis-iMac squashing % git commit -m 'Implementing' 
[ft/branch b96d4fb] Implementing
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 test5.txt
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
b96d4fb (HEAD -> ft/branch) Implementing
69ff117 (origin/main, main)  history.md
5ea932b trying to push after squashing
2762a99 Creating third and  fourth file
8acb35c Creating third file
f6cad50 Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymuruhimbi@uruhimbis-iMac squashing % git cherry-pick b96d4fb
[main 7fdba29] Implementing
 Date: Tue Mar 4 12:41:23 2025 +0200
 Committer: Gym Uruhimbi <gymuruhimbi@uruhimbis-iMac.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 test5.txt
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
7fdba29 (HEAD -> main) Implementing
69ff117 (origin/main)  history.md
5ea932b trying to push after squashing
2762a99 Creating third and  fourth file
8acb35c Creating third file
f6cad50 Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git log --graph --oneline --all
* 7fdba29 (HEAD -> main) Implementing
| * b96d4fb (ft/branch) Implementing
|/  
* 69ff117 (origin/main)  history.md
* 5ea932b trying to push after squashing
* 2762a99 Creating third and  fourth file
* 8acb35c Creating third file
* f6cad50 Creating second file
* 24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git reflog
7fdba29 (HEAD -> main) HEAD@{0}: cherry-pick: Implementing
69ff117 (origin/main) HEAD@{1}: checkout: moving from ft/branch to main
b96d4fb (ft/branch) HEAD@{2}: commit: Implementing
69ff117 (origin/main) HEAD@{3}: checkout: moving from main to ft/branch
69ff117 (origin/main) HEAD@{4}: pull --rebase origin main (finish): returning to refs/heads/main
69ff117 (origin/main) HEAD@{5}: pull --rebase origin main (start): checkout 69ff1174926d16533cde73f588e2bb600a1f3af3
9f2d18b HEAD@{6}: rebase (finish): returning to refs/heads/main
9f2d18b HEAD@{7}: rebase (pick): trying to push after squashing
baa713f HEAD@{8}: rebase (pick): Creating third and fourth file
4c6443e HEAD@{9}: rebase (pick): Creating second file
gymuruhimbi@uruhimbis-iMac squashing % git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
gymuruhimbi@uruhimbis-iMac squashing % git push
To https://github.com/bdushime/Git-Advanced-Exercise.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/bdushime/Git-Advanced-Exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gymuruhimbi@uruhimbis-iMac squashing % git pull --rebase origin main
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 2.89 KiB | 591.00 KiB/s, done.
From https://github.com/bdushime/Git-Advanced-Exercise
 * branch            main       -> FETCH_HEAD
   69ff117..aa93539  main       -> origin/main
Successfully rebased and updated refs/heads/main.
gymuruhimbi@uruhimbis-iMac squashing % git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 298 bytes | 298.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/bdushime/Git-Advanced-Exercise.git
   aa93539..7045dd2  main -> main
gymuruhimbi@uruhimbis-iMac squashing % git log --oneline
7045dd2 (HEAD -> main, origin/main) Implementing
aa93539  history.md
69ff117  history.md
5ea932b trying to push after squashing
2762a99 Creating third and  fourth file
8acb35c Creating third file
f6cad50 Creating second file
24165b9 Creating first file
gymuruhimbi@uruhimbis-iMac squashing % git checkout 69ff117
Note: switching to '69ff117'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 69ff117  history.md
gymuruhimbi@uruhimbis-iMac squashing % git checkout main
Previous HEAD position was 69ff117  history.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gymuruhimbi@uruhimbis-iMac squashing % 









Part 3 Advanced Workflow:

Exercise 1:



 D:\The GYM git Exercises\Git Advanced Exercise3\Git-Advanced-Exercise> git stash
 Saved working directory and index state WIP on main: 6a07ca2 adding exercise 2 readme
PS D:\The GYM git Exercises\Git Advanced Exercise3\Git-Advanced-Exercise> git stash list
stash@{0}: WIP on main: 6a07ca2 adding exercise 2 readme



Exercise 7:Working with tags

gymuruhimbi@uruhimbis-iMac squashing % git checkout main
gymuruhimbi@uruhimbis-iMac squashing % git tag v1.0
gymuruhimbi@uruhimbis-iMac squashing % git tag
v1.0

Exercise 8:Listing and Deleting Tags

gymuruhimbi@uruhimbis-iMac squashing % git tag v1.1
gymuruhimbi@uruhimbis-iMac squashing % git tag v1.2
gymuruhimbi@uruhimbis-iMac squashing % git tag
v1.0
v1.1
v1.2
gymuruhimbi@uruhimbis-iMac squashing % git tag -d v1.2
Deleted tag 'v1.2' (was 4a5004e)







   
