# 200 - Importing a project

To import a project, go to the [projects page](https://bohr.io/projects), click "Add a New Project," and then click "Import from Github." Now, select the repository with the project you want to import (e.g. ```https://github.com/agility-game/agility-game-on-bohr```). At this stage, you may need to grant permissions to bohr.io if you haven't done so earlier.

Next, define the desired subdomain (e.g. ```agility-game```), domain (e.g. ```bohr.io```), and desired environment variables.

Here is an example of our settings (based on the ```package.json``` file inside our project):

**Project**

Github repository: https://github.com/agility-game/agility-game-on-bohr

**Domain**

***Subdomain***: agility-game<br/>
***Domain***: bohr.io

**Build & Development**

Set the build and development commands for your project.

**FRAMESET PRESET**: ``` ``` (leave blank if not in the list, like Svelte)

**BUILD COMMAND**: ```npm run build```

**ROOT DIRECTORY**: ```my-app```

**OUTPUT DIRECTORY**: ```src```

**INSTALL COMMAND**: ```npm install```

**DEVELOPMENT COMMAND**: ```npm run dev```

**Environment variables**

Set environment variables for your build script and add-ons.

```Leave blank for now```

There you go. 

Now, bohr.io will be installed in your GitHub repository, and your project will be deployed on bohr.io. Once it's finished, your project will already be live and ready to be accessed. Now, you can edit your code and take advantage of bohr.io’s CI/CD along with GitHub Actions for automatic deployments of your changes.
