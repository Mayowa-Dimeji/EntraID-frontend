# 🔐 EntraFrontend (Blazor WebAssembly + Microsoft Entra External ID)

This is a minimal Blazor WebAssembly frontend integrated with **Microsoft Entra External ID** to support secure user authentication using **social login providers** (e.g., Google).

---

## 🚀 Features

- 🔑 Secure login flow via Microsoft Entra External ID
- 🌐 Supports federated social logins (Google, Facebook, etc.)
- 📦 Built with .NET 8 + Blazor WebAssembly
- 🧠 MSAL (Microsoft Authentication Library) integration
- 🔄 Access tokens available for calling protected APIs

---

## 🛠️ Tech Stack

| Layer             | Technology                                                 |
| ----------------- | ---------------------------------------------------------- |
| Language          | C# (.NET 8)                                                |
| Framework         | Blazor WebAssembly                                         |
| Identity Provider | Microsoft Entra External ID (OAuth2/OIDC)                  |
| Auth Library      | Microsoft.AspNetCore.Components.WebAssembly.Authentication |
| Hosting (Dev)     | ASP.NET Core Dev Server                                    |

---

## ⚙️ Setup

1. Make sure the **redirect URI** is registered in Azure:

   ```
   http://localhost:5208/authentication/login-callback
   ```

2. Run the project:

   ```bash
   dotnet run
   ```

3. Open in browser:
   ```
   http://localhost:5208
   ```

---

## 💡 Notes

- This app uses `RemoteAuthenticatorView` for handling login, logout, and token handling.
- After successful login, users are issued an **access token** which can be sent to your Azure Functions backend.

---

## 📬 Contact

Built by Mayowa Oladimeji  
[LinkedIn](https://linkedin.com/in/mayowa-oladimeji/)

---

## 📝 License

MIT — open for use, contributions welcome.
