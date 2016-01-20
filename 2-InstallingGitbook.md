##Getting Started

Go to your terminal (I highly recommend [Cmder Emulater for Windows][1]), and 

	npm install gitbook-cli -g

This will install command like tools for gitbook. Next do 

	gitbook versions

to check if the gitbook is already installed it or not. To install gitbook 

	gitbook versions:install latest

To check the version of gitbook do 

	gitbook versions:print

To check all the available versions of gitbook do 

	gitbook versions:available

To check all the versions of gitbook installed in your system do 

	gitbook versions

Now clone your repo from github / stash / bitbucket and then in your project's root folder do 
	
	gitbook init 

This will create directories and files for a book its SUMMARY.md (if it is existing) when you do 
	
	gitbook serve

When you do this two things happen
1. A **_book** folder is created with your *gitbook* in it with all html and css build
2. You can see your gitbook on http://localhost:4000 (by default), live reload is active by default.

###And you are up and running!
[1]: http://cmder.net/