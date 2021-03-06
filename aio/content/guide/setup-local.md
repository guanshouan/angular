# Setting up the Local Environment and Workspace


This guide explains how to set up your environment for Angular development using the [Angular CLI tool](cli "CLI command reference"). 
It includes information about prerequisites, installing the CLI, creating an initial workspace and starter app, and running that app locally to verify your setup. 


<div class="callout is-helpful">
<header>Learning Angular</header>

If you are new to Angular, see [Getting Started](start). Getting Started helps you quickly learn the essentials of Angular, in the context of building a basic online store app. It leverages the [StackBlitz](https://stackblitz.com/) online development environment, so you don't need to set up your local environment until you're ready. 


</div> 


{@a devenv}
{@a prerequisites}
## Prerequisites 

Before you begin, make sure your development environment includes `Node.js®` and an npm package manager. 

{@a nodejs}
### Node.js

Angular requires `Node.js` version 10.9.0 or later.

* To check your version, run `node -v` in a terminal/console window.

* To get `Node.js`, go to [nodejs.org](https://nodejs.org "Nodejs.org").

{@a npm}
### npm package manager

Angular, the Angular CLI, and Angular apps depend on features and functionality provided by libraries that are available as [npm packages](https://docs.npmjs.com/getting-started/what-is-npm). To download and install npm packages, you must have an npm package manager. 

This setup guide uses the [npm client](https://docs.npmjs.com/cli/install) command line interface, which is installed with `Node.js` by default. 

To check that you have the npm client installed, run `npm -v` in a terminal/console window.


{@a install-cli}

## Step 1: Install the Angular CLI

You use the Angular CLI 
to create projects, generate application and library code, and perform a variety of ongoing development tasks such as testing, bundling, and deployment.

Install the Angular CLI globally. 

To install the CLI using `npm`, open a terminal/console window and enter the following command:


<code-example language="sh" class="code-shell">
  npm install -g @angular/cli

</code-example>



{@a create-proj}

## Step 2: Create a workspace and initial application

You develop apps in the context of an Angular [**workspace**](guide/glossary#workspace). 

To create a new workspace and initial starter app: 

1. Run the CLI command `ng new` and provide the name `my-app`, as shown here: 

    <code-example language="sh" class="code-shell">
      ng new my-app

    </code-example>

2. The `ng new` command prompts you for information about features to include in the initial app. Accept the defaults by pressing the Enter or Return key. 

The Angular CLI installs the necessary Angular npm packages and other dependencies. This can take a few minutes. 

The CLI creates a new workspace and a simple Welcome app, ready to run. 


{@a serve}

## Step 3: Run the application

The Angular CLI includes a server, so that you can easily build and serve your app locally.

1. Go to the workspace folder (`my-app`).

1. Launch the server by using the CLI command `ng serve`, with the `--open` option.

<code-example language="sh" class="code-shell">
  cd my-app
  ng serve --open
</code-example>

The `ng serve` command launches the server, watches your files,
and rebuilds the app as you make changes to those files.

The `--open` (or just `-o`) option automatically opens your browser
to `http://localhost:4200/`.

Your app greets you with a message:


<figure>
  <img src='generated/images/guide/setup-local/app-works.png' alt="Welcome to my-app!">
</figure>


## Next steps


* If you are new to Angular, see the [Getting Started](start) tutorial. Getting Started helps you quickly learn the essentials of Angular, in the context of building a basic online store app. 

  <div class="alert is-helpful">
  
  Getting Started assumes the [StackBlitz](https://stackblitz.com/) online development environment. 
  To learn how to export an app from StackBlitz to your local environment, skip ahead to the [Deployment](start/deployment "Getting Started: Deployment") section. 

  </div>


* To learn more about using the Angular CLI, see the [CLI Overview](cli "CLI Overview"). In addition to creating the initial workspace and app scaffolding, you can use the CLI to generate Angular code such as components and services. The CLI supports the full development cycle, including building, testing, bundling, and deployment. 


* For more information about the Angular files generated by `ng new`, see [Workspace and Project File Structure](guide/file-structure).

