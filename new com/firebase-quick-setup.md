# Quick Firebase Setup for Real-Time Collaboration

## Step 1: Create Firebase Project
1. Go to https://console.firebase.google.com/
2. Click "Create a project"
3. Project name: `schedule-website` (or your choice)
4. Disable Google Analytics (optional)
5. Click "Create project"

## Step 2: Setup Realtime Database
1. In Firebase Console, click "Realtime Database"
2. Click "Create Database"
3. Choose "Start in test mode"
4. Select location (closest to your users)
5. Click "Done"

## Step 3: Get Configuration
1. Click gear icon → "Project settings"
2. Scroll to "Your apps" section
3. Click web icon `</>`
4. App nickname: `Schedule Website`
5. Copy the config object

## Step 4: Update Your Code
1. Open `firebase-config.js` in your project
2. Replace the placeholder config with your real config:

```javascript
const firebaseConfig = {
  apiKey: "your-real-api-key-here",
  authDomain: "your-project.firebaseapp.com",
  databaseURL: "https://your-project-default-rtdb.firebaseio.com/",
  projectId: "your-project-id",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "123456789",
  appId: "your-real-app-id"
};
```

3. Save and upload the updated file to GitHub

## Step 5: Test Real-Time Collaboration
1. Open your GitHub Pages website in multiple browser tabs
2. Click "የሳምንቱን ፕሮግራሞች ማስተካከያ" in one tab
3. Make schedule changes
4. Watch changes appear instantly in other tabs! ✨

## Security Note
The current setup allows anyone to edit. For production:
1. Go to Firebase → Database → Rules
2. Add authentication rules as needed