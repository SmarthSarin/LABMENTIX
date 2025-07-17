# 🎙️ Speech To Text Website

## 🚀 Step 1: Create the App

```bash
npm create vite@latest
```

### During setup

* **Project Name**: `SpeechToTextWebsite` (you can use any name)
* **Framework**: `React`
* **Variant**: `JavaScript + SWC`

---

## 📂 Step 2: Navigate into the Project

```bash
cd SpeechToTextWebsite
```

---

## 📦 Step 3: Install Dependencies

```bash
npm install
```

---

## 🧪 Step 4: Run the Development Server

```bash
npm run dev
```

---

## 🎨 Step 5: Install Tailwind CSS

```bash
npm install tailwindcss @tailwindcss/vite
```

## ⚙️ Step 6: Configure Tailwind

Add the @tailwindcss/vite plugin to your Vite configuration which is in vite.config.js

```bash
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'
export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
```

## ⚙️ Step 7: Import Tailwind CSS into your CSS file

In your project, open src/index.css and add

```bash
@import "tailwindcss";
```

## 💡 Notes

* This project uses **Vite** for fast builds and hot module reloading.
* **SWC** is used instead of Babel for faster transpiration.
**Tailwind CSS** enables rapid UI development with utility-first classes — no more writing custom CSS for common styling tasks.
