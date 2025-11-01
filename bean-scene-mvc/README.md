# Bean Scene MVC Reservation System

A role-based restaurant reservation system built with C# and ASP.NET Core MVC. It supports authentication, staff roles, and persistent data storage using Entity Framework Core.

---

## 🛠 Technologies

- **Language**: C#
- **Framework**: ASP.NET Core MVC (.NET 8)
- **Authentication**: ASP.NET Identity
- **ORM**: Entity Framework Core (EF Core)
- **Database**: SQLite or SQL Server

### Key NuGet Packages

- `Microsoft.AspNetCore.Identity.EntityFrameworkCore` 8.0.8  
- `Microsoft.EntityFrameworkCore.Sqlite` / `SqlServer` 8.0.8  
- `Microsoft.EntityFrameworkCore.Tools` 8.0.8  
- `Microsoft.AspNetCore.Identity.UI` 8.0.8  

---

## ✨ Features

- 🔐 User authentication with role-based access control
- 👤 Predefined roles: **Admin**, **Manager**, **Staff**
- 📋 Reservation and user management interfaces
- 💾 SQLite or SQL Server support via EF Core

---

## 🚀 Getting Started

### ✅ Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- SQLite or SQL Server

### ⚙️ Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/z-evm/bean-scene-mvc.git
   cd bean-scene-mvc
   ```

2. **Configure the database**

   Update `appsettings.json` with your connection string:

   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;User ID=YOUR_USER;Password=YOUR_PASSWORD;TrustServerCertificate=True"
   }
   ```

   Or use the included SQLite configuration.

3. **Apply database migrations**

   ```bash
   dotnet ef database update
   ```

4. **Run the application**

   ```bash
   dotnet run
   ```

---

## 👥 Default User Accounts

These are seeded during first-time setup:

| Role    | Email                                                 | Password |
|---------|-------------------------------------------------------|----------|
| Admin   | [admin@beanscene.com](mailto:admin@beanscene.com)     | password |
| Manager | [manager@beanscene.com](mailto:manager@beanscene.com) | password |
| Staff   | [staff@beanscene.com](mailto:staff@beanscene.com)     | password |

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
