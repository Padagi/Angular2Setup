# Angular2Setup
Basic Angular 2 Setup for Visual Studio Code / Visual Studio 2017 (CSPROJ based)

# Required and Recommended Installations
<ol>
<li>The .Net Core SDK. This project was built using the <a href="https://go.microsoft.com/fwlink/?LinkID=835014">.Net Core 1.1 64-bit SDK</a>.</li>
<li><a href="https://github.com/dotnet/core/blob/master/release-notes/rc3-download.md">The .Net Core SDK 1.0 RC3 Tools</a></li>
<li><a href="https://www.npmjs.com/">NPM</a>... Well, duh.</li>
<li>The TypeScript Compiler (tsc): <ul><li><b>npm install -g typescript</b></li></ul></li>
<li><i>Recommended install of Bower</i>: <ul><li><b>npm install -g bower</b></li></ul></li>
</ol>

# Using This Project (with Windows Shortcuts)
<ol>
<li>Clone this project and open the folder Angular2Setup in Visual Studio Code.</li>
<li>In VS Code open the Command Prompt using the <b>CTRL+`</b> shortcut.</li>
<li>Run the command <b>dotnet restore</b>.</li>
<li>Run the command <b>npm install</b>.</li>
<li>Build the project using the <b>Shift+B</b> shortcut.</li>
<li>Debug the application using <b>F5</b> shortcut.</li>
<li>Open Chrome (or any browser) and navigate to http://localhost:5000/index.html and the basic Angular 2 page should display.</li>
</ol>

# Why the heck did you make this project?
This is a standard template for Angular 2 in Visual Studio Code (or Visual Studio 2017) using the .Net Core SDK 1.0 RC3 tooling. Projects using the updated tools are now based on .csproj files instead of project.json files.

In addition, Visual Studio Code uses a Task Runner for building and other items. This project automatically has a task to run tsc (the TypeScript compiler) when running the application in debug. This also watches for changes in TS files and updates JS files in the browser automatically when code changes are made (TS is compiled into JS and then refreshing page shows the changes).

Occasionally the task runs even after stopping, which prevents you from making certain changes. You can force-end the task easily in VS Code when prompted to stop the running tasks.
