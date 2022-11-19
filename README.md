## potential-eureka
Angular client application with .Net Core API and sqlite database

### NuGet Packages
* Run `dotnet restore` to restore Packages
* Install `NuGet Gallery` VS Code extension 
  * Can then use `Open NuGet Gallery` to browse packages

### .NET CLI (.NET Core v6.x)
* `dotnet {cmd} -h` for list of commands available
* `dotnet new -l` for list of templates available
* `dotnet new sln` to create a new solution file
* `dotnet new webapi -o {dirname}` to create a new ASP.NET Core Web API in the given directory
* `dotnet sln add {dirname}` to add the project in that directory to the solution
* `dotnet dev-certs https --trust` to trust your local HTTPS development certificate

#### NuGet Packages Installed
* `Microsoft.EntityFrameworkCore` and install the appropriate version to `API.csproj`
* `Microsoft.EntityFrameworkCore.Sqlite` and install to `API.csproj`
* `Microsoft.EntityFrameworkCore.Design` and install the appropriate version to `API.csproj`

### Entity Framework
* Run `dotnet tool install --global dotnet-ef` to install Entity Framework tooling
* Run `dotnet clean` before running `dotnet ef database update`
* Go to https://www.nuget.org/packages/dotnet-ef to get the command to install the `dotnet-ef` package
  *  Ex: `dotnet tool install --global dotnet-ef --version 7.0.0`

#### Create EF Migrations
* In the "API" folder run `dotnet ef migrations add InitialCreate -o Data/Migrations`
  * Will need `Microsoft.EntityFrameworkCore.Design` installed to run this command
 
### VS Code Extensions
* C# by OmniSharp (run >NET: Generate assets for build and debug)
* C# Extensions
* SQLite
