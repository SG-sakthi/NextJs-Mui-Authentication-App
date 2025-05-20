: <<'README'

# 🌐 Next.js + MUI Web App with Expo Android Integration

This project showcases the seamless integration of a **Next.js web application** styled with **Material-UI (MUI)** into a native **Android app built using Expo** via `WebView`. It also includes **Firebase Authentication with Google Sign-In** and **native push notifications using Firebase Cloud Messaging (FCM)**.

---

## ✨ Highlights

### 🌍 Next.js Web App
- Built using **Next.js 15**
- Styled with **Material-UI**
- **Firebase Google Sign-In** integration
- Mobile-friendly, modern responsive UI

### 📱 Expo Android App
- Integrates Next.js app using **React Native WebView**
- Handles **native FCM push notifications**
- Compatible with **physical Android devices** and **emulators**

---

## ⚙️ Requirements

Make sure the following are installed:
- **Node.js** (v14+)
- **npm** or **yarn**
- **Expo CLI**
- **Android Studio** or a physical Android device
- A **Firebase Project**
- A **Google Cloud OAuth Client**

---

## 📁 Project Structure

nextjs-mui-mobile-app/
├── nextjs-mui-auth-app/ # Web App
│ └── .env.local # Firebase config for web
│
└── necxis-webview-app/ # Expo Android App
└── .env # Firebase config for native app

## Configure the Web App (Next.js + MUI)
cd nextjs-mui-auth-app
npm install

## Create a .env.local file with your Firebase web credentials:

NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

## Configure the Expo Android App
cd ../necxis-webview-app
npm install

##Create a .env file for Firebase native configuration:

GOOGLE_EXPO_CLIENT_ID=your_expo_client_id
GOOGLE_ANDROID_CLIENT_ID=your_android_client_id
GOOGLE_IOS_CLIENT_ID=your_ios_client_id
FIREBASE_API_KEY=your_firebase_api_key
FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
FIREBASE_PROJECT_ID=your_firebase_project_id
FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
FIREBASE_APP_ID=your_firebase_app_id

## Start the Web App
cd nextjs-mui-auth-app
npm run dev

##Start the Android App (Expo)
cd ../necxis-webview-app
npx expo start

##Next.js App (Vercel or Manual)
cd nextjs-mui-auth-app
npm run build

## Firebase & Notifications
Add Android app to Firebase Console

Enable Authentication → Google Sign-In

Configure Firebase Cloud Messaging

Add google-services.json for Android builds

Test notifications via Firebase Console or Firebase Admin SDK
