# 200 - Importing a project

To import a project, go to the [projects page](https://bohr.io/projects), click "Add a New Project," and then click "Import from Github" (or go directly to https://bhor.io/projects/new/import). 

**WARNING**: Make sure you pick the correct ```owner``` from the drop down menu (here: ```agility-game```, **not** wvanheemstra) in Bhor.io.

Now, select the repository with the project you want to import (e.g. ```https://github.com/agility-game/home```). At this stage, you may need to grant permissions to bohr.io if you haven't done so earlier.

If the **Import** button is shown, that means you have already successfully authorized bohr against this Github repository, click the button to import. Else, continue.

Next, define the desired subdomain (e.g. ```agility-game```), domain (e.g. ```bohr.io```), and desired environment variables.

Here is an example of our settings (based on the ```package.json``` file inside our project):

**Project**

Github repository: https://github.com/agility-game/home

**Domain**

***Subdomain***: agility-game<br/>
***Domain***: bohr.io

**Build & Development**

Set the build and development commands for your project.

**FRAMESET PRESET**: ```leave blank```

**BUILD COMMAND**: ```npm run build```

**ROOT DIRECTORY**: ```leave blank```

**OUTPUT DIRECTORY**: ```leave blank```

**INSTALL COMMAND**: ```npm install```

**DEVELOPMENT COMMAND**: ```next dev --port $PORT```

**Environment variables**

Set environment variables for your build script and add-ons.

| name | value | secret |
| -- | -- | -- |
| BOHR_WEB_ADAPTER | 1 | |
| BOHR_WEB_ADAPTER_TYPE | nextjs ||
| DATABASE_URL | postgres://boemekeld:kXfwz4NJAgl7@ep-super-term-409322.us-east-2.aws.neon.tech/neondb?sslmode=require | |
| EMAIL_HTTP_HOST | localhost | |
| EMAIL_HTTP_PORT | 1080 | |
| EMAIL_SMTP_HOST | localhost | |
| EMAIL_SMTP_PORT | 1025 | |
| POSTGRES_DB | neondb | |
| POSTGRES_HOST | ep-super-term-409322.us-east-2.aws.neon.tech | |
| POSTGRES_PASSWORD | kXfwz4NJAgl7 | X |
| POSTGRES_PORT | 5432 | |
| POSTGRES_USER | boemekeld | |
| VERCEL_ENV | 1 | |
| WEBSERVER_HOST | localhost | |
| WEBSERVER_PORT | 3000 | |

**WARNING**: Make sure your latest changes to your Github repository have been committed and pushed to your Github repository should you have edited remotely (such as in GitPod) before continuing.

Finally, click **IMPORT**.

**TIP**: In case the import would fail, you can manually install bohr npm package on the repository as follows:

```
$ git clone https://github.com/agility-game/home.git
$ cd home/my-app
$ npx -y bohr@latest dev
```

**NOTE**: It is important that the bohr package gets installed **inside** your ```my-app``` directory, so **not** in the root of the repository outside of the app directory!

**Commit you changes to the repository after the install of bohr!!**

There you go. 

Now, bohr.io will be installed in your GitHub repository, and your project will be deployed on bohr.io (here at: ```agility-game.bohr.io```). 

Once it's finished, your project will already be live and ready to be accessed (here at: https://agility-game.bohr.io). 

Now, you can edit your code (go to https://bohr.io/agility-game/agility-game-home)) and take advantage of bohr.io’s CI/CD along with GitHub Actions for automatic deployments of your changes.
