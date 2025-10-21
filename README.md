# ⚡ Vite + Tailwind CSS Setup Guide


### 🧠 A clean, fast, and modern setup for frontend development using **Vite** & **Tailwind CSS**

[![Made with Vite](https://img.shields.io/badge/Made%20with-Vite-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Styled%20with-TailwindCSS-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Node.js](https://img.shields.io/badge/Node.js-%3E%3D18.0.0-green?logo=node.js&logoColor=white)](https://nodejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 📖 Overview

This guide helps you **install and configure Vite with Tailwind CSS** step by step.  
Whether you’re using React, Vue, or vanilla JavaScript — this setup ensures a fast, clean, and modern frontend workflow.

---

## 🚀 Step 1: Create a Vite Project

Open your terminal and run:

```bash
npm create vite@latest my-project
```

Choose your preferred framework and variant (for example: **React + JavaScript**).  
Then move into your project folder:

```bash
cd my-project
```

---

## 🧩 Step 2: Install Dependencies

Run this to install all dependencies:

```bash
npm install
```

---

## 🌈 Step 3: Install Tailwind CSS

Install Tailwind and its required dependencies:

```bash
npm install -D tailwindcss postcss autoprefixer
```

Initialize Tailwind with configuration files:

```bash
npx tailwindcss init -p
```

This creates two files:
- `tailwind.config.js`
- `postcss.config.js`

---

## ⚙️ Step 4: Configure Tailwind

Open `tailwind.config.js` and update it like this:

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

This ensures Tailwind scans your project files for class names.

---

## 🎨 Step 5: Add Tailwind Directives

Open your main CSS file (usually `src/index.css`) and add:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## 🧠 Step 6: Start the Development Server

Run:

```bash
npm run dev
```

Then open the development URL (usually [http://localhost:5173](http://localhost:5173)) in your browser.  
If everything’s working, Tailwind styles should apply instantly.

---

## 🧱 Step 7: Test Tailwind Setup

Open `App.jsx` and replace its contents with:

```jsx
export default function App() {
  return (
    <div className="flex min-h-screen items-center justify-center bg-gray-100">
      <h1 className="text-4xl font-bold text-blue-600">
        Hello Vite + Tailwind! ⚡
      </h1>
    </div>
  );
}
```

If you see the styled “Hello Vite + Tailwind!” message, the setup is complete.

---

## 🧰 Step 8: Build for Production

When you’re ready to deploy, run:

```bash
npm run build
```

This will create a `dist/` folder with optimized static assets.

---

## 📘 Summary

| Tool | Purpose |
|------|----------|
| ⚡ **Vite** | Lightning-fast dev server and bundler |
| 🎨 **Tailwind CSS** | Utility-first CSS framework for rapid styling |
| 🧱 **PostCSS + Autoprefixer** | Handles cross-browser CSS compatibility |

**Quick Setup Recap**
```
npm create vite@latest my-project
cd my-project
npm install
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

---

## 🌍 Useful Links

- 🔗 [Vite Official Docs](https://vitejs.dev/)
- 🔗 [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- 🔗 [PostCSS Documentation](https://postcss.org/)

---

## 🪄 Tips

- Use `.jsx` or `.tsx` files when working with React and Tailwind.  
- Enable auto-formatting in your code editor for clean class ordering.  
- You can customize colors, fonts, and themes inside `tailwind.config.js`.

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use and modify.

---

<div align="center">

### 💻 Made with Vite ⚡, Tailwind 🎨, and Curiosity 🧠  
⭐ If this helped you, don’t forget to **star the repo**!
# Akash Bhattacharyya.

</div>
