# GitHub Tutorial

_by Laura Arias_


#### **If you DO NOT have a cloud9 or github account:**

1. Go to [github](https://github.com/) and click "sign up" 
2. Once you have your github account, go to [cloud9](https://c9.io/login) and click the [octocat](https://preview.c9users.io/laura5a/github-learning/github-tutorial/Screen%20Shot%202018-10-19%20at%209.31.05%20AM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io). And there, you have signed up for cloud 9 using your github accout.  





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


---
## Workflow & Commands



---
## Rolling Back Changes