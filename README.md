# Angular SSR Remote App with Module Federation (Angular 15)

This project is a **remote application** built with **Angular 15**, **Angular Universal (SSR)**, and **@angular-architects/module-federation**.

It is designed to **expose Angular components at build time** to other **host applications** using Webpack's Module Federation.

---

## 🚀 Features

- ✅ **Angular 15**
- ✅ **Server-Side Rendering (SSR)** with Angular Universal
- ✅ **Module Federation (Remote App)** via `@angular-architects/module-federation`
- ✅ Exposes components to be consumed by host apps
- ✅ Built-time sharing of Angular modules
- ✅ Express server for SSR

---

🔧 Setup

1. Install dependencies
   npm install

2. build the remote app
   npm run watch

3. run the ssr server
   npm run server

ng new remote
ng add @nguniversal/express-engine
npm run dev:ssr
ng add @angular-architects/module-federation@15 --project remote
ng build --watch
ng run remote:server
npm install cors
node dist/remote/server/main.js
