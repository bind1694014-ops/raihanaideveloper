# My AI Assistant — ওয়েবসাইট + Google লগইন সেটআপ

## ১. Firebase প্রজেক্ট (ফ্রি)
1. console.firebase.google.com → Add project (Analytics বন্ধ রাখতে পারেন)।
2. Build → **Authentication** → Get started → Sign-in method → **Google** → Enable → Save।
3. Build → **Firestore Database** → Create database (Production mode)।
4. Firestore → **Rules** ট্যাবে নিচেরটা বসিয়ে Publish করুন:

```
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /users/{uid}/{doc=**} {
      allow read, write: if request.auth != null && request.auth.uid == uid;
    }
  }
}
```
5. Project settings (⚙) → Your apps → **Web (</>)** → Register app → `firebaseConfig`-এর মান কপি করুন।
6. `config.js` ফাইলে `apiKey`, `authDomain`, `projectId`, `appId` বসান।

## ২. হোস্টিং (GitHub Pages)
1. github.com → New repository (Public) → সব ফাইল আপলোড (`index.html, config.js, sw.js, manifest.json, icon-192.png, icon-512.png`)।
2. Settings → Pages → Deploy from branch → main → /(root) → Save।
3. লিংক: `https://আপনার-নাম.github.io/রিপোর-নাম/`

## ৩. ডোমেইন অনুমতি (জরুরি)
Firebase → Authentication → Settings → **Authorized domains** → Add domain → `আপনার-নাম.github.io`

## ৪. ব্যবহার
লিংক খুললেই Google লগইন আসবে। লগইনের পর API key, মডেল, মেমরি, সেটিংস ক্লাউডে সেভ হয় এবং যেকোনো ডিভাইসে লগইন করলে ফিরে আসে।
প্রথমবার পুরোনো ব্রাউজারে (যেখানে key দেওয়া আছে) লগইন করলে সেগুলো ক্লাউডে উঠে যাবে।
