ভাই বোন ইলেকট্রনিক্স — মোবাইল দিয়ে APK বানানোর নির্দেশনা

এই ZIP-এ HTML অ্যাপটি Android অ্যাপের মধ্যে রাখা হয়েছে। Google Fonts-এর অনলাইন লিংক সরানো হয়েছে, তাই UI ফন্টের জন্য ইন্টারনেট লাগবে না। অ্যাপের জন্য INTERNET permission দেওয়া হয়নি।

মোবাইল দিয়ে APK বানানোর উপায়:
1. ZIP ফাইলটি ফোনে Extract করুন (যেমন Files app বা ZArchiver দিয়ে)।
2. GitHub.com-এ অ্যাকাউন্টে লগইন করুন।
3. নতুন Public repository তৈরি করুন, নাম দিন VaiBonElectronics এবং README যোগ করার অপশন বন্ধ রাখুন।
4. Repository-তে Add file > Upload files দিয়ে ZIP-এর ভেতরের ফাইল/ফোল্ডারগুলো আপলোড করুন; ZIP ফাইলটিকে একা আপলোড করবেন না। .github ফোল্ডারটিও অবশ্যই আপলোড করতে হবে।
5. Upload/commit করার পর Actions ট্যাবে যান। “Build Android APK” workflow দেখা গেলে সেটি খুলে Run workflow চাপুন।
6. কাজ শেষ হলে সবুজ সফল রান খুলে নিচে Artifacts অংশ থেকে VaiBonElectronics-APK ডাউনলোড করুন।
7. ZIP extract করে app-debug.apk ইনস্টল করুন। ফোনে অনুমতি চাইলে এই উৎস থেকে ইনস্টল অনুমতি দিন।

নোট:
- APK build করার সময় ইন্টারনেট লাগবে; ইনস্টল করা অ্যাপটি HTML-এর লোকাল কপি চালাবে।
- IndexedDB ডেটা সাধারণত এই অ্যাপ ইনস্টলেশনের ভেতরে থাকে। অ্যাপ uninstall বা app data clear করলে ডেটা মুছে যেতে পারে। Settings থেকে নিয়মিত JSON backup নিন।
- প্রথমবার ইনস্টল করার পর ডেমো/বাস্তব ডেটা প্রবেশের আগে অ্যাপ খুলে পরীক্ষা করুন।
