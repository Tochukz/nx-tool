# Nx
[Docs](https://nx.dev/docs/getting-started/intro)  

## Introduction
You can run your `npm` script using `nx`
```bash
$ nx build nest-app
```
This will run the `build` script as defined in the `package.json` of  the `nest-app` project.  

__Common Commands__  

Description       | Command
------------------|-------------------
Run multiple apps |  `nx run-many -t serve -p app1 app2`
Run multiple app (Alt) | `nx run-many --target=serve --projects=app1,@org/app2`
Run apps on native terminal | `NX_TUI=false nx run-many --target=serve --projects=app1,app2`
Reset | `nx reset`



## Quick Start
1. __Installation__  

You can install the `nx` CLI tool globally which is optional, or you can just run `nx` using `npx`.  
Let install it globally:
For MacOS
```bash
$ brew install nx
```

For Windows
```batch
> choco install nx
```

2. __Starting Nx project__   

Starting with a new project
```bash
$ npx create-nx-workspace@latest
# Follow the prompt, choose a starter workspace template.
# I choose React monorepo
```

Or adding to an existing project
```bash
$ npx nx@latest init
```

3. __Operate applications__
```bash
$ nx build my-app
$ nx test my-lib
```

4. __Server an application__  
```bash
$ nx serve shop
```
You can then go onto the application URL such as `http://localhost:4200/` to see the app in action.  

5. __Checkout application project details__
```bash
$ nx show project shop
```
