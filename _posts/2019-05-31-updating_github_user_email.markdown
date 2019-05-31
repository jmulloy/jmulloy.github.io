---
layout: post
title:      "Updating Github User Email "
date:       2019-05-31 12:11:20 +0000
permalink:  updating_github_user_email
---


I recently discovered that most of my commits were not showing up on Github. Upon doing some research I realized that I needed to update my user email address in my local editor on my computer in order to track those changes on my Github account. I noticed this because I went into one of the recent projects I have been working on and I noticed that the commits were showing up with a generic avatar image and a user with the name “GitHub username”. Obviously, this was wrong considering I have my own generic user name for my account that I created when I first started studying and working on web development. I was able to confirm my findings by running the `user.email` command in my terminal and it quickly returned `github user email.` WHich again, is also wrong considering I have my own personal email assigned to my Github account. After all, I needed an email to set up the account in the beginning. 

To fix this issue, I did some research through GitHub forums and I found that there was an easy way to update the author email address for the GitHub commits I am pushing on a weekly basis. I ran `git config --global user.email "email@example.com` in my terminal and I was able to quickly update the email to be correctly associated with my account. This seems to be a fairly common issue that pops up for new web developers. Most amateur developers start out my working through online courses or even a boot camp. Most of these courses don't require a user to update this information immediately due to being able to fork and clone different repositories that were set up by the course. However, this is crucial for any potential employers or colleagues to be able to see what is being worked on by a specific GitHub user/team member. This is a change that took place presently. This change did not update all of my previous commits and I am working to find an alternative solution for this issue ASAP.
