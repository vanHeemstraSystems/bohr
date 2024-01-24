# 100 - Example of using a template

Create a dummy repository in GitHub to host the new to be created project. We name it ```bohr-test``` at https://github.com/agility-game/bohr-test.git.

Select ```tabnews.com.br``` from the projects templates page at https://bohr.io/projects. This template can be viewed for details at https://github.com/bohr-io/tabnews.com.br.

When asked to authorize Bohr.io towards your GitHub repository, follow the instructions provided on screen.

You will be prompted with a form called **New Project** at https://bohr.io/createRepository?sampleUrl=https://github.com/bohr-io/tabnews.com.br

Enter the variables as below:

**Template**

name: tabnews.com.br<br/>
GitHub repository: https://github.com/bohr-io/tabnews.com.br

**Domain**

Subdomain: ```bohr-test```<br/>
Domain: ```bohr.io```

**NOTE**: You have the option here to create a private Git repository, instead of using our dummy repository. Leave it blank this this case.

**Build & Development**

Set the build and development commands for your project.

BUILD COMMAND: ```npm run build```

ROOT DIRECTORY: ```leave blank```

OUTPUT DIRECTORY: ```leave blank```

INSTALL COMMAND: ```npm install```

DEVELOPMENT COMMAND: ```next dev --port $PORT```

**Environment Variables**

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

Follow by clicking the button **PUBLISH**.

The first time, you will be prompted as follows:

```
PERMISSION ERROR

We need repository permission to publish in your organization
```

Click the button **GO TO GITHUB**

In the GitHub dialog Grant access to ```agility-game``` and click the button **Authorize bohr-io**.

Your will be prompted as follows:

```
Sorry! We need some permissions first!

We ask you to install and authorize our app within your GitHub account so bohr.io can give to you all the power for creating and launching your projects its deploys and more. By clicking the button below, you'll see the screen aside, follow the instructions and happy deploying!
```

Click the button **INSTALL & AUTHORIZE**



