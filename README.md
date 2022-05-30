## Setting up SSH for github

Run the following commands in your local computer:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
clip < ~/.ssh/id_ed25519.pub
```

Now, you should add your ssh key to your github account according to this [link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

In the next step, you can test your ssh connection by running the following command:

```bash
ssh -T git@github.com
```

## Clone a remote repository

```bash
git clone [remote-address]
```

## Adding upstream branch

```bash
git branch -u origin [upstream-branch]
```

## Creating a new branch

```bash
git checkout -b <new-branch>
```

## Switching between branches

```bash
git checkout <target-branch>
```

## Getting latest changes from remote

```bash
git pull
```

## Naming Conventions

- Branches: `rekar-[task-branch-name]`
- Pull Requests: `merge [source-branch] into [target-branch]`
- Component File Names: `TextInput.tsx` (PascalCase)
- Component Names: `TextInput` (PascalCase)
- Page File Names: `phoneVerification.tsx` (camelCase)
- Page Component Names: `[name]Page` (PascalCase e.g. `PhoneVerificationPage`)
- Function Names: `verifyPhone` (camelCase)
- Variable Names: `variableName` camelCase
- Class Names: `AuthenticationService` (PascalCase)

## Visual Studio Extensions

Install these extensions to get a better develeopment experience in you IDE:

- ES7 React/Redux/GraphQL/React-Native snippets
- Prettier – Code formatted
- Auto Rename Tag
- ESLint
- npm Intellisense
- change-case

## Useful Shortcuts in VSCode

- Alt+Shift+O to remove unused imports
