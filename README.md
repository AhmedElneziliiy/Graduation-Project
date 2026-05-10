# Graduation Project — Social Platform API

An **ASP.NET Core Web API** serving as the backend of a social platform graduation project — with real-time messaging via SignalR, JWT authentication, user profiles, photo management, and a threading/gallery system.

## Tech Stack

- **ASP.NET Core Web API** (.NET)
- **Entity Framework Core** — SQL Server
- **ASP.NET Identity** — JWT authentication with roles
- **SignalR** — presence hub and message hub for real-time communication
- **Cloudinary** — photo storage
- **AutoMapper**

## Key Features

- User registration and JWT-based login
- Member profiles with photo galleries
- Real-time private messaging (SignalR `MessageHub`)
- Online presence tracking (SignalR `PresenceHub`)
- Thread system for user interactions
- Admin and Moderator role support

## Getting Started

1. Update `appsettings.json` with:
   - SQL Server connection string
   - JWT secret key
   - Cloudinary credentials (`CloudName`, `ApiKey`, `ApiSecret`)
2. Apply migrations: `dotnet ef database update`
3. Run: `dotnet run`
