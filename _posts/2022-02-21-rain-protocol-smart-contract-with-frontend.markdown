---
layout: single
title:  "Rain Protocol: Smart Contract with Frontend"
date:   2022-02-21 14:00:23 +0000
categories: various
---

## Setting Up the Environment

For this project, we will use [Hardhat][hardhat], which is a popular tool that describes itself as "A development environment to compile, deploy, test, and debug your Ethereum software". [Click here][hardhat] to read more about the tool.

We will not go into too much detail here about how to set up new `npm` based repositories, but, in order to get started, we will create a new directory and run `npm init` to create a `package.json` file which will contain the list of dependencies which our project will use.

After running the command, and selecting the default options, your `package.json` file should look something like this:

```
{
  "name": "example",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}
```

Next we will add hardhat by running `npm install --save-dev hardhat`

## Creating an example

We will now create a basic hardhat project using `npx`. Npx should come bundled with `npm` and is basically [`a CLI tool whose purpose is to make it easy to install and manage dependencies hosted in the npm registry.`][npx]. If we run `npx hardhat` we will then create a basic Hardhat project in our project folder (select the `sample project` option for now). You can read more about this process [here][hardhat]. Running `npx hardhat` again will give a list of available options which can be used with the tool. You will probably want to select `yes` to the `add .gitignore` option, especially if you are considering creating a git repo of your project. You can do this by running `git init` at this point. Details on how to use git are beyond the scope of this tutorial, but to get started, you can run `git add .` (which will add everything in the current directory EXCEPT everything in `.gitignore` to your repo), and then `git commit --message "My First Commit"`.



[discord]: https://discord.gg/dzYS3JSwDP
[hardhat]: https://hardhat.org/getting-started/
[npx]: https://www.freecodecamp.org/news/npm-vs-npx-whats-the-difference/