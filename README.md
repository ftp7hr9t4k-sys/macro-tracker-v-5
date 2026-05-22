# ⚫ Macro Tracker V6

**Clean B&W Lean Bulk Tracker** with local storage + optional cloud sync

## Features

✅ **Local Tracking** – Track protein, carbs, calories with browser localStorage  
✅ **Food Database** – Search OpenFoodFacts API for real macro data (scaled by grams)  
✅ **Multi-user Profiles** – Switch between different tracking profiles  
✅ **Real-time Feedback** – Smart bulk status: protein targets, calorie surplus alerts  
✅ **Cloud Sync** – Optional Firebase integration for pull/push sync  
✅ **Clean UI** – Minimalist black & white design, mobile responsive  

## Quick Start

1. **Visit the app:** https://ftp7hr9t4k-sys.github.io/macro-tracker-v-5/
2. **Set a profile name** (e.g., "Alex")
3. **Log foods** – Type food name + grams → searches OpenFoodFacts
4. **View totals** – See protein, carbs, calories with real-time feedback

## How It Works

### Local Tracking (Always Works)
- All data stored in `localStorage` → persists across sessions
- No server needed
- Works offline

### Cloud Sync (Optional)
1. Add your Firebase config to `index.html` (replace `YOUR_*` placeholders)
2. Click **Google** or **Anonymous** login
3. Use **Pull from cloud** / **Push to cloud** buttons

## Deploy Options

### Option 1: GitHub Pages (Free, Already Live! ✅)
Your app is live at: **https://ftp7hr9t4k-sys.github.io/macro-tracker-v-5/**

```bash
# Already deployed! No extra steps needed.
# Updates push automatically when you edit index.html
```

### Option 2: Vercel (Already Configured)
```bash
# Already points to: https://macro-tracker-v-5.vercel.app
```

### Option 3: Netlify (Free)
1. Drag & drop `index.html` to https://app.netlify.com/drop
2. Get instant live link

## Firebase Setup (For Cloud Sync)

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a new project
3. Enable **Authentication** (Google + Anonymous)
4. Enable **Firestore** (start in test mode)
5. Copy your config and replace in `index.html`:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "123456789",
  appId: "1:123456789:web:abcdef"
};
```

Then commit & push to GitHub – updates live instantly! 🚀

## Tech Stack

- **Frontend:** Vanilla JS (no frameworks)
- **Data:** localStorage + OpenFoodFacts API (free)
- **Auth/DB:** Firebase (optional)
- **Hosting:** GitHub Pages / Vercel / Netlify

## Customization

Edit `index.html` to:
- Change protein target (currently 140g-165g)
- Adjust bulk surplus thresholds
- Modify UI colors/fonts
- Add more macros (fiber, fat, etc.)

## License

MIT – Use freely, modify as needed

---

**Built for lean bulk tracking** 🥗💪
