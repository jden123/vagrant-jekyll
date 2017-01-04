vagrant-jekyll
===
That’s just a quick way to develop your own Jekyll site. 

Getting Started
---
1. To start working:
	```
	vagrant up
	```
	It setups VM with ruby 2.3 and github-pages. And maps local folder to "/projects" on VM.
	To choose the folder change vagrantfile(line 40):
	```
	config.vm.synced_folder 'D:\Projects\GitHubPages', "/projects"
	```

2. Use putty or similar to connect to the VM.

3. On VM go to "/projects" folder.
4. Make new site with:
	```
	jekyll new my-site-name
	```

5. Go to created folder:
	```
	cd my-new-site
	```
6. Start the local server:
	```
	 jekyll serve -H 0.0.0.0
	```

7. On local machine open a browser and go to:
	```
	localhost:4000
	```
Congratulation! You can see your new site! :)

8.  To edit the site go to "D:\Projects\GitHubPages"(or what you have set up) and put new articles to created site.