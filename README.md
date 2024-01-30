# Import-own-libraries
This repo shows how to import functions that are in different folders in the same project.

The most important part of this program is the configuration of the launch.json inside the folder .vscode.
This configuration is run first even if we run from terminal in vscode or pressing run in the menu.


"version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "program": "C:/RICARDO/CISTECH-CISTEL/cistech/2024/import own libraries/src/main.py",
            "request": "launch",
            "console": "integratedTerminal",
            "cwd": "C:/RICARDO/CISTECH-CISTEL/cistech/2024/import own libraries/",
            "env": {
                "PYTHONPATH": "${cwd}"
            }
        }
    ]
    
The most important parameters inside the launch.json are the following:
cwd: it is directory/folder where python will start the run. Put the path of the folder project
env: the PYTHONPATH is the most important parameter. It is necessary to put this. Otherwise, it does not work.
