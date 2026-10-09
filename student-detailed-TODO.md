# Setup & Workflow Checklist

The present checklist is designed to guide you through the initial setup of a GitHub repository for periodic reporting about a project and to establish a workflow for regular updates and reporting. 

NOTE: This checklist is very detailed (hence very long...) as it is meant to be a **step-by-step guide for students who begin with GitHub**, version control, and the reporting process.

By the end of this checklist, you will be able to: 
- Set up a GitHub repository for your periodic project report
- Use GitHub Desktop and VSCode to manage your repository 
- Follow a structured workflow for regular reporting to your supervisor 

For a student who is new to GitHub and version control, the initial setup may take up to a few hours, but this time is well invested for learning tools that are widely used in the industry and in research.

----
## 1. Set up the necessary tools 

You will alternate between VSCode :blue_heart:, GitHub Desktop :purple_heart: and GitHub web interface :green_heart: to create the repository and manage periodic updates of the report.


  > :orange_circle: If you have any questions or need assistance, ask your favorite LLM for detailed instructions, but do it wisely, reviewing the instructions and **understanding them** before proceeding. Do not hesitate to ask your LLM for a detailed explanation of any step you find unclear in its previous response. 


- [ ] :green_heart: Create a GitHub account on the Internet 

  > :green_circle: If you do not have a GitHub account yet, create one. Ask your favorite LLM for suggestions on **how to choose a username** and use your **university email address** for the primary email (you easily change the primary email later, but changing the username later can be cumbersome).

  > :green_circle: If you already have a GitHub account with a personal email, you should add the university email as a secondary email in your GitHub account settings and *set it as the primary email for this repository*. This way, you can keep your personal and professional work separate while still using the same account. :warning: **The common mistake is to create a new GitHub account with the university email**, as *GitHub does not allow multiple accounts with the same email*. 


 - [ ] :green_heart: Ask for free Copilot access, by [applying for a student program](https://education.github.com/pack). **Copilot is not mandatory, so you can go to the next steps without it.**  Yet, Copilot is highly recommended to assist you in generating a clear report and commit messages based on the changes you made in the report.
   > :orange_circle: It can take up to a few days for GitHub to approve your request, so **do this step early in the process**.


- [ ] On your computer, install GitHub Desktop   :purple_heart: 
  GitHub Desktop provides a user-friendly interface for managing your GitHub repositories, creating commits, and visualizing changes without needing to use the command line. 


- [ ] On your computer, install  VSCode  :blue_heart: 
  VSCode is a powerful code editor that supports markdown editing and has a wide range of extensions that can enhance your workflow. 

  - Inside  VSCode, set up your tools: 
    - [ ] install the *Markdown Preview Enhanced* extension 
    :warning: this is mandatory to preview and export markdown to HTML with correct formatting and images.
    - [ ] activate *GitHub Copilot* by signing in with your GitHub account that has access to Copilot.
    :green_circle: Copilot is of great help to provide suggestions and help learn how to use the tools. 
 

---
## 2. One-time setup of the repository 
In this very first step, you want to create a new repository for your project report based on the provided template. 

### 2.1. Create the repository on GitHub from the template

- [ ] :green_heart: Go to https://github.com/DenisMot/PeriodicReport 
- [ ] :green_heart: Sign in with your GitHub account
- [ ] :green_heart: Click "Use this template" (green button on top of the page) --> "Create a new repository"
- [ ] :green_heart: Name the repository at your name: `periodic-report-firstname-lastname`
- [ ] :green_heart: Include all branches = OFF (only main)
- [ ] :green_heart: Description: "Repository for periodic report of the [Title of the project]"
- [ ] :green_heart: Set repository to Private 
  > :red_circle: :warning: Do not make the repository public now :warning: :red_circle:, as it contains information about your project that may be confidential. You can always change the visibility later if allowed by your supervisor, but it's safer to start with a private repository.

- [ ] :green_heart: Click "Create repository from template"


### 2.2. Clone the repository to your local machine
Once the repository is created and set up correctly on GitHub, you need to clone it to your local machine using GitHub Desktop :purple_heart:. This allows you to work on the report locally and manage changes using Git.
- [ ] :purple_heart:  Clone the repository to your local machine using GitHub Desktop 

  - :purple_heart: File > Clone repository > select your project report repo
  > :green_circle: Save this repository on your computer in `User/Documents/GitHub/EuroMovDHM/ProjectReport/`.

|  Repository  | Description |
| -------- | ------- |
| Local Repository | Your local copy of the repository on your computer, where you *make changes* :blue_heart:  and *create commits* :purple_heart: : `User/Documents/GitHub/EuroMovDHM/ProjectReport/` |
| Remote Repository | The copy of the repository hosted on GitHub, where you *push your commits* :purple_heart:  and *create pull requests* :green_heart: for review: `https://github.com/yourusername/ProjectReport/` |

You now have the repository set up and cloned on your local machine ([Illustration of a Git repository](https://media.geeksforgeeks.org/wp-content/uploads/20250710172654460719/What-is-Git-repository.webp)), and you can start working on the report by following the workflow outlined in the next section.

> :green_circle: Now that you have the repository set up and cloned on your local machine, you will most of the time work on your local files, using VSCode:blue_heart: and GitHub Desktop:purple_heart:.


### 2.3. One-time setup of the readme file
You need to have a `README.md` file that is dedicated to your project, not the one from the template.
- [ ] :blue_heart: Open the cloned repository folder in VSCode
- [ ] :blue_heart: Delete the `README.md` file 
- [ ] :blue_heart: Rename  `project-repo-readme.md` to `README.md`
- [ ] :blue_heart: Modify the (new) `README.md` file to adapt it to your project. 
- [ ] :purple_heart: Commit the changes you made to the `README.md` file 
    - commit message: "Initial setup of readme.md" 
    - commit description: "Add all mandatory information about the project, including title, description, authors, organization, project period, supervisor, and project repository link."

### 2.4. One-time setup of the first reporting file
- [ ] :blue_heart: Create a new markdown file for the first reporting period `week-01.md` in the root of the repository. 
  > :green_circle: You should use one of examples you can find in the repository, that you can modify to suit your needs.
- [ ] :purple_heart: Commit the changes you made to `week-01.md` with a commit message "Create week-01.md"


### 2.5. Check that the repository is set up correctly
- [ ] :green_heart:  Check that the repository is created and accessible on GitHub
- [ ] :green_heart: Check that the repository is private 
  - Go to Settings > Access and check that "Private" is selected
- [ ] :green_heart: Check that the `README.md` file is present and looks correct
- [ ] :green_heart: Check that the `week-01.md` file is present and looks correct


:warning: If any check fails, go back to the previous steps and **correct the issue before proceeding**. 
:warning: It is crucial that the repository is set up correctly to ensure a smooth workflow for the interaction with your supervisor.

### 2.6. Add your supervisor as a collaborator
- [ ] :green_heart: Add your supervisor as a collaborator in the repository 
  - Go to Settings > Collaborators and add your supervisor's GitHub username
> :orange_circle: **Do not add your supervisor as a collaborator before the repository is ready**. When this is done, any push would send a notification to your supervisor, and you do not want to do that too early, when the repository is not yet ready for review.

---
## 3. Workflow for periodic reports



### Every new reporting period (usually weekly)

- [ ] **Day 1** 
  - :blue_heart: create a new file `week-XX.md` in the root of the repository for the new reporting period.

- [ ] **Throughout the reporting period** 
  - :blue_heart: Update the content of `week-XX.md` as needed
  - :purple_heart: Commit changes, but **do not push until the reporting period is complete**.


- [ ] **Last day** 

  - :blue_heart: Make the final updates to the content of `week-XX.md`
  - :purple_heart: Commit the final changes to the `week-XX.md` file
  - :purple_heart: **Push the commits to the remote repository on GitHub**. This will generate a notification to your supervisor that the report is ready for review.


---


## Commit procedure
The easiest way to create commits is to use the GitHub desktop app, which provides a user-friendly interface for creating commits and visualizing changes.

The process is as follows:
1. :blue_heart: Make changes to `report.md` in VSCode 
1.  :blue_heart: Save the file in VSCode
1.  :purple_heart: In GitHub Desktop, you will see the changed file under "Changes"
1.  :purple_heart: Check the box next to `report.md`
1.  :purple_heart: Write a commit message that summarizes the changes you made to the report during this update (e.g., "Update report with April progress and Gantt chart") :green_circle: Use the Copilot button to generate a commit message based on the changes you made in the report, but **double-check the generated text for accuracy**.

1. :purple_heart: Click the Commit button to create the commit in your local repository

:orange_circle: Once you have created some commits (usually a few, at the end of a work session), you need to push them to the remote repository on GitHub so that your supervisor can see the updates and review them. To push the commits:
1. :purple_heart: Click "Push origin" to push the commit to the remote repository


---

## Gantt chart

The Gantt chart is maintained directly in the report file `week-XX.md` as a Mermaid block.

- Use `done` for completed tasks
- Use `active` for current tasks
- Update the Gantt chart as needed throughout the reporting period to reflect progress and changes in the plan.

:warning: Always **check the Gantt chart in the markdown preview** to ensure it renders correctly and reflects the current state of the project.

---