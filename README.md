coordination repo
---------

⚠️ NOTE - if you are using humanlayer and have found your way to this repo, it is very possible that the [Workspaces feature](https://docs.humanlayer.com/guide/workspaces) obviates the need for a standalone repo, or at least the claude config and additionalRepos part of it. You may still want this setup for shared AGENTS.md, skills, etc.

### Setup

1. create a new repo from this template

2. Clone this repo as a sibling to all your other repos:

```
~/src
  - repo1
  - repo2
  - rpi-coordination
```


3. edit .claude/settings.json to list out all repos you want to work on

```json
{
  "permissions": {
    "additionalDirectories": [
      "../repo1",
      "../repo2"
      ]
  }
}
```


4. edit CLAUDE.md to add list of repos and brief descriptions

replace this placeholder text in the markdown file:

```xml
This is a coordination repo for multiple repositories. The repos you have access to are:

- ../repo1 - [DESCRIPTION]
- ../repo2 - [DESCRIPTION]
```

### Instructions

Run all your sessions from here
