# Graduation Project — Social Platform API

An **ASP.NET Core Web API** serving as the backend of a graduation project social platform — with real-time messaging via SignalR, JWT authentication, user profiles, photo management, and a threading/gallery system.

## What it does

A social networking backend built for a graduation project. Users can register, build profiles with photos, send real-time messages, and interact through threads and galleries. SignalR powers live presence and messaging features.

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
2. Apply migrations and seed data:
   ```bash
   dotnet ef database update
   dotnet run
   ```
