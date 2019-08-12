## C4SF Todo Project

![CoveoTodoList](coveotodos.png)

The Coveo for Salesforce Todo Project is a step by step guide for developers to get started with the Coveo JSUI Framework, Coveo for Salesforce integration package, Source Indexing and the overall Coveo tech stack when integrating.

## Installation Instructions

-   [Set up your Environment with Salesforce DX](#setting-up-JoeCoffee-using-salesforce-dx): This is the recommended setup. Use this option if you are a developer.


## Pre-requisites
1. This project assumes you are familair with version control, Git and Github.
    -   In order to get familiar with the basics, follow the steps in the [Git and GitHub Basics](https://trailhead.salesforce.com/en/content/learn/modules/git-and-git-hub-basics) Trailhead module.

## Set up your Environment with Salesforce DX

0. Get Started with Visual Studio Code. Follow the steps in the [Quick Start: Visual Studio Code for Salesforce Development](https://trailhead.salesforce.com/content/learn/projects/quickstart-vscode-salesforce) Trailhead project. The steps include:

-  Install Visual Studio Code
-  Install the Salesforce CLI
-  Use VS Code for Salesforce Development  

1. Set up your environment. Follow the steps in the [Quick Start: App Development with Salesforce DX](https://trailhead.salesforce.com/en/content/learn/modules/sfdx_app_dev) Trailhead module. The steps include:

-   Salesforce DX
-   Create an App
-   Build an App Using the Salesfsorce CLI
-   Convert and Deploy an Existing App

2. Authenticate with your hub org and provide it with an alias (**myDevHub** in the command below):

```
sfdx force:auth:web:login -d -a myDevHub
```

3. Clone the repository:

```
git clone https://github.com/gminero/coveotodos.git
cd coveotodos
```

4. Create a scratch org and provide it with an alias (**coveotodos** using the command below):

```
sfdx force:org:create -s -f config/project-scratch-def.json -a coveotodos
```

5. Push the app to your scratch org:

```
sfdx force:source:push
```

6. Open the scratch org:

```
sfdx force:org:open
```

7. You should now be ready to work on the todo tasks of this project.
