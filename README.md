# 🍔 Food Delivery System — Backend

A robust backend system for an online food delivery platform, built with **C#** and **ASP.NET**. This project handles the core business logic, data management, and server-side operations required to power a full-featured food ordering and delivery service.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)

---

## Overview

The Food Delivery System Backend provides the server-side infrastructure for managing users, restaurants, menus, orders, and deliveries. It is designed to serve as the API and business logic layer for a food delivery web or mobile application — similar in scope to platforms like Swiggy or Zomato.

Key goals of this project:
- Enable customers to browse restaurants and place food orders online
- Allow restaurant administrators to manage menus and incoming orders
- Track orders through the full lifecycle (placed → preparing → out for delivery → delivered)
- Support secure user authentication and role-based access

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | C# |
| Framework | ASP.NET |
| IDE | Microsoft Visual Studio |
| Database | SQL Server (MS SQL) |
| Solution Format | `.sln` (Visual Studio Solution) |

---

## Features

**Customer**
- User registration and login
- Browse restaurant listings and menus
- Add items to cart and place orders
- Choose between online payment and cash on delivery
- View order status and history

**Restaurant / Admin**
- Manage food items, categories, and pricing
- View and process incoming orders
- Update order status in real time
- Generate delivery reports (daily/weekly/monthly)

**System**
- Role-based access control (Customer, Restaurant, Admin)
- Secure authentication
- Order lifecycle management
- Database-backed persistence for all entities

---

## Project Structure

```
Food-Delivery-System-Backend/
├── Online food delivery system/     # Main C# project directory
│   ├── Controllers/                 # Request handlers and API logic
│   ├── Models/                      # Data models (User, Order, MenuItem, etc.)
│   ├── Data/                        # Database context and migrations
│   ├── Services/                    # Business logic layer
│   └── ...
├── Online food delivery system.sln  # Visual Studio solution file
└── README.md
```

---

## Getting Started

### Prerequisites

- [Visual Studio 2019 or later](https://visualstudio.microsoft.com/) with the **ASP.NET and web development** workload
- [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) (or SQL Server Express)
- .NET Framework / .NET SDK (version as required by the project)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/BinoyBabu10/Food-Delivery-System-Backend.git
   cd Food-Delivery-System-Backend
   ```

2. **Open the solution in Visual Studio**
   ```
   File → Open → Project/Solution → Online food delivery system.sln
   ```

3. **Configure the database connection**

   Update the connection string in `Web.config` or `appsettings.json` to match your local SQL Server instance:
   ```xml
   <connectionStrings>
     <add name="DefaultConnection"
          connectionString="Server=YOUR_SERVER_NAME;Database=FoodDeliveryDB;Integrated Security=True;" />
   </connectionStrings>
   ```

4. **Set up the database**

   Run the provided SQL scripts (if any) or use Entity Framework migrations:
   ```
   Tools → NuGet Package Manager → Package Manager Console
   PM> Update-Database
   ```

5. **Run the project**

   Press **F5** or click the **Run** button in Visual Studio. The application will launch in your default browser.

---

## Usage

Once running, the system exposes endpoints/pages for:

- **`/register`** — Create a new customer account
- **`/login`** — Authenticate and log in
- **`/menu`** — Browse food items and restaurants
- **`/cart`** — Manage your order cart
- **`/orders`** — Place and track orders
- **`/admin`** — Admin dashboard for restaurant and order management

---

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to fork the repository and submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## Author

**Binoy Babu**
[GitHub Profile](https://github.com/BinoyBabu10)

---

*Built as part of a backend development project demonstrating C# / ASP.NET skills in designing and implementing a real-world food delivery platform.*
