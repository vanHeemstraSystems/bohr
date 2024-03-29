# 300 - Using the terminal

You can use the terminal to create and publish projects on the platform. You can also use the terminal locally or the terminal available within bohr.io.

In this example, we'll create a Svelte project and name it "my-app". See [Creating a Project in Svelte](https://kit.svelte.dev/docs/creating-a-project) then type "npm create svelte@latest my-app" and set your preferences. The project will then be initialized automatically.

```
wvanheemstra@bohr.io:/app $ npm create svelte@latest my-app
```

For the options offered, choose:

- Which Svelte app template: Skeleton project
- Add type checking with TypeScript?: Yes, using TypeScript syntax
- Select additional options (use arrow keys/space bar):
  - Add ESLint for code linting
  - Add Prettier for code formatting
  - Add Playwright for browser testing
  - Add Vitest for unit testing

Now, navigate to your new Svelte project folder by typing:

```
$ cd my-app
```

To install and run the development environment you can optionally type the following:

```
npm install
npm run dev
```
