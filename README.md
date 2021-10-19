![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

# How to maintain your Codes using **git** on **GitHub** website

In this doc, you will find minimum most essential **steps** and **git commands** to maintain your projects locally (on PC) and upload them to github

## Step 1: Create your project (repository) on github website

1. Create an acount on github and sign in, 

2. Go to **Your profile**/**Repositories** and create a new repository (by clicking on **New** button)
	Generally, your repository name is something like this:
	
	`my_first_project`

3. After defining your repository name, hit **Create repository** button

## Step 2: download and install [git](https://git-scm.com/downloads) software on your PC

To **clone** (download) your project to a PC, **Update** your project **locally** on your PC, and then **push** (upload) it again to remote server (like github), YOU NEED to install **git** software on your PC
	

## Step 3: git commands to maintain your project locally (on PC)

Follow bellow steps:

1. Setup **SSH Key** for your PC according to this [Doc](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account):

	
	- Generate a new SSH key
	
			
			ssh-keygen -t ed25519 -C "YourEmail@example.com"
			
	- Add SSH key to the ssh-agent
	
			eval "$(ssh-agent -s)"
			ssh-add ~/.ssh/id_ed25519
	- Add the new SSH key to your GitHub account
	
		Copy SSH to clipboard:

			clip < ~/.ssh/id_ed25519.pub

		Go to your account **Setting / SSH and GPG keys** 
		Click on **New SSH key** button, paste your *Key*, and hit **Add SSH key** button


2. **Clone** the project to PC: (**download** a copy of your repository)
	
	* Go to a desired directory on your PC
	* Start **Git Bash** (right click and select **Git Bash Here**)
	* Git command to clone your project:
	
		 
			git clone git@github.com:[YourUserName]/my_first_project
		
		
3. Modify and Update your projects locally on your PC:

    * After updating your files locally, **stage** (**select**) all modified files to be updated:
	Git Command:
		
			git add .
	
    * **Commit** (**Update**) Selected Files:
		
			git commit -m "Your Explanation for this update" 
		
4. **Push** (**Upload**) your updated project to your remote server (like GitHub)

	* Update **remote url**: (in case, it is needed)

			git remote set-url origin git@github.com:[YourUserName]/my_first_project
		
	* **Push** (upload) your project to remote server:
		
			git push -u origin main
		


 
 

## Some additional Commands:

### Check to see **Status** of your modified "Local" repository
	git status 
### Update local repository based on remote repository   
	git pull
### Update local repository based on remote repository  and "Overwrite" current local Repo 
	git fetch --all
	git reset --hard origin/master
### Check to compare local and remote repository
	git remote update 
	git status -uno

### Git global setup
	git config --global user.name ["YourUserName"]
	git config --global user.email ["YourEmailAddress"]
### Create a file on PC 
	touch README.md                     
	touch .gitignore

In Windows, to create ".gitignore" file, besides the above command, you can create a txt file and rename it to **".gitignore."** (Windows explorer changes it to ".gitignore")

### Push an existing local project

	cd [existing_project]
	git init
	git add .
	git commit -m "Initial commit"
	git remote add origin git@github.com:[UserName]/RepoAddress
	git push -u origin main



## Contact

Email: smtoraabi@ymail.com

