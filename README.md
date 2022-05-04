# Setting up SSH for github
In order to push changes to your remote repository, make sure to setup SSH settings according to this [link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

## Creating a new branch

```bash
$ git checkout -b <new-branch>
```

## Switching between branches

```bash
$ git checkout <target-branch>
```

## Getting latest changes from remote

```bash
$ git pull
```

## Naming Conventions

- Branches: rekar-feature-[feature-name]
- Pull Requests: merge [<source-branch>] into [<target-branch>]
