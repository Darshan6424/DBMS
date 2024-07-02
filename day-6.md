#  Steps for Basic github setup with vscode

## Introduction

Hey there, So, Today's assignment is to kind of get familiar with basic things like having github setup with vscode and its step. It is a very important step if we dont know the basic then we cant go ahead. Basic layout of todays main focus is:

1. Creating a Gmail account
2. Creating a GitHub account
3. Connecting VS Code to your GitHub account
4. Cloning/pulling a repository from GitHub
5. Pushing a repository/folder to GitHub
6. Publishing the repository as a live site

## 1. Creating a Gmail Account 

1. **Go to Gmail:** Open your browser and go to [Gmail](https://www.gmail.com).
2. **Create an Account:** Click on **Create account**.
3. **Choose Account Type:** Select **For myself** or **For my business**.
4. **Fill in Details:** Enter your first name, last name, desired username, and a strong password. Click **Next**.
5. **Verify Your Phone Number:** Enter your phone number for verification and follow the instructions.
6. **Complete Setup:** Provide the additional information required and finish the setup process.

**Tip:** Choose a username that is kind of unique and easy to remember for future use!

## 2. Creating a GitHub Account 

1. **Open GitHub:** Go to [GitHub](https://www.github.com).
2. **Sign Up:** Click on **Sign up**.
3. **Enter Details:** Provide a username, email address, and password. Click **Create account**.
4. **Verify Your Email:** Follow the instructions sent to your email to verify your account.
5. **Choose Your Plan:** Select the **Free** plan (or Pro if you need advanced features).

**Tip:** Your GitHub username is very important as all of your project will be hosted with that particular username. So think of a kind of coolll name.

## 3. Connecting VS Code to GitHub Account 🔗

1. **Open VS Code:** Launch Visual Studio Code on your computer.
2. **Install GitHub Extension:** Go to the **Extensions** view by clicking the Extensions icon in the Activity Bar on the side of the window. Search for **GitHub Pull Requests and Issues** and install it.
3. **Sign In to GitHub:** Press **F1** (or `Ctrl+Shift+P`) to open the Command Palette. Type **GitHub: Sign in to GitHub** and select the command. Follow the prompts to authenticate with GitHub.

**Tip:** Installing github pull and issue request extension will save you from trouble of doing pull commit push usiong commands. But u can directly use ui to do so.`but its recommended to learn commands `

## 4. Cloning/Pulling a Repository from GitHub 

### Cloning

1. **Open VS Code:** Launch Visual Studio Code.
2. **Clone the Repository:** Press **F1** (or `Ctrl+Shift+P`) to open the Command Palette. Type **Git: Clone** and select the command.
3. **Enter Repository URL:** Paste the URL of the repository you want to clone. 
4. **Choose Local Directory:** Select a local directory where the repository will be cloned.

**Tip:** Cloning a repo is like getting a personal copy of a project. So the orginal repo that you cloned wont get affected if u mess up with the clone repo.

### Pulling

1. **Open Terminal:** In VS Code, open the terminal (`Ctrl+` or `Cmd+`).
2. **Navigate to Repository:** Use the `cd` command to navigate to your local repository directory.
3. **Pull Changes:** Type `git pull` and press **Enter** to pull the latest changes from the remote repository.

**Tip:** Pull regularly to keep your local project in sync with the remote repository.

## 5. Pushing a Repository/Folder to GitHub 🚀

1. **Open VS Code:** Launch Visual Studio Code.
2. **Open Terminal:** In VS Code, open the terminal (`Ctrl+` or `Cmd+`).
3. **Navigate to Project Directory:** Use the `cd` command to navigate to your project directory.
4. **Initialize Git:** If the repository is new, initialize it by typing `git init`.
5. **Stage Your Files:** Add your files to the staging area by typing `git add .`.
6. **Commit Your Changes:** Commit your changes with a message by typing `git commit -m "Initial commit"`.
7. **Add Remote Repository:** Add the remote repository by typing `git remote add origin <repository-URL>`.
8. **Push Your Changes:** Push your changes to the remote repository by typing `git push -u origin master`.

**Tip:** Writing good commit messages is an important thing to do from beginning. As it will help you know what changes u did to the code without having to need to look through entire code

## 6. Publishing the Repo as a Live Site (GitHub Pages) 🌐

1. **Go to Your Repository:** Open your repository on GitHub.
2. **Open Settings:** Click on **Settings** at the top of the repository page.
3. **Scroll to GitHub Pages:** Scroll down to the **Pages** section.
4. **Select Source:** In the **Source** section, select the branch you want to publish and the directory (usually **root**).
5. **Save:** Click **Save**.
6. **Access Your Site:** Your site will be published at `https://<username>.github.io/<repository>`.


## Conclusion

If u folloe those above mentioned step, then you will be able to understand the flow. But you need to practise on your own, test on your own to have mastery over this topic.  
