Here are the guidelines and details related to our process and working environment.

## Tooling

We use the following day-to-day tools:
* **Google Mail** - teleporthq.io email, which we use for all the internal tools
* **JIRA** - for product roadmap, board, issue tracking and planning
* **Confluence** - for internal documentation and product specifications
* **Slack** - for all async communication
* **Gitlab** - code repository for the internal projects
* **GitHub** - code repository and issue tracker for our open source projects
* **Figma** - for UI designs and workflows

### Security Note
It is mandatory to use a password manager for your accounts and to enable 2FA for Gitlab, GitHub and other tools that support that.

At the end of your onboarding process you should have access to all repos, run your local setups and check that everything works.

## Development Guidelines
We work as a single team, but each major task we have is connected to one of the 3 major areas or activities: **Product**, **Infrastructure** or **Research**. For research and infrastructure, the process is very flexible and the owner of each track establishes the best way to communicate and move forward with the work. The **product** activites are the core of our work and we make sure that the development pipeline is smooth at any time there. 

Each major product activity has an owner from the team and that owner should have a clear status of that story/task at all times. The JIRA product board should offer relevant information about the status of each major feature as you scroll through the board.

### JIRA issue types
Infra and Product tasks are tracked in JIRA. We use a system of stories and **sub-tasks** or **story-bugs** to keep everything organized by story, not by assignee or status. All JIRA tickets are identified with TELHQ-xxx.

All tickets go through the same workflow: Backlog, In Analysis, Todo, In Progress, In Review, Dev Complete, Ready for QA, Stage Testing, Deploy Ready.

Keep in mind to update your tasks before the daily meeting so that the board reflects the reality as much as possible.

### Gitlab/GitHub Guidelines

A few guidelines for our work with version control:
* we work with feature branches, so for each change you want to introduce, you'll create a branch from `development`
* branch name should be: prefix/TELHQ-number-title where prefix, number and title are of course dynamic. See the explanation below.
* always put ticket link from JIRA in description on GitLab. GitHub will link with the issue automatically.
* the owner of the branch/MR should merge `development` as often as possible.
* code reviews will be done using comments on the changes.
* everyone should pick unassigned MRs and do the code review.
* thumbs up if all good (GitHub has approve/reject workflow) → owner can merge it
* merge with squash, delete branch after merge

### Branch names

There are 3 dynamic parts in the branch name.

The **prefix** is the type of task the branch is addressing and can be one of the following:
* **fix** - bug fix
* **feat** - new feature added
* **imp** - improvement to an existing feature
* **ref** - refactoring work, no impact on the product
* **chore** - codebase related work (setups, CI/CD, cleanup)

The **number** should be the number of the ticket in JIRA. Ideally, all branches should follow a ticket.

The **title** should be a 3-4 word explanation of the scope of the feature/fix/task/etc.

Examples:
* feat/TELHQ-192-project-settings
* fix/TELHQ-723-stage-overlay
* ref/TELHQ-245-dependency-injection

## Process
We work in a kanban-style agile, but with a very team-tailored process. You'll get quickly onboard with the process, but for now, you should keep in mind the following:
* we have a **daily meeting** from **11:00-11:15** EEST time, everyone in gets a calendar invite for it.
* we consider the period **11:00-13:00** EEST our **core hours**, when everyone is available for interaction and meetings, please let your team know when you are not available during the time span.
* after each release we do a **retro meeting**, where we analyze the process and draw the learning points.
* on the product side, we do a **planning meeting** before each 3-4 week interation to distribute work and assign responsibilities.
* on the **infrastructure** side, we have a weekly meeting from 16:00 til 18:00 EEST every Thursday.
