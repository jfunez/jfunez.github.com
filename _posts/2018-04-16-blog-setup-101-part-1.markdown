---
layout: post
title:  "How to create a blog with Jekyll and Github Pages - part 1"
date:   2018-04-16 21:44:08 -0300
categories: en tutorials
---
Here goes the first post (of a series of posts) about how to create and setup your own blog with Jekyll and Github Pages.

As I said on [Twitter][tweet], my setup is a simple Jekyll + Github Pages.

But why? Why a python developer choose a ruby tool?

The short answer maybe is because I want to learn a little bit about it. It looks so simple! An even shorter answer could be: why not?

Let's go!

## Step 1: Create a github account

Simple! Just go to [github.com](https://github.com), click on Sign Up, then keep going...


## Step 2: Need to know Git, the basics at least

If you don't know anything about Git, this is a good chance to learn it!

You need to know the very basics commands, such as:
- `git clone ...` to download a git repo.
- `git add ...` to add files to the repo.
- `git commit ...` to commit (like "save") the changes in a new version.
- `git push ...` to send your local changes to an upstream server (a git repo).

From now on, I will assume that you have a basic knowledge of git and github.


## Step 3: Create a github repo

First, go to [github.com][github-com], and create a new repo clicking in the green button with a `New repository` label. Very easy, right?!

You need to **pay attention here** to name your new repo as: `USERNAME.github.io`, **replacing `USERNAME` with your github username**.
In my case I use: `jfunez.github.io` because my username is: [jfunez][github-profile] ;)

*From now on, everytime you see something like: `username.github.io` you need to replace `username` with your own github username.*

### Now you have a repo! take a time to enjoy it!

## Step 4: clone your new repo

Now you have to open your terminal and clone your repo to work locally.
To do this you must execute this in your console:

{% highlight shell %}
git clone https://github.com/username/username.github.io
{% endhighlight %}

**REMEMBER to replace `username` with your github username**

Then we will add some content, to do this enter the project folder and add an `index.html` file, like this:

{% highlight shell %}
cd username.github.io
echo "Hello World" > index.html
{% endhighlight %}

### What is that?:
- The first command is to enter in the repo root folder.
- The second command will print "Hello World" text, then set this text as content of the `index.html` file.

Feel free to open `index.html` file with your favorite text editor and change it with valid HTML code.

## Step 5: Send you changes to github!

We have created a few things locally in your repo. Now is time to upload this changes to github. To do this we need to use the `git push` command.


Like this:

{% highlight shell %}
git add --all
git commit -m "Initial commit"
git push -u origin master
{% endhighlight %}

### What is that?:
- first we add all files we have in the directory to be included by git in this version
- then we commit (or "save") the changes in a new version
- finally, we push the commits to our github repo

New you can access your github repo: [https://github.com/username/username.github.io][github-repo] and see your new files there.


## Step 6: Enjoy your progress!

You can see the result of your hard work opening your github page at: https://username.github.io. Remember to replace `username`... yeah, you know!

![Happy Bender Bending Rodriguez dancing](/assets/img/happy-bender.gif)

*gif from: https://giphy.com/gifs/dancing-happy-mIZ9rPeMKefm0*

[tweet]: https://twitter.com/juanfunez/status/985677306491523072
[github-com]: https://github.com/
[github-profile]: https://github.com/jfunez/
[github-repo]: https://github.com/username/username.github.io
