# fork_and_clone

This is a repo to demonstrate the **fork&clone** workflow.

## How this workflow works

* make a fork of this repo on your Github space
* clone your fork on your development machine; this will add a remote path like this:

>    origin  https://github.com/lucaMalignaniOrg/fork_and_clone.git (fetch)

>    origin  https://github.com/lucaMalignaniOrg/fork_and_clone.git (push)
 
* now on your machine add another remote, name it for example as **upstream**, that points to the original repo you've forked. For example, if you forked from damoreluc/fork_and_clone, type in this command:
>   git remote add upstream https://github.com/damoreluc/fork_and_clone.git

then, verify the new remote of your local git:

>  git remote -v

it should respond like this:
>  origin  https://github.com/lucaMalignaniOrg/fork_and_clone.git (fetch)

>  origin  https://github.com/lucaMalignaniOrg/fork_and_clone.git (push)

>  upstream        https://github.com/damoreluc/fork_and_clone.git (fetch)

>  upstream        https://github.com/damoreluc/fork_and_clone.git (push)

---

## Pull from upstream and push locally

Now you  can pull from upstream repo into your local main branch:

>   git pull upstream main

and this updates your local repository. 

From here on, you can do your changes, commit it and finally push to your personal forked repo. **And** you can PR the original repo to include your changes.
