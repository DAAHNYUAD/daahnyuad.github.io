---
title: "Creating a Static Site in GitHub Pages S26"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - lab
  - S25
  - markdown
  - Github Pages
  - VSCode
---

## Guidelines for the Lab: 

Today in lab one of the things we will be doing is to create your own site at GitHub Pages in which you post all of your coursework, including writing and visuals. Creating such a site will require us to set up GitHub, GitHub Desktop and a text editor (VSCode in S26), to learn and practice some Markdown and to get comfortable with editing on our own machine and then publishing our materials gently to the web. 

Knowing how to create such a "[static site](https://kinsta.com/knowledgebase/what-is-a-static-website/)" is an important skill in minimal and sustainable digital arts and humanities. The site is free, maintenance is minimal and it can also sit alongside examples of code or data that you have created. Curating a tidy, clear site creates a web presence for yourself. 

> This course site is created in GitHub Pages by forking the **Minimal Mistakes** starter theme. I have used this theme to model how you can go about learning for yourself. When you gain more confidence you will be able to change to other themes (or even go with the full version of the Minimal Mistakes theme) and customize them to your own liking.


STEP 1: Getting the basics set up

1.  You need to have a [Github account](https://github.com/signup). We will create a repository in it in which we install a template for the site. If you already have a Github account and would like to use it and there is a repository {yourusername}.github.io set up already, you have a few options: 

- you can delete the repository if you do not want it anymore
- you can rename the repository, e.g. if the repo were named daahnyuad.github.io you could rename it daahnyuad1.github.io and proceed with this tutorial. 
- you can create an empty repository named, for example `daah`, and then install the template inside of it. 
- you can create a new Github account for the purposes of this course. 

<img src="/assets/images/creatingacct.png" style="zoom:25%;" /> 

1.  Make sure you have downloaded a text editor of your choice for your system. This lab write up will explain how to use [Visual Studio Code](https://code.visualstudio.com/). [Sublime Text](https://www.sublimetext.com/). Others are possible, such asor [RStudio Desktop](https://posit.co/download/rstudio-desktop/), but they are not explained here. 

2.  Make sure you have downloaded [Github Desktop](https://desktop.github.com/) for your system. If you are familiar with versioning systems, you do not have to use Github Desktop and its graphic user interface, but this tutorial assumes that you do. Some folks like to use [Visual Studio Code](https://code.visualstudio.com/) because they can push their code directly to GitHub as explained [here](https://www.youtube.com/watch?v=7JjVz_1t34Q), but we have kept the intermediate step to foreground the versioning process. Feel free to work in the way that is most intuitive and efficient for you. I suggest starting with Github Desktop and transitioning to VSCode.
 

STEP 2  "Forking" a repo. 

Detailed general instructions for forking can be found [here](https://liamodwyer.github.io/github-pages/5-templates.html)

4.  Once you have chosen your option from step 1, number 1, you can proceed with making a duplicate of the template we will be using. We do this by navigating to the main page of an existing GitHub page of `minimal-mistakes` and will be using their starter template: https://github.com/mmistakes/mm-github-pages-starter

With your GitHub account open (you can tell it is open when you see the icon of your account at top right), navigate to this link above, look above the file list to the right, and click `Use This Template` (If you do not see it, you may have to go to Settings to click it on). Select `create a new repository`. This will take what is at `minimal-mistakes` and transfer it over into your account.

On the page `create a new repository` you need to give the repository a name. Type exactly {yourusername}.github.io where {yourusername} is your GitHub user name. Make sure you set the repository to public and then click on the green button `create repository`

<img src="/assets/images/namingrepo.png" style="zoom:25%;" />

If you choose option 3 above (installing the template into a new repository), make sure that you are installing to the correct repo. 

The detailed instructions linked at the top of Step 2 gives you another template and points you to many more to choose from. Note that the repo we have forked is a simplified version of `minimal-mistakes`. If you want to tap into all the options of the full version, you will have to download the full theme and do more work!

> We will use the starter website (and customize it) for our work in IM-UH 1511, including the creation of pages and posts.


STEP 3 Connecting the cloud-based Github to your own machine.


5.   Cloning this repository to Github Desktop

Open GitHub Desktop and log into it with your credentials from your GitHub account. You can check that at Setting > Accounts. 

Then, click on the down arrow which reveals a button `add` with another down arrow which takes you to Clone Repository. 

<img src="/assets/images/clonerepo1.png" style="zoom:40%;" />

There are several ways of finding the repository you want to clone. When you install Github Desktop for the first time it may ask you if you want to clone.

A sure way of selecting the right place is to copy the URL of your repository where you forked the `minimal-mistakes`template. You can paste that URL in the URL tab and click clone. 

<img src="/assets/images/clonerepo.png" style="zoom:60%;" />

If successful, you should be able to see the repository in the current repository tab at top left in Github Desktop. 

6.  Editing the repository on your own machine. 

Now that you have a copy of the repository on your laptop you can edit it there (even offline and with no internet connection) and then later "push" the changes to the web. 

When you edit and save (and sometime enter a commit message), you will see a blue button to transfer these changes to the web. 

<img src="/assets/images/pushing.png" style="zoom:25%;" />

NB: You can do some editing in the GitHub web interface itself, but I recommend editing in Github Desktop, and not to mix the two, since you end up with a versioning nightmare.

Let's make some changes in Sublime Text and push them. 

<img src="/assets/images/pushing.png" style="zoom:25%;" />

From GitHub Desktop you can also select which text editor you want to work in. 

NB: It is possible to do some editing in the GitHub web interface itself, but I recommend editing in Github Desktop, and not to mix the two, since you end up with a versioning nightmare.

> Remember that every time you push to the web, the compiler works to make your page's updates.  Be patient and look for the green arrow which indicates that your site has been rebuilt with the changes you made. If you see a brown dot next to the last commit message in the repository holding the site, the compiler has not finished. Go have some tea or a quick walk--it will be done soon. 

There is a follow up post [Customizing your Static Site in GitHub Pages]().

Enjoy!
