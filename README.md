# Postify

A knowledge-sharing platform where users publish posts, comment, vote and join discussions, with content organized by tags and categories. Built during my internship at IDS.

## Features

- Sign up, sign in and author pages
- Create and edit posts
- Comments and votes
- Categories, tags and search
- Notifications

## Tech stack

- **Backend:** ASP.NET Core (.NET 8), Entity Framework Core, AutoMapper, Swagger
- **Database:** SQL Server
- **Frontend:** HTML, CSS, JavaScript, Material Kit (Bootstrap)

## Project structure

```
serverside/   REST API: Controllers, Data, Mappings, Migrations, Models/DTOs
clientside/   Static front-end pages and assets
```

## Getting started

You'll need the .NET 8 SDK, the `dotnet-ef` tool and SQL Server.

1. Set the connection string in `serverside/appsettings.json` to point at your SQL Server instance.
2. Create the database and start the API on `https://localhost:7069`, which is the address the front end calls:
   ```bash
   cd serverside
   dotnet ef database update
   dotnet run --launch-profile https
   ```
3. Open `clientside/index.html` in your browser.
