# PicoServer
![2f4c1767266451.png](https://picoserver.cn/content/uploadfile/202601/c5481768225502.png)

**[简体中文](README.md)|[English](README.en.md)**



### 🛠️ What is PicoServer?
> PicoServer is a **lightweight web request glue library** for the .NET ecosystem, focusing on "integration first, flexible embedding". It can be directly embedded into any .NET application to quickly build Web APIs.

> It runs without relying on IIS or Kestrel, out of the box with zero configuration, and requires no modification to existing business code. Whether you need a lightweight Web API, WebSocket real-time communication, edge computing web service, or a lightweight streaming media server, PicoServer is the perfect fit.

### ❤️ **Let's Call It "Pika"**

> It's exciting💥 to come up with this Chinese nickname. Pika, let's go!

### Implement a Web API in One Line of Code
**C#**
```csharp
MyAPI.AddRoute("/hello", async (req, resp) => await resp.WriteAsync(@"{""code"":1,""msg"":""Hello PicoServer WebAPI""}"));
```

**VB.NET**
```vb
MyAPI.AddRoute("/hello", Function(req, resp) resp.WriteAsync(<t>{"code":1,"msg":"Hello PicoServer WebAPI"}</t>.Value))
```

| [Quick Start](https://picoserver.cn/quikstart.html "Quick Start") | [C# Samples](https://picoserver.cn/usage-csharp.html "C# Samples") | [VB.NET Samples](https://picoserver.cn/usage-vbnet.html "VB.NET Samples") | [Performance Test](https://picoserver.cn/benchmark.html "Performance Test") | [Secondary Development](https://picoserver.cn/developer.html "Secondary Development") |
| :------------: | :------------: | :------------: | :------------: | :------------: |

### ✨ Key Features of PicoServer

📦 **Ultra-Small Size**: Single DLL is only 60kb, **zero third-party dependencies**, extremely lightweight.
💡 **Minimal Learning Curve**: **[Install PicoServer via NuGet](https://picoserver.cn/quikstart.html "Install PicoServer via NuGet")**, then add one route to build a Web API.
🔗 **Flexible Compatibility**: Its **glue feature** integrates seamlessly with other libraries, no need to modify business code in legacy projects.
🛡️ **Out-of-the-Box Capabilities**: Built-in default routing, simple Token validation, and JWT validation to cover most basic scenarios.
🚀 **Blazing Fast Performance**: Full asynchronous non-blocking architecture, native AOT compilation support, millisecond-level startup, ideal for various gateways.
🌍 **Cross-Platform Support**: Developed based on .NET Standard 2.0, compatible with .NET Framework 4.6.1+, .NET Core/5/6+, and runs on Linux, Windows, and macOS.
✨ **Highly Extensible**: Achieve secondary development easily through custom `AddRoute` (routing) and `AddMiddleware` (middleware) to unlock more advanced features.

---

### 🎯 When to Choose PicoServer?
Choose **PicoServer**, the **glue library**, if your requirements match any of the following:

* **Need to add APIs to an existing application**: For example, adding Web API support to console apps, desktop applications, or Windows services.
* **Pursue "ultimate transparency"**: You want every line of processing logic (middleware/routing) to be visible, rather than hidden in a black box.
* **Resource-constrained environments**: Every megabyte of memory counts in industrial PCs, edge devices, or MCP (AI assistant integration) scenarios.
* **Pure stream processing**: Need to build simple file upload/download services, video stream forwarding, or intranet penetration gateways.

---

### 🧰 Three Core Capabilities: Embed on Demand, Empower Flexibly
**Don't limit your imagination by its 60kb lightweight size**

PicoServer embeds into your application as a library, providing direct web capabilities support that you can call as needed.

1.  **Route Mapping (AddRoute) — Business Entry Point**
    「Precise Request Handling」: As the core entry for web requests, map specific URL requests to your business logic with just a few lines of code, whether returning JSON data or executing business commands, responses are instant.
2.  **Middleware (AddMiddleware) — Request Defense Line**
    「Pre-Request Interception」: Takes effect before requests reach business logic. Quickly integrate identity verification, log auditing, IP filtering, etc. Achieve request interception or release in one step without modifying core business code.
3.  **Extension Capabilities — On-Demand Empowerment**
    「Lightweight Integration」: Thanks to its glue feature, it can be flexibly extended based on the above two capabilities. Embed WebAPI, file download, streaming media forwarding, etc., on demand to easily expand your application's functional boundaries.

---

### 🚀 Start Your Embedded Integration Journey
** Web Connects Everything**
**"PicoServer handles the connection, you focus on the creation."**

> PicoServer is simple and ready to use; it is user-friendly and non-intrusive to business logic; it is flexible and enables simple [secondary development](https://picoserver.cn/developer.html "Secondary Development").

Check out the **[User Guide (C#)](https://picoserver.cn/usage-csharp.html)** or **[User Guide (VB.NET)](https://picoserver.cn/usage-vbnet.html)** now. Start your integration journey with just three lines of code.
