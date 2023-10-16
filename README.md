# GitHub Actions

## Main Components
- ### Workflows
    A workflow is a configurable automated process that will run one or more jobs. Workflows are defined by a YAML file checked in to your repository and will run when triggered by an event in your repository, or it can be triggered manually, or at a defined schedule.
    Workflows are defined in the **.github/workflows** directory in a repositor, and a repository can have multiple workflows, each of wich can perform a different set of tasks.

    #### Workflow basics
    A workflow must contain the following basic components:
    - One or more events that will be trigger the workflow
    - One or more jobs, each of which will execute on a runner machine and run a series of one or more steps.
    - Each step can either run a script that you define or run an action, which is a reusable extension that can simplify your workflow


- ### Jobs
  A workflow run is made up of one or more **jobs**, which run in parallel by default. To run jobs sequentually, you can define dependencies on other jobs using the **jobs.<job_id>.needs** keywork.
  Each job runs in a runner environment specified by **runs-on**.
  
- ### Steps