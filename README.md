# GitHub-Basics-
How to Pull, edit and push files on GitHub

1	Download and install Git
2	Open GitHub account
3	Open terminal or git bash and configure username and email id( use the name and ID similar to that used for making your github account)
4	$git config –global user.name ABC    ( * there is double dash infront of word global)  
5	$git config –global user.email ABC@gmail.com   ( you need to do step 5 and 6 only once, the first time when you are connecting your Git bash with GitHub account.
6	To check the changes made:  $git config –list , this will show your username and user email id. (* there is double dash infront of list)
7	In GitHub account - Create repository named datasciencecoursera or of any  other name 
8	Now create directory named coursera project on your desktop to do this 
9	At terminal- Navigate to desktop by command  cd desktop  then,  make directory by command mkdir courseraproject ( you can use any name  for your new directory, I used courseraproject )
10	Navigate to this directory by   cd courseraproject
11	 Create an empty Git repository in this directory named courseraproject by command git init
12	 screen will show that empty git repo is been created.
13	Now we need to setup connection of Git terminal on laptop with the Github available online  using HTTPS link – connecting this two is must to push your file present on desktop to Github account. So to do this give command
14	$ git remote add courseraproject < your repo link for datasciencecoursera available on github >
15	Till now you connected your Git with GitHub and created empty Git repository in directory courseraproject
16	Now we need local copy of Github repository on your laptop. To do this you need to pull courseraproject master to for this give command  $ git pull courseraproject master 
17	To check if local copy is added to your repository  courseraproject  give command 
$ ls    now you can see  Read.md file
18	 Now our task is to create Markdown file named HelloWorld.md   in directory courseraproject  to do this give command    $ touch HelloWorld. md 
19	to add content to this file give command  $ echo ## This is a mark down file >> HelloWorld.md
20	Your file is ready to be sent to staging environment. To do this give command 
$ git add HelloWorld.md
21	Now give command $ git status     You can see that your file helloworld.md is already added to staging phase and now ready to be committed.
22	Now we will commit the file, while doing so you need to mention the changes you made to the orginal file that pulled from master branch. So give command
23	 $  git commit – m “Added HelloWorld.md file & added text to it.”
24	 Now give command  $ git status   to check the status of your project. You will see notice -on branch master nothing to commit.
25	Then its time to push your project to github ( your remote repository ) and share your files with world.
26	 Give command $ git push –u courseraproject master.
Done. 
Later you can check github account and check for HelloWorld.md file .. you can open it and check if it has content in it…. When I completed this task i was not able to find written text in file HelloWorld.md, so I just edited on Github account



