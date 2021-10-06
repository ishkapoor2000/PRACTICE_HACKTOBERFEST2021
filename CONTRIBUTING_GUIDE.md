# Contributing Guidelines

Hello👋. Welcome to Practice Repository for HACKTOBERFEST 2021✨✨
| Index                                                         |
| ------------------------------------------------------------- |
| [Contributing to this repo](#contributing-to-this-repository) |
| [Adding A New Folder](#adding-a-new-folder)                   |
| [Index (readme) Files](#index-readme-files)                   |
| [Basics of Git & GitHub](#basics-of-git-and-github)           |

## Contributing to this repository

We encourage you to share your knowledge and ideas to develop skills and gain valuable experience in the field of open source. We have created a practice repository for **HacktoberFeast 2021**, which is full of valuable resources. Folders for different domains like **Machine Learning**, **Arduino**, **Programming**, and **No_Code** have been created and contribution to a specific domain will go to that folder only. Inside each directory there will be subdirectories for sub-topics of that particular domain. For example, if someone is contributing to Programming or a subtopic of it, contributions to that domain should only go to that folder and not other.

### Types of contribution you can make

Throughout the program there are three modes of contribution, as listed below:

1. Documentation

- Content Creation in the form of codes or tutorials
- Preferred language should be English
- Clear, Consise and Complete.

2. Graphics

- Animations, Banners, presentations and regular explanatory films are all possibilties
- Video length should not exceed more than 25 min
- Presentable and Clear
- Add graphic file to the folder only if it is less than [N]MB, else provide link.

3. Coding

- Should be in specfic format
- Includes clear comments, and proper functionality
- Presentation can also be submitted along with code tutorial [Optional]
- Create proper, concise, and clear Pull Request

✔ Contributors are requested to give regular updates if any task for more than a week is assigned.

<br />

## Adding a new folder

If you are adding a new folder in any domain, you may create a new branch (optional). That branch should be created from branch `main` and not from any other branch. The naming convention of the branch should follow `Python_Pattern_Programs`. Examples are given below:

If you want to add the domain `Linear Regression` , the name of the corresponding branch and folder should be <br/>
Branch: `Linear_Regression` <br/>
Folder: `Linear_Regression` <br/>
The starting letter of every word should be in uppercase. Try not use spaces or hyphen(-). Instead use underscore (_) to join words.
All branches and folder and sub-folder names should follow this naming convention to maintain a uniformity in the repository

<br/>

## Index (readme) files

Inside each directory there is a `README` file. This is the index file of the directory. This `README` file should contain the list of sub-directories clicking on which one can navigate to a particular sub-directory. If you are adding a new sub-directory make sure you have added it to the `README` also. Again, inside subdirectories, there is another `README` file, that will contain all the topics that the subdirectory contains. The point of adding `README` inside directories and sub-directories is to help someone know about the content that is residing inside the directory or subdirectory. For the index files, please refer to the
[ templates (<- Fix this)](../templates)

---

<br />

## Repository Hierarchy

```
.root:PRACTICE_HACKTOBERFEST2021
│   CONTRIBUTING_GUIDE.md
│   README.md
│   LICENSE
│
└───Arduino
│   │   Arduino_CONTRIBUTION.md
│   │
│   └───Your_Topic
│       │   Your_Topic_CONTRIBUTION.md
│
└───Machine Learning
│   │   MachineLearning_CONTRIBUTION.md
│   │
│   └───DL
│   │   │   DeepLearning_CONTRIBUTION.md
│   │   │
│   |   └───Your_DL_Topic
│   │       │   Your_DL_Topic_CONTRIBUTION.md
│   |
│   └───ML
│   │   │   MachineLearning_CONTRIBUTION.md
│   │   │
│   |   └───Your_ML_Topic
│   │       │   Your_ML_Topic_CONTRIBUTION.md
│   |
│   └───NLP
│   │   │   NaturalLanguageProcessing_CONTRIBUTION.md
│   │   │
│   |   └───Your_NLP_Topic
│   │       │   Your_NLP_Topic_CONTRIBUTION.md
│   |
│   └───OPENCV
│   │   │   OPENCV_CONTRIBUTION.md
│   │   │
│   |   └───Your_OPENCV_Topic
│   │       │   Your_OPENCV_Topic_CONTRIBUTION.md
│
└───Prohramming
│   │   Programming_CONTRIBUTION.md
│   │
│   └───Your_Topic
│       │   Your_Topic_CONTRIBUTION.md
│
```

## Basics of Git and GitHub

### Git & GitHub

Before we proceed, it's better to know the difference between **_Git_** and **_Github_**. **Git** is a _version control system_ (VCS) that allows us to keep track of the history of our source code , whereas **GitHub** is a service that hosts Git projects. 

We assume you have created an account on Github and installed Git on your System.

Now enter your name and E-mail (used on Github) address in Git, by using following command.

`$ git config --global user.name "YOUR NAME"`
` $ git config --global user.email "YOUR EMAIL ADDRESS"`
This is an important step to mark your commits to your name and email.

<br />

### Fork a project

You can make a copy of the project to your account. This process is called forking a project to your Github account. On Upper right side of project page on Github, you can see -

<p align="center">  <img  src="https://i.imgur.com/P0n6f97.png">  </p>
Click on fork to create a copy of project to your account. This creates a separate copy for you to work on.

<br />

<br />

### Clone the forked project

You have forked the project you want to contribute to your github account. To get this project on your development machine we use clone command of git.

`$ git clone https://github.com/<your username>/PRACTICE_HACKTOBERFEST2021.git` <br/>

Now you have the project on your local machine.

<br />

### Add a remote (upstream) to original project repository

**Remote** means the _**remote location** of project on **Github**_. By cloning, we have a remote called _origin_ which points to your forked repository. Now, we will add a remote to the original repository from where we had forked.

`$ cd <your-forked-project-folder>`
`$ git remote add upstream https://github.com/<your username>/PRACTICE_HACKTOBERFEST2021.git` <br/>
You will see the benefits of adding remote later.

<br />

### Synchronizing your fork

Open Source projects have a number of contributors who can push code anytime. So it is **necessary to make your forked copy equal with the original repository**. You might face **problems** if you do not follow this step. The remote added above called **Upstream** helps in this.

`$ git checkout main`
`$ git fetch upstream`
`$ git merge upstream/main`
`$ git push origin main` <br/>
The last command pushes the latest code to your forked repository on Github. The _origin_ is the _remote_ pointing to your **forked repository** on github.

<br />

### Create a new branch for new contribution [Optional]

Usually, all repositories have a main branch that is regarded to be stable, and new features should be (optional) developed on a separate branch before being merged into the main branch. As a result, we should establish a new branch for our contribution and go to work on the issue.

`$ git checkout -b <feature-branch>`
This will create a new branch out of master branch. Now start working on the problem and commit your changes.

`$ git add --all`
`$ git commit -m "<commit message>"`
_Commit Message_ can be replaced by some valid message that helps you & other understand your reason for that commit
The first command adds all the files or you can add specific files by removing -a and adding the file names. The second command gives a message to your changes so you can know in future what changes this commit makes. If you are solving an issue on original repository, you should add the issue number like #35 to your commit message. This will show the reference to commits in the issue.

<br />

### Push code and create a pull request

You now have a new branch containing the modifications you want in the project you forked. Now, push your new branch to your remote github fork. 

`$ git push origin <feature-branch>`
_feature branch_ is the branch that you created, now, you need to copy the same changes to **your** fork's main branch by the above command.
Now you are ready to help the project by opening a pull request means you now tell the project maintainers to add the feature or bug fix to original repository. You can open a pull request by clicking on green icon -

<p align="center">  <img  src="https://i.imgur.com/aGaqAD5.png">  </p>

Remember your upstream base branch should be main and source should be your feature branch. Click on create pull request and add a name to your pull request. You can also describe your feature.

_Note_: If you face any problem, you ask in **_Doubts & Discussions_** issue.

Amazing! You've already made your first contribution.🥳

#### JUST CHILL!

#### Happy Contribution 👩‍💻👩‍💻
