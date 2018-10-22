# GitHub Tutorial

_by Laura Arias_


#### **If you DO NOT have a cloud9 or github account:**

1. Go to [github](https://github.com/) and click "sign up" 
2. Once you have your github account, go to [cloud9](https://c9.io/login) and click the [octocat](https://preview.c9users.io/laura5a/github-learning/github-tutorial/Screen%20Shot%202018-10-19%20at%209.31.05%20AM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io). And there, you have signed up for cloud 9 using your github accout.  
3. Now go to the addition icon next to your profile and click "New Repository"
4. After doing so, give it a name and click create 
5. It will take you to a page with code in it, on the top it will have the options for HTTPS and SSH. Pick the one that says SSH. 
6. Copy the code you see and paste it into your command line. 
7. Boom! New repository




---
## Git vs. GitHub

**Github:**
    Github is the place where all of your coding/work is stored.  
  It needs git in order to work. 
  
  **Git:**
        A type of **version-control system**  
         **Version Control System:** 
         A type of system that saves the changes in your file/directory/repository for you to look at later. 
        

---
## Repository Setup

Before you can work in git and use it's amazing tools, you need to start it. Or as the command says, initialize it. 

First things first, make sure your in the file you want to initialize git in. 
If you initialize git somewhere else or the workspace, you'll have to remove it and put it in the file you originially wanted it in. 

**How do you initialize git?:**  
    You initialize git by putting "git init" in the command line. 
    
Example: 
 ``` git 
laura5a:~/workspace/name-of-file $ git init 
```

In the end, you should get this: 

```
Initialized empty Git repository in /home/ubuntu/workspace/example/.git/
laura5a:~/workspace/filename (master) $ 
```

You see how infront of the filename it says "(master)". That means that file is now a **repository**. 
**Repository:** a foldier that has git in it (can also be called a repo)

**So what now?** 
    Well, now you have a repository. So let's **add** something to it. 
    
Although, how can I add something that still isnt there?  
 Your probably confused right now, like, we did just make a repository so how could it be that there isn't nothing?  
  Think of your repository as a foldier, right now it's empty because there is not content inside the foldier. 

So in that case, let's make some content! 
    Make a README.md file, like this! 
    
    
   ``` laura5a:~/workspace/github-tutorial (master) $ touch README.md ```

After that, you should see a README file in your repo.  
    [Like this](https://preview.c9users.io/laura5a/github-learning/github-tutorial/Screen%20Shot%202018-10-22%20at%209.38.44%20AM.png?_c9_id=livepreview2&_c9_host=https://ide.c9.io)
    
Now that you have your new README file, open it by double clicking on it and type something inside. 
    
After that, go to your command line and type git status, the README file should be red. 

Now, in the command line, type **git add**  
 **git add:** adds the changed you made in your file into git 

Now if you do git status again, you should see the readme file as green. 

Almost done! 
    Now you have to commit it. 
    
**what do i mean by commiting?**  
 Well, you have to commit your changes. You have already added your changes into git, now you have to store it. 
You do so by doing this commassnd. 
        
**git commit -m "short-message":** stores the content of your changes into git and leaves a message you wrote that would typically say what you did.     
In github, you already made a repo, all you have to do now is connect the repo there to the repo here.  
That is called a **remote**  
        
 **Remote:** setting up the connection between current repo to an external one (setting up a bridge)
  

---
## Workflow & Commands

In the previous section we talked about...
1. Git add 
2. Git Status 
2. Git commit 

But now...how to we push our code and work onto the repository in github? 
I got you, you use: 

**git push:** sends your commit from our c9 repository to the repo in github.  

 Although, if you are doing the push for the first time, you must do: 
 
 **git push -u origin master:**  
  That "-u" means "upstream". In english language, it will remember which repository in github to push all this code/work into.
  

---
## Rolling Back Changes

Unfortunetly, humans are not perfect. We all make mistakes. 
 So what happens when we add something we didn't mean to add? 
  or if we commit something we didn't mean to commit? 
   well, you can't fix those errors....just kidding! 
    This is how you can fix your changes regardless if you added or push them. 
    
0. I accidently edited something: 
You can just delete it but if you did a lot of edits, here's the easy way out;

``` git checkout -- <file>```

1. I added something by accident: 
In the command line, it will tell you what to do if you wish to undo an add. 
which is... 

```git reset HEAD <file>```

2. I accidently did a commit: 
oof, should have been careful. 

```git reset --soft HEAD~1```

3. Use this if you wanna go way back. When you want to __undo commit and add:__

```git reset HEAD~1```

4. Use this when you wanna basically restart everything. When you want to __undo commits and edits:__

```git reset --hard HEAD~1```






