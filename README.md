Perfect — since you’re setting up a **mini project** and want to go the CLI route, let me give you a clean, ready‑to‑use **README template** for your `azure-webapp-demo` repo. You can paste this directly, and it will document your steps clearly.

---

# Azure Web App Demo

## 📖 Overview
This project demonstrates deploying a simple Node.js application to **Azure Web App** using both the **Azure Portal** and the **Azure CLI**.  
The app is a minimal Express server that responds with “Hello from Azure Web App!”.

---

## ⚙️ Prerequisites
- An Azure account (Free tier or Pay‑As‑You‑Go).
- Installed [Node.js](https://nodejs.org/) (includes npm).
- Installed Azure CLI [(learn.microsoft.com in Bing)](https://www.bing.com/search?q="https%3A%2F%2Flearn.microsoft.com%2Fcli%2Fazure%2Finstall-azure-cli").
- A GitHub repository (`azure-webapp-demo`).

---

## 🛠️ Project Setup
1. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/azure-webapp-demo.git
   cd azure-webapp-demo
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run locally:
   ```bash
   npm start
   ```
   Visit `http://localhost:3000` to see the app.

---

## 📂 Project Structure
```
azure-webapp-demo/
│── app.js
│── package.json
│── README.md
│── screenshots/
    └── azure-webapp.png
```

---

## 🚀 Deploy with Azure CLI
1. Log in:
   ```bash
   az login
   ```

2. Create a resource group (if not already):
   ```bash
   az group create --name demo-rg --location eastus
   ```

3. Deploy the app:
   ```bash
   az webapp up --name azure-webapp-demo --resource-group demo-rg --runtime "NODE|18-lts"
   ```

4. Verify deployment:  
   Open `https://azure-webapp-demo.azurewebsites.net` in your browser.

---

## 🌐 Deploy via GitHub
1. In the Azure Portal, go to your Web App → **Deployment Center**.  
2. Connect your GitHub repo (`azure-webapp-demo`).  
3. Enable CI/CD so every push to `main` redeploys automatically.

---

## ✅ Verification
- Visit your Web App URL.  
- You should see: **Hello from Azure Web App!**  
- Take a screenshot and save it in `/screenshots/azure-webapp.png`.

---

## 🎯 Outcome
By following these steps, you’ll have:
- A live Azure Web App running your Node.js project.
- A GitHub repo with documentation and screenshot proof.
- Both CLI and Portal deployment methods tested.

---

This README gives you a professional structure and makes your mini project look polished.  

👉 Do you want me to also include the **exact `app.js` code snippet** inside the README so it’s fully self‑contained, or would you prefer to keep the code separate in the file?
