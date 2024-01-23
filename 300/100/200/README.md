# 200 - Importing a project

To import a project, go to the [projects page](https://bohr.io/projects), click "Add a New Project," and then click "Import from Github" (or go directly to https://bhor.io/projects/new/import). 

Now, select the repository with the project you want to import (e.g. ```https://github.com/agility-game/agility-game-home```). At this stage, you may need to grant permissions to bohr.io if you haven't done so earlier.

Next, define the desired subdomain (e.g. ```agility-game```), domain (e.g. ```bohr.io```), and desired environment variables.

Here is an example of our settings (based on the ```package.json``` file inside our project):

**Project**

Github repository: https://github.com/agility-game/agility-game-home

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

**WARNING**: Make sure your latest changes to your Github repository have been committed and pushed to your Github repository should you have edited remotely (such as in GitPod) before continuing.

Finally, click **IMPORT**.

There you go. 

Now, bohr.io will be installed in your GitHub repository, and your project will be deployed on bohr.io (here at: ```agility-game.bohr.io```). 

Once it's finished, your project will already be live and ready to be accessed (here at: https://agility-game.bohr.io). 

Now, you can edit your code (go to https://bohr.io/agility-game/agility-game-home)) and take advantage of bohr.io’s CI/CD along with GitHub Actions for automatic deployments of your changes.
