# github-foundations-prep
This is a repo where I follow the study guide for the exam prep and tinker with the new concepts that I learn

## Some learning resources I found useful (and actually followed)
1. [The study guide.](https://github.com/LadyKerr/github-certification-guide/blob/main/study-guides/gh-foundations.md)  
I would take the mentioned point, copy paste it in google, then read the corresponding article that addresses that point from github docs.

2. [Questions bank](https://ghcertified.com/questions/foundations/)   
This bank is not questions taken from the exam (they explicitly mention that they don't accept questions that came in the exam but instead the question author should create the question themselves).

Although they try to follow the previous point, I have found some questions from that bank within the exam, which is pretty cool!

3.[ A course by freeCodeCamp presented by exampro](https://www.youtube.com/watch?v=Jdc0i7RcBv8&ab_channel=freeCodeCamp.org)  
I haven't watched all of the course, but the videos I watched were explained in a good way.
Also, the course walks you through using github actions and codespaces, which is optional because the exam won't ask you to do that, but instead have a general knowledge about the domain like (what is github actions and github codespaces).

I was surprised that the exam almost has no github branching and merging problem (Just MCQ about general knowledge about VCs in general, github and their products)


## Regarding contributions 
To contribute, please read our [contribution guidelines.](docs/contributing.md)
## My notes 
1. Using keywords in issues
This means that some keywords like "closes, fixes, resolve,..." will automatically close the issue when a PR is merged

2. Github actions notes 
   1. An event is like : creating an issue or a PR
   2. Workflow: a configurable automated process (using yml) that will run one or more jobs
   3. workflows are defined in `.github/workflows`
   4. The workflow can contain one or more **jobs**
   5. Each job can contain steps
   6. Runner: a server that runs the workflows when they're triggered

3. Github codespaces notes
   1. it is the more robust way to use `github.dev` as it provides you with a virtual machine to work on
   2. dev containers are docker containers that are specifically configured to provide a fully featured dev env
   3. `devcontainer.json` should be used for *customization*(share common configuration for a project) not *personalization*
   4. **deep link:** It is a way to provide a link to the codespace but you can choose the base branch that the link will point to (an overloaded way of being able to share the repo link other than the normal way)


4. Github projects: An amazing github version of jira
5. github innersource: using best practices used in big open source projects in companies in order to be more productive

### Scattered notes from [this website](https://ghcertified.com/practice_tests/foundations/)
1.  different possible lifecycle phases for github workspaces
  1. create
  2. rebuild
  3. stop
  4. delete
2. Two workflows are enabled by default in github projects
   1. When issues or PRs are closed, they are set to **DONE**
   2. when PRs are merged, they are set to **DONE**
3. What are github organizations ? => They are shared accounts where businesses and open source projects can collaborate
4.  When you stop a codespace, any running processes are stopped. 
5.  if you're using a codespace in the VS Code web client and you close the browser tab, the codespace remains running on the remote machine. 
6.  You can disconnect and reconnect to an active codespace without affecting its running processes.
7.  Types of accounts on github
    1.  User accounts
    2. Organization accounts: shared accounts when a large number of people can collaborate across many projects at once.
    3. Enterprise accounts: enable innersourcing between multiple organizations
 8. Regarding tasklists in github markdown
    1. They are being deprecated in favor of sub-issues
    2. You can create them by prepending either - [ ] or - [x] before an el to mark it is incompleted/completed
 9. Project templates: You can't set an existing project as a template, but instead you can copy the project as a template. This will make a duplicate of the current project and set that copied project as a template for your organization
 10. If a repository contains more than one `README` file, then the file shown is chosen from locations in the following order: the `.github` directory, then the repository's root directory, and finally the `docs` directory. (I thought they would 1st pick the repo root dir, since this is the default place!)
 11. deleting a project will remove everthing associated with it
 12. closing a project will retain the project contents, along with the ability to open it later
 13. Github enterprise
     1.  cloud => runs on github
     2.  server => runs on a company infrastructure
 14. Github teams: A group of users from the same org
 15. find all open issues labeled `test` that mention 'fix' in their body text
`is:issue is:open label:test "fix"`
16. repository topics: the labels you see in the left sidebar on the repo main page
   