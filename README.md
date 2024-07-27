# 🌅 Sunrise - osu! private server

Sunrise is a private server for osu! written in C#. This repository has both endpoints for game-client and for the website. The server is currently in development and is not yet ready for public use.

> [!NOTE]
> Why C#? Well, because owner of this project has allergies to non-typed languages. Sad, I know.

## Installation 📩

1. Clone the repository
2. Open the project in Visual Studio (or any other IDE)
3. Run the project
4. (Optional) Forward osu! traffic to your local server using a tool like [Fiddler](https://www.telerik.com/fiddler)

## File structure 📂

```
Sunrise/
├── bin/               # Compiled files
├── Properties/        # Project properties
├── Database/          # Files (SQLite with c# classes)
├────── Files/         # Files stored in the  (e.g. avatars, beatmaps, backgrounds)
├────── Schemas/       # Database schemas
├── GameClient/        # Game client logic (e.g. c.ppy.sh, a.ppy.sh, osu.ppy.sh requests)
├────── Controllers/   # Game client controllers - Endpoints for game client
├────── Handlers/      # Game client handlers - Handlers for controllers (e.g. login, register)
├────── Helpers/       # Game client helpers - Helper classes for game client
├────── Objects/       # Game client objects - Objects used in game client (e.g. session, location)
├────── Repositories/  # Game client repositories - Right now contains SessionRepository for all user's sessions
├────── Services/      # Game client services - Microservices for game client
├────── Types/         # Game client types
├── WebServer/         # Website logic (e.g. API calls)
├────── Controllers/   # Website controllers (endpoints)
├────── Services/      # Website services (e.g. user service)
├── Utils/             # Utility classes (e.g. parsers, decoders)
├── Sunrise.csproj     # Project file
```

> [!WARNING]
> Project in early development stage. File structure may change in the future.

## API Endpoints 🛜

### Locally

All endpoints can be checked after running the server locally by navigating to `http://localhost:{your-port}/swagger/index.html`.

### Server

In the near future, the server will be hosted on a domain and the API documentation will be available there.

## Contributing 💖

If you want to contribute to the project, feel free to fork the repository and submit a pull request. We are open to any suggestions and improvements.
