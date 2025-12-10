# 📦 ParcelsApp Custom Card for Home Assistant

A modern, easy-to-use Lovelace card for the ParcelsApp integration. Track your incoming deliveries directly from your Home Assistant dashboard!

## ✨ Features
- **Easy Tracking**: Add new packages by simply pasting the tracking ID.
- **Visual Editor**: Configure the card title and height directly in the UI—no YAML required!
- **Rich Details**: See status, carrier, location, origin, destination, and transit time at a glance.
- **Smart Coloring**: Badges color-code automatically (Green for Delivered, Orange for Pending/Transit, Red for Unknown).
- **Responsive**: Adapts to your dashboard columns and scales perfectly.
- **Scrollable**: Optional max-height setting with a built-in scrollbar for long lists.

---

## 🛠️ How to Install

### Step 1: Create the Folders
1.  Use a File Manager (like VS Code Server, File Editor addon, or Samba) to access your Home Assistant configuration files.
2.  Navigate to the `www` folder in your configuration directory (usually `/config/www`).
    *   *If `www` doesn't exist, create it.*
3.  Inside `www`, create a new folder named `parcelsapp`.

### Step 2: Add the Card File
1.  Download the `parcels-app-card.js` file.
2.  Upload/Place it into the folder you just created:
    `config/www/parcelsapp/parcels-app-card.js`

### Step 3: Register the Resource
1.  Go to your Home Assistant Dashboard.
2.  Click **Settings** (Sidebar) → **Dashboards**.
3.  Click the **3 dots** in the top-right corner → **Resources**.
4.  Click **+ ADD RESOURCE** (bottom right).
5.  Enter the following details:
    *   **URL**: `/local/parcelsapp/parcels-app-card.js`
    *   **Resource type**: `JavaScript Module`
6.  Click **Create**.

### Step 4: Add to Your Dashboard
1.  Go to your Dashboard and click the **Pencil Icon** (Edit Dashboard).
2.  Click **+ ADD CARD**.
3.  Search for **"Parcels App"** in the list.
4.  Select **Parcels App Tracking Card**.
5.  (Optional) Use the visual editor to change the Title or set a Max Height (e.g., `400px`).
6.  Click **Save**.

🎉 **You're done!** Enjoy tracking your packages.
