# Wisdom Pet Medicine

This is the **Wisdom Pet Medicine** web application, designed to help manage pets, breeds, species, and owners. The app is built with ASP.NET Core Razor Pages and Entity Framework Core.

## Features

- Manage pets, breeds, species, and owners
- Search and filter pets
- Edit and create pet records
- Responsive UI with Bootstrap

## Getting Started

### Prerequisites

- [.NET 7 SDK](https://dotnet.microsoft.com/download/dotnet/7.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) or VS Code
- Azure account (for deployment)

### Running Locally

1. Clone the repository:

    ```sh
    git clone <your-repo-url>
    cd azure-devops-wisdom-pet-medicine/src/Wpm.Web
    ```

2. Restore dependencies:

    ```sh
    dotnet restore
    ```

3. Run the application:

    ```sh
    dotnet run
    ```

4. Open your browser at [http://localhost:5219](http://localhost:5219) (or the port shown in the console).

### Deploying to Azure

1. Create an **Azure App Service** (Web App) in the Azure Portal.
2. Push your code to an Azure DevOps or GitHub repository.
3. Set up a deployment pipeline (Azure DevOps Pipeline or GitHub Actions) to build and deploy the app to your Azure Web App.
4. Configure your connection strings and environment variables in the Azure Portal as needed.

## Configuration

- App settings are in [`appsettings.json`](Wpm.Web/appsettings.json) and [`appsettings.Development.json`](Wpm.Web/appsettings.Development.json).
- By default, the app uses an in-memory database. For production, update the connection string and use SQL Server.

## Project Structure

- `Wpm.Web/` - Main ASP.NET Core project
  - `Domain/` - Entity models
  - `Dal/` - Data access layer (DbContext and extensions)
  - `Pages/` - Razor Pages (UI)
  - `wwwroot/` - Static files (CSS, JS, images)

## License

This project is licensed under the MIT License.

---

**Ready to deploy to Azure!**