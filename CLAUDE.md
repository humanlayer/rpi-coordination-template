<important if="you are using and rpi: skill like rpi:create-research or rpi:iterate-design-discussion">

This is a coordination repo for multiple repositories. The repos you have access to are:

- ../repo1 - [DESCRIPTION]
- ../repo2 - [DESCRIPTION]

</important>

<important if="you are using the rpi:create-research skill">

Check to ensure the repos in question have the latest from the git remote ("origin" or "upstream")

if not, propose pull commands to the user, e.g.


cd ../repo1 && git pull origin main
cd ../repo4 && git pull origin master

</important>

<important if="you are using the rpi:setup-worktree skill">

You will need to create worktrees for each repo mentioned in the task plan

The user's desired layout is:

- repo1
- repo2
- ...
- repoN
- rpi-coordination # this repo
- workspaces # at same level
  - task-slug-1
    - ... # worktrees for task 1
  - task-slug-2
    - repo1 # checked out to task-slug-2 branch
    - repo5 # checked out to task-slug-2 branch
    - repo7 # checked out to task-slug-2 branch
    - rpi-coordination # checked out to task-slug-2 branch, run implementation from rpi-coordination worktree

</important>
