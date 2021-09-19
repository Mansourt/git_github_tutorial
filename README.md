![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

# How to maintain your Codes using **git** on **github** website

In this doc, you will find minimum most essential **steps** and **git commands** to maintain your projects locally (on PC) and upload them to github

## Step 1: Create your project (repository) on github website

1. Create an acount on github and sign in, 

2. go to **Your profile**/**Repositories** and create a new repository (by clicking on **New** button)
	Generally, your repository name is something like this:
	
	```my_first_project```

3. After defining your repository name, hit "**Create repository**" button

## Step 2: download and install [git](https://git-scm.com/downloads) software on your PC

To **clone** (download) your project to a PC, **Update** your project **locally** on your PC, and then **push** (upload) it again to remote server (like github), YOU NEED to install **git** software on your PC
	

## Step 3: git commands to maintain your project locally (on PC)

Follow bellow steps:

1. **Clone** the project to PC: (**download** a copy of your repository)
	
	* Go to your desired directory on your PC
	* Start **Git Bash** (right click and select **Git Bach Here**)
	* Git command to clone your project:
	
		```git 
		git clone https://github.com/[YourUserName]/my_first_project
		```
		
2. Modify and Update your projects locally on your PC:

    * After updating your files locally, **stage** (**select**) all modified files to be updated:
	Git Command:
		```
		git add .
		```
    * **commit** (**Update**) Selected Files:
		```
		git commit -m "Your Explanation for this update" 
		```
3. **Push** (**Upload**) your updated project to your remote server (like github)

	* Setup **SSH Key** for your PC accoridng to this [Doc](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
	* Update **remote url**: (default name for remote: *origin*)
		```
		git remote set-url origin git@github.com:[YourUserName]/my_first_project
		```
	* **Push** (upload) your project to remote server:
		```
		git push -u origin main
		```



## Contact

Email: smtoraabi@ymail.com

