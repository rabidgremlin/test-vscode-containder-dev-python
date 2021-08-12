# test-vscode-containder-dev-python
A project to test VS Code's local container dev setup. With a Python project.

## Setup

1. Install Docker

2. In VS Code install the "Remote - Containers extension" 

3. Launch VS Code

4. Then either:

    * If you have checked out this repo locally....
        1. Open the checked out folder in VS Code
        2. Click the green "><" box in lower left corner 
        3. Select "Open Folder in Container"

    * If you haven't checked out this repo locally....
        1. Open VS Code
        2. Click the green "><" box in lower left corner 
        3. Select "Clone Repository in Container Volume"
        4. Enter https://github.com/rabidgremlin/test-vscode-containder-dev-python as Github repo    

5. Wait for initial dev container to download/build        

## Running the app
1. Open new terminal (this will open shell in your dev container)
2. Run
```
export FLASK_APP=hello
flask run
```
3. Browse to http://localhost:5000/

## How does this work ?
See https://code.visualstudio.com/docs/remote/containers-tutorial#_how-it-works

Also check out files in `.devcontainer` to see the setup. These were creaed by VS Code using the "Remote-Containers: Add Development Container Configuration Files" option on the repo before it had a `.devcontainer` folder.

