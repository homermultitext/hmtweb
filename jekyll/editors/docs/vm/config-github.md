---
title: Configuring your github account in the HMT VM
layout: page
---


Before you can commit and push to github, you need to configure your `git` settings in the HMT VM to tell it who you are on GitHub. That requires the following two commands. First,

    git config --global user.name "YOUR NAME"

YOUR NAME should be your real name (not your github user name).

Then,

    git config --global user.email "YOUR GITHUB EMAIL"

YOUR GITHUB EMAIL should be the email you used when you signed up for a GitHub account.

When you push, you will still be asked for your GitHub username and password.

In addition, it's a good idea to define a preferred text editor, in case git needs you to supply further information (such as a message, when you commit fies). Git will helpfully try to guess at an editor to open for you, but this is not so helpful if you're unfamiliar with the editor.  The HMT VM includes a very handy editor called atom, which is a good default choice.  Configure it with the following line:

    git config --global core.editor "atom --wait"

As an aside, atom runs on pretty much any operating system.  If you'd to install it on your own computer as well, you can download it from <https://atom.io/>.
