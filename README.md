# vscode-notes
VS Code related things, mostly for myself.

## Javascript

### Using Prettier with ESlint
This setup will use Prettier to format the code based on the rules in your .eslintrc file. Meaning it will insert semicolons if required, set the correct number of spaces in your indents etc. etc.

Here's how to do it.  
This assumes you have already set up the project, installed eslint, and configured the .eslnitrc file.

**1. Install prettier-eslint**  
`npm install -D prettier-eslint`

**2. Install the prettier plugin for VS Code.**  
In VS Code, press `CMD+SHIFT+X` and search for `Prettier - Code formatter` to find it.

**3. Enable prettier-eslint in VS Code**  
Open the user settings by pressing `CMD+SHIFT+P` and search for settings.  
In the settings, search for the setting `Prettier: Eslint Integration`. Click the checkbox to enable the setting.

### Git Project Manager (GPM)
![GPM](https://raw.githubusercontent.com/manskronkvist/vscode-notes/master/gpm.png)
For easily navigating between project directly inside VS Code   

**1. Install the Git Project Manager extension in VS Code.**  

**2. Add configuration** 
In your you VS Code settings JSON-file, add these lines:
```JSON
    "gitProjectManager.baseProjectsFolders": [
        "~/projects"
    ],
    "gitProjectManager.codePath": "code -r",
```
Replace the project folder paths with the ones you want.  
The `code -r` in the last line will make sure that projects are opened in the same instance of VS Code (a.k.a. it doesn't open a new window.)

**4. Restart VS Code**  

Now when you open a javascript file inside a project with eslint and prettier-eslnit installed, you can simply press
`SHIFT+OPTION+F`and the code will be magically formatted according to the rules in your .eslintrc. 
No more trying to manually insert the correct amount of spaces!


## Keyboard shortcuts
Look and feel

**Zen mode**
`CMD+K Z`

**Search and open files in current project**
`CMD+P`

**Open Last Files**
`CMD+PP`

