# 🚀 Nuxt 4.2.1 Starter Template

A fully configured **Nuxt 4.2.1** starter project with TailwindCSS v4, TypeScript, ESLint, VueUse, Nuxt DevTools, and more. This repo is ready-to-use for building production-quality Nuxt applications with clean structure and modern tooling.

---

## 📦 Included Dependencies

### **Runtime Dependencies**

```
"@nuxtjs/color-mode": "4.0.0"
"@vueuse/core": "^14.0.0"
"@vueuse/nuxt": "^14.0.0"
"better-sqlite3": "^12.4.1"
"nuxt": "^4.2.1"
"vue": "^3.5.24"
"vue-router": "^4.6.3"
```

### **Dev Dependencies**

```
"@antfu/eslint-config": "^6.2.0"
"@nuxt/devtools": "^3.1.0"
"@nuxt/eslint": "^1.10.0"
"@tailwindcss/vite": "^4.1.17"
"eslint": "^9.39.1"
"tailwindcss": "^4.1.17"
"typescript": "^5.9.3"
```

---

## 📁 Project Structure

```
├── app.vue
├── nuxt.config.ts
├── pages/
├── components/
├── layouts/
├── server/
├── plugins/
├── public/
├── assets/
└── package.json
```

---

## ⚙️ Features & Setup Details

### ✅ Nuxt 4.2.1

Latest Nuxt version with hybrid rendering, islands architecture, and enhanced dev experience.

### 🎨 TailwindCSS 4 (via Vite plugin)

Fully configured utility-first styling with zero setup.

### 🌙 Color Mode

Dark/Light mode support via `@nuxtjs/color-mode`.

### 🧰 VueUse + VueUse Nuxt

Hundreds of powerful composables already integrated.

### 🐘 SQLite Support

`better-sqlite3` for server-side database usage.

### 🛠 ESLint (Antfu Config)

Modern ESLint setup with opinionated rules.

### 🧪 TypeScript

Type safety, auto imports, and seamless DX.

---

## 🚀 Getting Started

### 1️⃣ Install Dependencies

```bash
pnpm install
# or
npm install
# or
yarn install
```

### 2️⃣ Run Development Server

```bash
pnpm dev
```

This starts your Nuxt app at:

```
http://localhost:3000
```

### 3️⃣ Build for Production

```bash
pnpm build
```

### 4️⃣ Preview Production Build

```bash
pnpm preview
```

---

## ⚡ Recommended VS Code Extensions

* TailwindCSS IntelliSense
* Vue Language Features (Volar)
* TypeScript Vue Plugin
* ESLint
* Iconify IntelliSense

---

## 🧩 Included Nuxt Config Basics

Typical `nuxt.config.ts` includes:

```ts
export default defineNuxtConfig({
  css: [],
  modules: [
    '@vueuse/nuxt',
    '@nuxtjs/color-mode',
    '@nuxt/devtools',
  ],
  colorMode: {
    classSuffix: ''
  }
})
```

---

## 📜 License

This project is free to use for personal and commercial development.

---

## 🤝 Contribution

Pull requests and improvements are welcome!

---

## ❤️ Author

Created by **Hussain Ullah** — Fully optimized Nuxt starter template for smooth development.
