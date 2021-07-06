# 42 and GitHub Configuration

Hello fellow students, as many of you asked me recently how to upload your code on github  
to work remotely on your code or show off your libft, I decided to write a tutorial for you.


## **Step 0**  Getting the the key
Before we can start we need to add our public key to github as  
we want to use ssh for git authentication.  

> If you do not have a key, you can create one with `ssh-keygen`.  
> *Make sure you DO NOT overwrite an existing key.*

Navigate to your homefolder by just typing `cd`.  
We want to know the public part of the keypair.  
It is easy to get with `cat .ssh/id_rsa.pub`  
If you called your key differently, you have to adjust the command.

## **Step 1**  Adding it to github

Great job. Copy the key and make sure to copy all of it! (even the ssh-rsa at the beginning).

Navigate now to: https://github.com/settings/keys
You can now add your key there. Call it whatever you want.

## **Step 2**  Adding a remote repository to an existing project

Now we want to add an remote repository to our existing project.
First, create a n new project on GitHub. Make it private and do not add a README or License file.

**Click on ssh** after creation and copy the `git remote add command`.  
It should look like something like this: `git remote add origin git@github.com:chronikum/42add_github.git`  

**IMPORTANT**  

 `git remote add origin git@github.com:chronikum/42add_github.git`  
 should be changed to  
 `git remote add github git@github.com:chronikum/42add_github.git` 

That's because we want to add a new remote repository called github.
Navigate now to the code repository on your machine.

Now enter the command with your repository as remote path  

Example: `git remote add github git@github.com:yourrepository`

If you have done that, it is basically already done!

Just do not forget you will need to enter `git push github` to push to github.

## **Step 3**  Working remotely

We work from home often, maybe another pandemic? No worries.
You should also add your key on your private machine to github. 
After that it is as easy as `git clone`!



## WARNING

You are responsible for git conflicts.
They are easz to avoid though. Make sure you do not have more than one version you are working on  
and make sure to ALWAYS push your changes.

Thanks for reading and don't panic

Jonathan

(Need something? Hit me up on intra/slack. My user is jfritz)