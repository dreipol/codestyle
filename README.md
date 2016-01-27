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


# commit hooks

## prepare-commit-msg
Prefixes your git commit message with the name of the current branch. You can link the script by executing the following commands
```
chmod a+x ~/Documents/Repositories/codestyle/prepare-commit-msg 
mkdir ~/Documents/Repositories/[REPOSITORY]/.git/hooks
ln -s  ~/Documents/Repositories/codestyle/prepare-commit-msg ~/Documents/Repositories/[REPOSITORY]/.git/hooks/prepare-commit-msg
```

