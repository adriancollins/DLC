## What is this?
This guide accompanies a workshop to learn how to use docs as code.

## Learning outcomes
You'll learn

* GitHub using GitHub Desktop.
* Simple markdown
* How to create a local static help website using MKDOCS.
* How to contribute to a docs as code project.


## Prerequisites
Before starting this guide, please make sure you have the following.

* GitHub access to this [repo](https://github.com/mckesson/DLC).
* [GitHub Desktop](https://desktop.github.com/)
* [Python 3 and pip3](https://www.python.org/downloads/). Follow [these instructions](https://ehmatthes.github.io/pcc/chapter_01/osx_setup.html#current_version) to check if Python is already installed on your computer. By default, some Apple computers have this pre-installed.
* Text editor of your choice. We recommend [Atom](https://atom.io/).


## Tasks

### 1. Sign In to GitHub Desktop
  1. Open GitHub Desktop on your computer.
  2. Click `GitHub Desktop` followed by `Preferences`.
  3. In the `Accounts` tab, click `Sign in`.
  4. Enter you your GitHub credentials and follow the instructions to verify your account.

![GitHub login](img/gh-login.gif "GitHub Login")

### 2. Clone the test repo
  1. Using you browser open the [GitHub repo](https://github.com/mckesson/DLC).
  2. Click `Clone or download`.
  3. Copy the HTTPS url.
  4. Using GitHub Desktop, select `Clone a Repository from the Internet`.
  5. Click the `URL` tab and paste the repo HTTPS url into `URL or username/repository`.
  6. Click `Clone`.

![Clone Repo](img/gh-clone.gif "Clone Repo")


### 3. Make changes
Using your file explorer (Finder for Mac or Explorer for Windows), navigate to the `people` directory of the cloned repo.
For example.
`your-local-folder\DLC\docs\people`

!!! note "note"
    If you don't know where your repo was cloned to on your computer, use GitHub Desktop to open it. Using GitHub Desktop, click `Repository` and `Open in Finder` (or `Open in Explorer` for Windows).


Open the markdown file with your name using your text editor. Make some changes for demonstration and save the file.

### 4. Test locally
We recommend that you test you documentation on you local computer before merging with the main project. This reduces the chance that something you do will break the main document.

To setup your local test environment, follow these steps.

  1. Using your terminal or command prompt, navigate to your repo location.
  2. Install the dependencies using this command `$ pip3 install -r requirements.txt`.
  3. Run the site locally using this command `$ mkdocs serve`.
  4. Using your browser, paste this URL into the address bar `localhost:8000`.
  5. Inspect your content to make sure it works as expected.

For future testing, only steps 3 - 5 are necessary.

![Run local](img/run_local.gif "Run local")

### 5. Commit
  1. Using GitHub Desktop, under `Changes`, add a summary and description to describe the changes you have made.
  2. Create a new branch by clicking `Current branch` and `New Branch`.
  3. Name your new branch with a descriptive name and click `Create Branch`.
  4. Click `Bring changes to 'your branch name'` and `Switch branch`.
  5. Click `Commit to 'your branch name'`.
  6. Click `Publish branch`.

![Commit](img/commit.gif "Commit")

### 6. Create PR
Before you merge your content with the project you must create a Pull Request (PR).

  1. Open the GitHub repo in [your browser](https://github.com/mckesson/DLC).
  2. Click `New pull request`.
  3. On 'compare:', select your branch.
  4. Click `Create pull request`.

![PR](img/PR.gif "PR")

### 7. Merge
Depending on your workflow, you can add reviewers to your PR to validate your work.
Following review, click `Merge pull request` and `Confirm merge` to combine your branch to the master branch.

![PR](img/merge.gif "merge")

## Finally
Your document changes are merged. These files will be automatically built and published. This can take a little time so be patient.
To check the build, follow this [link](https://adriancollins.github.io/DLC/).
