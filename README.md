# Angular2Setup
Basic Angular 2 Setup for Visual Studio Code / Visual Studio 2017 (CSPROJ based)

# Requirements to continue
<ol>
<li>The .Net Core SDK. This project was built using the <a href="https://go.microsoft.com/fwlink/?LinkID=835014">.Net Core 1.1 64-bit SDK</a>.</li>
<li><a href="https://github.com/dotnet/core/blob/master/release-notes/rc3-download.md">The .Net Core SDK 1.0 RC3 Tools</a></li>
<li><a href="https://www.npmjs.com/">NPM</a>... Well, duh.</li>
<li>The TypeScript Compiler (tsc): <ul><li><b>npm install -g typescript</b></li></ul></li>
<li><i>Recommended install of Bower</i>: <ul><li><b>npm install -g bower</b></li></ul></li>
</ol>

# Using This Project
<ol>
<li>Clone this project and open the folder Angular2Setup in Visual Studio Code.</li>
<li>Right click Program.cs in the folder and select "Open in Command Prompt".</li>
<li>Run the command "dotnet restore".</li>
<li>Build using Shift+B.</li>
<li>Debug using F5.</li>
<li>Navigate to http://localhost:5000/index.html and Angular2 page should display.</li>
</ol>

# Why make this project?
This is a standard template for Angular 2 in Visual Studio Code (or Visual Studio 2017) using the Visual Studio's RC3 tooling. Projects are now based on .csproj files instead of project.json.

In addition, Visual Studio Code supports a number of tasks. This project automatically has a task to run tsc (TypeScript compiler) when running the application in debug. This also watches for changes in TS files and updates JS files for the browser when changes are made.

Occasionally the task runs even after stopping, which prevents you from making certain changes. You can force-end the task easily in VS Code when prompted to stop the running tasks.
