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

---

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

---

## 📄 Step 7: Import Tailwind CSS into your CSS file

In your project, open src/index.css and add

```bash
@import "tailwindcss";
```

---

## 🖥️ Step 8: Set Up the Backend with Express

Now let's set up a backend using Express.js.

### 📁 1. Create a Backend Folder

Inside your project directory, create a new folder named:

```bash
SpeechToTextServer
```

### 🧱 2. Initialize the Project

Open a terminal in the `SpeechToTextServer` folder and run:

```bash
npm init
```

> Press `Enter` through the prompts or fill in your project details (e.g., name, description, entry point as `index.js`, etc.).

### 📦 3. Install Express

```bash
npm install express
```

### 📝 4. Create `index.js` File

Inside `SpeechToTextServer`, create a file named `index.js` and add:

```js
const express = require('express');
const app = express();
const PORT = 3000;

app.use(express.json());

app.get('/', (req, res) => {
  res.send('Speech-to-Text Backend is Running');
});

app.listen(PORT, () => {
  console.log(`✅ Server running at http://localhost:${PORT}`);
});
```

### ▶️ 5. Run the Server

In terminal:

```bash
node index.js
```

---

## 💡 Notes

* This project uses **Vite** for fast builds and hot module reloading.
* **SWC** is used instead of Babel for faster transpiration.
**Tailwind CSS** enables rapid UI development with utility-first classes — no more writing custom CSS for common styling tasks.
