# Typescript Docker (with VSCode)

Template structure to quickly initiate a Typescript project with NodeJS, in a docker context, and using VSCode.

## Prerequisites ##
Having following software installed on your environment :
* Git
* Docker & Docker-Compose
* VSCode (including "Remote Explorer" extension)

## Installation ##
Create project directory and clone repository :
```bash
cd <project_directory>
git clone https://github.com/VirtualGit/TypescriptDocker.git .
docker-compose up -d
```
Launch VSCode and attach to the container :
* In the "Activity Bar" (left), select "Remote Explorer"
* In the top dropdown, select "Containers"
* In the container list, right-click the new "template" then "Attach to container"
* A new VSCode window may open, it's now in your docker container

Initial project installation : 
* Open VSCode command palette (default Ctrl+Shift+P)
* Type "run task", press Enter
* Select "Install" and press Enter again (npm install is executing)

Execute or debug the main script
* Open file app/src/main.ts.
* Run the script (Menu Run > Start debugging).

That's all.

Note that the container will indefinitely remain up. It can be stopped with :
```bash
docker-compose down
```
