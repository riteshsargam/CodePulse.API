# CodePulse.API

Welcome to **CodePulse.API**, a blog website built using ASP.NET Core. This repository houses the back-end API for a dynamic blogging platform that allows users to create, edit, and manage their blogs easily. This project leverages ASP.NET Core's capabilities to deliver a robust, scalable, and performant API.

## Features

- **User Authentication**: Secure user registration and login functionality.
- **Blog Management**: CRUD operations for blog posts.
- **Comments System**: Users can leave comments on blog posts.
- **Tagging**: Support for tagging blog posts to categorize content.
- **Search Functionality**: Easily search for posts using keywords.

## Prerequisites

- [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) or any compatible database
- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or any preferred IDE

## Getting Started

To get a local copy up and running, follow these steps:

### Clone the repository

```bash
git clone https://github.com/riteshsargam/CodePulse.API.git
cd CodePulse.API
```

### Set up the database

1. Configure your database connection string in `appsettings.json`.

```json
{
"ConnectionStrings": {
"DefaultConnection": "Your Database Connection String"
}
}
```

2. Run EF Core migrations to set up the database schema:

```bash
dotnet ef database update
```

### Build and run the application

1. Restore the NuGet packages and compile the project:

```bash
dotnet build
```

2. Run the application:

```bash
dotnet run
```

The API will be available at `https://localhost:5001`.

## API Endpoints

Here's a brief overview of some of the key API endpoints:

- **Authentication**
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Authenticate a user

- **Blog Posts**
- `GET /api/posts` - Retrieve all blog posts
- `GET /api/posts/{id}` - Retrieve a single blog post by ID
- `POST /api/posts` - Create a new blog post
- `PUT /api/posts/{id}` - Update a blog post
- `DELETE /api/posts/{id}` - Delete a blog post

- **Comments**
- `GET /api/posts/{postId}/comments` - Retrieve comments for a blog post
- `POST /api/posts/{postId}/comments` - Add a comment to a blog post

## Contributing

Contributions are welcome! If you have suggestions for improvement or new features, feel free to fork the repository and submit a pull request. Please ensure your contributions align with the project's coding standards and practices.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please reach out through the repository's GitHub issues section.

---

Thank you for checking out CodePulse.API! We hope you find it useful and a solid starting point for your ASP.NET Core projects.
```
