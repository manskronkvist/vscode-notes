# vscode-notes
VS Code related tips, tricks and shortcuts

## Javascript Specific

### Using Prettier with ESlint
This setup will use Prettier to format the code based on the rules in your .eslintrc file. Meaning it will insert semicolons if required, set the correct number of spaces in your indents etc. etc.

Here's how to do it. 
This assumes you have already set up the project, installed eslint, and configured the .eslnitrc file.

1. Install prettier-eslint
`npm install -D prettier-eslint`

2. Install the prettier plugin for VS Code.
In VS Code, press `CMD+SHIFT+X` and search for `Prettier - Code formatter`

3. Enable prettier-eslint in VS Code
Open the user settings by pressing `CMD+SHIFT+P` and search for settings.
In the settings, search for the setting ´Prettier: Eslint Integration´. Click the checkbox to enable the setting.

4. Restart VS Code

5. Now when you open a javascript file inside a project with eslint and prettier-eslnit installed, you can simply press
`SHIFT+OPTION+F`and the code will be magically formatted according to the rules in your .eslintrc. 
No more trying to manually insert the correct amount of spaces!


## Keyboard shortcuts
Look and feel

**Zen mode**
`CMD+K Z`

**Open Last Files**
`CMD+PP`


