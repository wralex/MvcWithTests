# MvcWithTests

.NET MVC Web Project with Unit testing a Functional Testing components

Steps:

1. Create a Repository with Source Control
2. Clone repository to a local folder to use for the project
3. Open Terminal window to the root folder of project on system
4. In the Terminal window execute the following commands:

    ``` powershell
    mkdir src\web
    cd .\src\web\
    mkdir MvcWeb
    cd .\MvcWeb\
    dotnet new mvc
    cd ..\..\..
    mkdir tests
    cd .\tests\
    mkdir unit
    mkdir selenium
    mkdir inter
    cd .\unit\
    mkdir MvcUnit
    cd .\MvcUnit\
    dotnet new xunit
    cd ../..
    cd .\inter\
    mkdir MvcInter
    cd .\MvcInter\
    dotnet new nunit
    cd ..\..\..
    dotnet new sln --name "MvcSolution"
    dotnet sln add (ls -r **/*.csproj)
    dotnet add tests/unit/MvcUnit/MvcUnit.csproj reference src/web/MvcWeb/MvcWeb.csproj
    ```

5. Open the project in Visual Studio by double-clicking the `MvcSolution.sln` file.
6. On all projects right-clicking each and update any/all dependent NuGet package.
7. On the Web Project add the following Dependancies:
   - [MarkDig](https://github.com/xoofx/markdig)
   - [Westwind.AspNetCore.Markdown](https://github.com/RickStrahl/Westwind.AspNetCore.Markdown)
8. On Web project do the following:
   1. Add the following Dependancies:
      - [MarkDig](https://github.com/xoofx/markdig)
      - [Westwind.AspNetCore.Markdown](https://github.com/RickStrahl/Westwind.AspNetCore.Markdown)
   2. Right click on project and click `Manage Client-Side Libraries...`. (This will all 'libman.json' to the project)
   3. 
   4. 
9.  