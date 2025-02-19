---
name: walkthrough-jsscreate
routeTemplate: ./data/component-templates/article.yml
title: Walkthrough with `jss create`
---
# Walkthrough: Using the JSS CLI to Get Started with JSS and Next.js 

You can create a JSS Next.js application by using the JSS command-line tool (CLI). 

> When using this approach, you will need to perform additional steps to connect to a Sitecore instance.

We recommend this approach for Sitecore developers who use the [code-first developer workflow](/docs/fundamentals/dev-workflows/code-first) or wish to evaluate the JSS developer experience without installing Sitecore.

## TL;DR

To quickly scaffold a JSS Next.js application with default configuration, run the following commands in a terminal:

```
npm install -g @sitecore-jss/sitecore-jss-cli
jss create my-first-jss-app nextjs
cd my-first-jss-app
jss start
```

> To ensure that your new JSS application is compatible with your licensed Sitecore XP version, consult the [compatibility table](https://support.sitecore.com/kb?id=kb_article_view&sysparm_article=KB0541788). 
> 
> To create an application using a previous version of JSS, see an example in the [JSS CLI reference](/docs/fundamentals/cli).

##  Create your application

To create a JSS application, you must: 

1. Install  [Node.js](https://nodejs.org/).

2. Install the JSS CLI: 

   ```
   npm install -g @sitecore-jss/sitecore-jss-cli
   ```

   > To verify the successful installation of the JSS CLI and to see the list of commands availability globally, run `jss --help`.

3. Run:

   ```
    jss create my-first-jss-app nextjs [--fetchWith {REST|GraphQL}] [--prerender {SSG|SSR}]
   ```

   The command will create the JSS Next.js application and install the required packages. 
   
   > For more information on `jss create` see [the JSS CLI reference](/docs/fundamentals/cli).
    

   
   > To ensure that your new JSS application is compatible with your licensed Sitecore XP version, consult the [compatibility table](https://support.sitecore.com/kb?id=kb_article_view&sysparm_article=KB0541788).  
   > 
   > To create an application using a previous version of JSS, see an example in the [JSS CLI reference](/docs/fundamentals/cli).

## Run your application

To run your application: 

1. In the terminal, go to your application directory. For example: `cd my-first-jss-app`.

2. Run `jss start`.

   > To see the full list of commands available for your application, run `jss --help`.

## Connect to Sitecore

Deploying your code-first artifacts and content to Sitecore, WYSIWYG editing, and use of JSS in production will require a Sitecore instance.

Sitecore requires Windows, but the instance can be on a virtual machine or a remote server. 

To connect your application to Sitecore, you must:

1. [Setup JSS Server Components](/docs/client-frameworks/getting-started/jss-server-install).
2. [Deploy the application to a Sitecore environment](/docs/client-frameworks/getting-started/app-deployment).
3. [Connect to the Experience Editor](/docs/nextjs/experience-editor/walkthrough).
