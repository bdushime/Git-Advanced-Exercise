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
