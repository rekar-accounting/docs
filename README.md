## Setting up SSH for github
Run the following commands in your local computer:
```bash
$ ssh-keygen -t ed25519 -C "your_email@example.com"
$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/id_ed25519
$ clip < ~/.ssh/id_ed25519.pub
```
Now, you should add your ssh key to your github account according to this [link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

In the next step, you can test your ssh connection by running the following command:
```bash
$ ssh -T git@github.com
```

## Clone a remote repository

```bash
$ git clone [remote-address]
```

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
- Pull Requests: merge [source-branch] into [target-branch]
