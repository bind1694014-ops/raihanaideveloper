# Rayhan AI — v19 আপডেট

## ✏ চ্যাটেই সরাসরি ছবি এডিট
- চ্যাটের 📎 দিয়ে ছবি যুক্ত করুন → লিখুন কী বদলাবেন (যেমন "হাসি যোগ করো", "ব্যাকগ্রাউন্ড সাদা করো") → Send। Studio খুলতে হবে না।
- প্রম্পট প্রশ্ন মনে হলে (যেমন "এতে কী আছে?") সাধারণ চ্যাট উত্তর আসবে। জোর করে এডিট চালাতে ছবির পাশের **✏ AI এডিট** বাটন চাপুন।
- ফলাফলের নিচে **✏ আবার এডিট করো** বাটনে ওই ছবিই আবার এডিট করা যায়।
- এডিটে আগের Photo Expert পদ্ধতিই চলে (ছবি দেখা → প্ল্যান → এডিট → নিজে যাচাই)। Gemini/OpenRouter key লাগবে; ফলাফলের মান (১-১০) সৎভাবে দেখানো হয়।

## 🖼 নতুন আইকন
- `icon-192.png`, `icon-512.png` (সাধারণ) এবং `icon-maskable-192.png`, `icon-maskable-512.png` (Android গোল/স্কয়ার মাস্ক-সেফ)।
- আপডেটের পর ফোনে পুরোনো আইকন বদলাতে পুরোনো শর্টকাট মুছে আবার "Add to Home screen" করুন।

# Rayhan AI — v15 আপডেট

## 🛡 টুলবক্সে নতুন ২০টা সিকিউরিটি ও অটোমেশন টুল
(সবই ডিফেন্সিভ/এথিক্যাল; বেশিরভাগ ডিভাইসেই চলে)
১ পাসওয়ার্ড জেনারেটর ও শক্তি পরীক্ষা · ২ হ্যাশ (SHA) টেক্সট/ফাইল · ৩ Base64/URL/Hex/Binary/HTML এনকোড-ডিকোড · ৪ JWT ডিকোডার · ৫ Regex টেস্টার · ৬ JSON ফরম্যাটার
৭ AES-256 এনক্রিপ্ট/ডিক্রিপ্ট · ৮ পাসওয়ার্ড লিক চেক (HIBP k-anonymity) · ৯ DNS লুকআপ + SPF/DMARC চেক · ১০ আমার IP ও ব্রাউজার ফুটপ্রিন্ট · ১১ URL অ্যানালাইজার (ফিশিং লক্ষণ + defang)
১২ ছবির EXIF/GPS দেখা ও মুছে সেভ · ১৩ ইনভিজিবল টেক্সট (zero-width) · ১৪ সাইফার ও মোর্স · ১৫ ফিশিং ডিটেক্টর (AI) · ১৬ কোড সিকিউরিটি রিভিউ (AI)
১৭ এক্সপোজার অডিট (নিজের ডোমেইনের OSINT ডর্ক, Wayback, crt.sh) · ১৮ HTTP/API টেস্টার · ১৯ প্রম্পট চেইন অটোমেশন · ২০ শিডিউলড AI অটোমেশন (অ্যাপ খোলা থাকলে)

## ⚙ Settings-এ নতুন
- **➕ আরও AI প্রোভাইডার**: Grok (xAI), Groq, DeepSeek, OpenAI, Mistral, Together, Perplexity, Cerebras বা কাস্টম (Base URL + key)। যোগ করে "মডেল লিস্ট"-এ প্রোভাইডার বেছে মডেল ID দিন। চ্যাট, তুলনা, মডেল সভা, চেইন — সবখানে কাজ করবে।
- **🧩 অন্যান্য সার্ভিস API**: News, Stability, LiveKit, Google Search, OpenWeather, Mem0, Song finder ইত্যাদির জন্য আলাদা ঘর + নিজের নামে নতুন API যোগের অপশন + `.env` কপি বাটন। কোডে পড়তে: `RX_API.get('NEWS_API_KEY')`।
- key কোনো ফাইলে হার্ডকোড নেই — শুধু আপনার ডিভাইসে (লগইন করলে প্রাইভেট ক্লাউডে) সেভ হয়।

# Rayhan AI — নতুন ফিচার (v14)

## 🐍 কোড ইন্টারপ্রেটার
- টুলবক্স → **কোড ইন্টারপ্রেটার**
- ব্রাউজারেই Python চলে (Pyodide, প্রথমবার ~10MB)
- Excel/CSV ধরনের হিসাব, লুপ, numpy/pandas (প্যাকেজ ইনস্টল বাটন)
- AI দিয়ে কোড লেখার বাটন আছে

## 🌐 এক ক্লিকে ওয়েবসাইট লাইভ
1. Settings / টুলবক্স → **ওয়েবসাইট লাইভ** থেকে Netlify Personal Access Token সেভ করুন  
   (https://app.netlify.com/user/applications#personal-access-tokens)
2. **🛠 Build app** চালু করে গেম/অ্যাপ বানান
3. AI HTML দিলে চ্যাটে বা Preview-তে **🌐 Live** চাপুন
4. পাবলিক HTTPS লিংক পাবেন

## 📱 APK (ফোনে ইনস্টল)
Build মোডে HTML গেম/অ্যাপ এলে এখন বাটনগুলো:
- ▶ Preview / Test
- 🔍 Review & Fix
- ⬇ HTML
- **📱 APK** ← নতুন
- **🌐 Live** ← নতুন

**📱 APK** চাপলে Android Studio-রেডি প্রজেক্ট ZIP ডাউনলোড হয় (`*-apk-project.zip`):
- WebView অ্যাপ + আপনার HTML `assets/index.html`-এ
- README-APK.txt-এ ধাপে ধাপে নির্দেশনা
- Android Studio দিয়ে APK বানিয়ে ফোনে ইনস্টল করুন

> ব্রাউজার থেকে সরাসরি সাইন করা `.apk` ফাইল জেনারেট করা সম্ভব নয় (Google/Android নিরাপত্তা)। তাই সম্পূর্ণ সোর্স প্রজেক্ট দেওয়া হয়েছে যাতে আসল ইনস্টলযোগ্য APK তৈরি হয়।

## ফাইল তালিকা
- index.html (আপডেটেড)
- config.js, manifest.json, sw.js, icon-192.png, icon-512.png
- README-SETUP.md, README-NEW-FEATURES.md

## 👑 মালিক চেনা (v16)
- Settings → **👑 মালিক ফেস সেটআপ** → নিজের ছবি দিন → ফেসপ্রিন্ট (১২৮ সংখ্যা) তৈরি হয়, ছবি সেভ/আপলোড হয় না।
- "config.js লাইন কপি" চেপে `config.js`-এর `window.OWNER_FACE = [];` লাইনটা বদলে আপলোড করুন → সব ইউজারের ফোনে চালু।
- ক্যামেরা চালু থাকলে বা কেউ ছবি দিলে, ডিভাইসেই মুখ মিলিয়ে দেখা হয়; মিললে "আপনি আমার মালিক ও ডেভেলপার" বার্তা ও ভয়েস আসে।
- এটা শুধু অভিবাদন। এর ভিত্তিতে কোনো অ্যাডমিন/বিশেষ অধিকার দেবেন না (ছবি দেখিয়ে ফাঁকি দেওয়া সম্ভব)।

## 🎨 Stability AI (v17)
- Settings → **🎨 Stability AI API key** (OpenRouter ঘরের ঠিক নিচে) → key বসান, মডেল বাছুন (Core / SD3.5 Large / Ultra), "টেস্ট" চেপে ক্রেডিট দেখুন।
- key থাকলে নতুন ছবি তৈরি (Studio, মুভির দৃশ্য, চ্যাটে ছবি বানাও) আগে Stability দিয়ে হয়। ব্যর্থ হলে Gemini → ফ্রি Pollinations।
- ছবি এডিট (Expert) আগের মতো Gemini/OpenRouter দিয়েই চলে।

## 🖼 চ্যাটে সরাসরি ছবি (v18)
চ্যাটে "ছবি বানাও" / "image banao ..." লিখলে এখন মডেলের উত্তরের অপেক্ষা না করে সরাসরি ইমেজ জেনারেটর চলে (Stability → Gemini → ফ্রি)। বাংলা/Banglish অনুরোধ আগে ইংরেজি ডিটেইল প্রম্পটে বদলে নেওয়া হয়।


# Rayhan AI — বর্তমান প্যাকেজের আপডেট

- নতুন Rayhan AI neon icon চারটি Android/PWA icon size-এ যুক্ত করা হয়েছে।
- Chat input-এ Gallery attachment-এর পাশে 📄 File button যোগ হয়েছে। PDF, TXT, Markdown, CSV, JSON, HTML, XML, JS, Python, log, DOCX এবং XLS/XLSX ফাইল পড়ার চেষ্টা করে; PDF/DOCX/XLSX-এর জন্য প্রথমবার ইন্টারনেট থেকে parser library লোড হতে পারে।
- Live Voice স্ক্রিনে 📖 Long Story Mode যোগ হয়েছে। চালু থাকলে AI-এর পরের অংশ স্বয়ংক্রিয়ভাবে চাইবে; বন্ধ করতে একই বোতাম আবার চাপুন বা কল End করুন। API/model সীমা, নেটওয়ার্ক বা voice service-এর সমস্যায় একটানা বলা ব্যাহত হতে পারে।
- Service worker cache version আপডেট করা হয়েছে যাতে নতুন ফাইল লোড হয়।


# Story Features 1–7 update
- Story style selector: auto, animal movie, mystery, horror, adventure, romance, Islamic educational, fantasy, realistic, bedtime.
- Longer Bengali storytelling directions with continuity, dialogue, emotion and no English status announcements.
- Recent story text stored in local browser storage; resume/clear controls are in Live Voice settings. This is local only, not cloud sync.
- Empty/error story responses stop auto-continuation instead of endlessly retrying.
- TTS is asked for expressive narration; actual emotional/volume control depends on the selected voice service. Separate voices for every character are not guaranteed.


# Free-first story voice update (2026-10)
- গল্প বলার prompt-এ পেশাদার, স্বাভাবিক বাংলা audiobook narration জোরদার করা হয়েছে।
- গল্পে সাউন্ড ইফেক্ট, ব্যাকগ্রাউন্ড মিউজিক, ambience বা কৃত্রিম sigh/filler যোগ না করতে বলা হয়েছে।
- Settings UI থেকে ঐচ্ছিক paid/add-on OpenRouter, Stability ও extra service API প্যানেল লুকানো হয়েছে; মূল Gemini API key সেটিংস রাখা হয়েছে।
- কণ্ঠের বাস্তবতা নির্বাচিত ব্রাউজার/TTS voice-এর ওপর নির্ভর করে; সম্পূর্ণ মানুষের কণ্ঠের নিশ্চয়তা নেই। Gemini API ব্যবহারে ফ্রি quota সীমা থাকতে পারে।
