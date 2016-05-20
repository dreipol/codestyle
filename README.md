# codestyle
This repo contains the code styles for all JetBrains based IDEs used at dreipol

## Import instructions
- Open your IDE
- Choose Menu File > Import Settings
- Select the jar for your IDE


## IDE settings
### PyCharm
pycharm.jar

#### Formatting
- 120 chars line width
- Default Python settings
- dreipol drontend (JS/CSS/HTML) formatting

#### Macros
- reformat_and_save: Rearranges, reformats and organizes imports, then saves the file

### Android Studio
android_studio.jar

#### Formatting
- Spaces instead of tabs
- Code Arrangement and field prefixes
- Method and Field arrangement
- XML Linebreaks

#### Macros
- reformat_and_save: Rearranges, reformats and organizes imports, then saves the file

### AppCode
appcode.jar

#### Formatting
- Spaces instead of tabs
- Code Arrangement
- Method and Field arrangement

#### Macros
- reformat_and_save: Reformats, indents and organizes imports, then saves the file

# commit hooks

## prepare-commit-msg
Prefixes your git commit message with the name of the current branch.
You can link the script by executing the following commands:
```
chmod a+x ~/Documents/Repositories/codestyle/git-templates/hooks/prepare-commit-msg
mkdir ~/Documents/Repositories/[REPOSITORY]/.git/hooks
ln -s  ~/Documents/Repositories/codestyle/git-templates/hooks/prepare-commit-msg ~/Documents/Repositories/[REPOSITORY]/.git/hooks/prepare-commit-msg
```
or you can change your global config to use the template folder from codestyle:
```
git config --global init.templatedir '~/Documents/Repositories/codestyle/git-templates'
```
New repositories will have the hooks automatically. For existing repositories, you have to `git init` in the repository to add the templates. Please note that you will have to do this again if the hook-script changes.

# How to Write a Git Commit Message

1. Separate subject from body with a blank line
 - Summarise the change with a single short line 
 - Add a blank line before the body
 - Not every commit message needs a body
2. Limit the subject line to 69 characters
 - GitHub truncates subjects with more than 69 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
 - Git never wraps text automatically
 - More readable
 - You can display the column guide in Sourcetree or PyCharm
7. Use the body to explain what and why vs. how
 - Leave out details about how a change has been made
 - Focus on the reasons
 - Explain why you decided to solve it the way you did
8. Prefix subject with feature branch name
 - Set up the commit hook on your machine (see section `commit hooks` above)
 - Use short names for feature branches to stick to the second rule
9. Link the Asana task in the body
