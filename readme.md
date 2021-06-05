# Text101 project

## Setup Unity with VS Code and intellisense on Linux

- Install extension in vscode `C# extension OmniSharp`

- Install .net SDK from here: https://docs.microsoft.com/es-es/dotnet/core/install/linux-ubuntu#2004-

- Install latest Mono release (Ubuntu 20.04): https://www.mono-project.com/download/vs/

the following line must be changed:

```shell
deb https://download.mono-project.com/repo/ubuntu vs-focal main
```

to this one:

```shell
deb [arch=amd64] https://download.mono-project.com/repo/ubuntu vs-focal main
```

- Open VS Code, go to menu File - Preferences - Settings - Extension - C# configuration, look for "Omnisharp: Use Global Mono", and set it to "always".

- Go to Unity menu Edit - Preferences - External Tools - External Script Editor, and pick "Visual Studio Code"

- In the same window, check "Embedded packages", "Local packages", "Built-in packages", "Git packages" and after click on "Regenerate project files"

## Get the latest gitignore

`.gitignore` file can obtained here

https://raw.githubusercontent.com/github/gitignore/master/Unity.gitignore
