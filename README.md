# Zohirola – Download website

একটাই পেজের ওয়েবসাইট (`index.html`)। বাংলা ও ইংরেজি, লাইট ও ডার্ক মোড।

## GitHub Pages-এ চালানোর নিয়ম

1. GitHub-এ একটা নতুন রিপো বানান (যেমন `zohirola`)।
2. এই ফোল্ডারের সব ফাইল (`index.html`, `404.html`, `favicon.svg`, `og.png`, `.nojekyll`) রিপোতে আপলোড করুন।
3. **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**।
4. কয়েক মিনিট পর সাইট চালু হবে: `https://USERNAME.github.io/zohirola/`

## APK কীভাবে দেবেন (যেকোনো একটা)

**A. রিলিজ থেকে (সবচেয়ে সহজ, বড় APK-র জন্যও)**
1. রিপোর **Releases → Create a new release** এ গিয়ে APK ফাইলটা অ্যাটাচ করুন।
2. `index.html`-এর উপরের `CONFIG` ব্লকে `githubRepo: "USERNAME/zohirola"` লিখুন।
3. এরপর থেকে নতুন রিলিজ দিলেই ডাউনলোড বাটন আর ভার্সন নম্বর নিজে নিজে বদলে যাবে।

**B. সরাসরি ফাইল হিসেবে**
APK-র নাম `Zohirola.apk` রেখে `index.html`-এর পাশেই আপলোড করুন।
(GitHub ওয়েবসাইট দিয়ে আপলোডে প্রতি ফাইল ২৫ MB পর্যন্ত। বড় হলে A ব্যবহার করুন।)

**C. Firebase থেকে**
`firebaseDbUrl`-এ Realtime Database লিংক দিলে অ্যাডমিন অ্যাপের `/app_update` থেকে লিংক ও ভার্সন নেবে।

## ছোট নোট
- অ্যাপের নাম বদলাতে চাইলে `CONFIG.appName`।
- শেয়ার প্রিভিউ ছবি `og.png`। কাস্টম ডোমেইন পেলে `og:image`-এ পুরো লিংক বসালে সব জায়গায় ঠিকমতো দেখাবে।
