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
