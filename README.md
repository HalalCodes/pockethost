# 🚀 PocketHost Studio

### Multi-Repo GitHub Hosting Engine

**PocketHost Studio** হলো একটি **mobile-friendly static website & image hosting engine**, যা **GitHub REST API** এবং **GitHub Pages** প্রযুক্তি ব্যবহার করে তৈরি।

এর মাধ্যমে GitHub-এ সরাসরি ম্যানুয়ালি প্রবেশ না করেই আপনার **ব্রাউজার বা মোবাইল অ্যাপ** থেকে সহজেই ফাইল, ছবি এবং HTML ওয়েবসাইট GitHub Repository-তে আপলোড করে **লাইভ হোস্টিং লিংক** তৈরি করা যায়।

---

## ✨ প্রধান বৈশিষ্ট্যসমূহ

### 📦 1. Multi-Repository Management

GitHub-এর Repository storage সীমার কাছাকাছি পৌঁছে গেলে নতুন Repository যুক্ত করে সহজেই hosting চালিয়ে যেতে পারবেন।

* একাধিক Repository সংযুক্ত করা যায়
* এক ক্লিকে Repository পরিবর্তন করা যায়
* প্রতিটি নতুন Repository-তে মূল PocketHost Studio কোড পুনরায় আপলোড করার প্রয়োজন নেই
* বিভিন্ন Repository আলাদাভাবে hosting storage হিসেবে ব্যবহার করা যায়

---

### 📁 2. Dynamic Folder System

আপনার Hosted Files সুন্দরভাবে সাজিয়ে রাখার জন্য রয়েছে Dynamic Folder System।

আপনি চাইলে নিজের প্রয়োজন অনুযায়ী যেকোনো Folder তৈরি করতে পারবেন।

**উদাহরণ:**

```text
/
├── picture/
├── website/
├── projects/
├── assets/
└── documents/
```

আরও সুবিধাজনক বিষয় হলো—

> কোনো Folder-এর ভিতরে নতুন File বা Image Upload করার সময় সেই Folder-এর অপ্রয়োজনীয় `.gitkeep` File থাকলে সেটি স্বয়ংক্রিয়ভাবে মুছে দেওয়া হবে।

---

### 🖼️ 3. Image Hosting

Gallery বা Upload Section ব্যবহার করে সরাসরি GitHub Repository-তে ছবি Upload করুন এবং সঙ্গে সঙ্গে একটি Direct Image URL পান।

**উদাহরণ:**

```text
https://username.github.io/repository/picture/myphoto.jpg
```

এই URL আপনি ব্যবহার করতে পারবেন—

* Website
* Blog
* Portfolio
* Social Media
* HTML/CSS Project
* API/Data Project
* Image Preview

ইত্যাদিতে।

---

### 🌐 4. HTML & Static Website Hosting

শুধু Image নয়, HTML এবং অন্যান্য Static Files-ও সরাসরি GitHub Pages-এর মাধ্যমে Host করা যাবে।

একটি HTML File Upload করার পর PocketHost Studio স্বয়ংক্রিয়ভাবে তার Live URL তৈরি করবে।

**উদাহরণ:**

```text
https://username.github.io/repository/website/index.html
```

অর্থাৎ, ছোট Static Website বা Web Project দ্রুত Online করা সম্ভব।

---

### 🗑️ 5. 5-Second Safety Delete

ভুল করে কোনো File বা Folder Delete হয়ে যাওয়া ঠেকাতে রয়েছে নিরাপদ Delete System।

Delete করার আগে:

```text
5 → 4 → 3 → 2 → 1
```

একটি Animated Countdown চলবে।

এই সময়ের মধ্যে চাইলে **Cancel** করে Delete বন্ধ করা যাবে।

এটি বিশেষভাবে গুরুত্বপূর্ণ, কারণ GitHub Repository থেকে কোনো File Delete করলে সেটি সঙ্গে সঙ্গে Repository-তে পরিবর্তন হিসেবে Commit হয়ে যেতে পারে।

---

## ⚙️ কীভাবে কাজ করে?

PocketHost Studio সম্পূর্ণ **Client-Side Architecture** অনুসরণ করে।

```text
┌──────────────────────┐
│   PocketHost Studio  │
│      Web / App       │
└──────────┬───────────┘
           │
           │ GitHub REST API
           │ + Personal Access Token
           ▼
┌──────────────────────┐
│   GitHub Repository  │
│                      │
│  Files / Images      │
│  HTML / Folders      │
└──────────┬───────────┘
           │
           │ GitHub Pages
           ▼
┌──────────────────────┐
│    Live Website      │
│   / Images / Files   │
└──────────────────────┘
```

কোনো আলাদা Hosting Server বা Database-এর প্রয়োজন নেই।

---

# 🔐 GitHub Connection

PocketHost Studio ব্যবহার করার জন্য আপনার GitHub Account-এর সঙ্গে সংযোগ স্থাপন করতে হবে।

### ধাপ ১ — Personal Access Token তৈরি করুন

GitHub Account থেকে একটি:

**Personal Access Token (Classic)**

তৈরি করুন।

প্রয়োজনীয় Permission:

```text
repo
```

### ধাপ ২ — PocketHost Studio-তে তথ্য দিন

Settings থেকে আপনার:

```text
GitHub Username
GitHub Personal Access Token
```

সংরক্ষণ করুন।

Token আপনার Browser-এর **Local Storage**-এ সংরক্ষিত থাকবে এবং API Request-এর সময় ব্যবহার করা হবে।

> ⚠️ আপনার GitHub Token কখনো অন্য কারও সঙ্গে শেয়ার করবেন না।

---

# 📂 Folder তৈরি

প্রথমে **Folders** Section-এ যান।

তারপর:

```text
Folder Name
      ↓
Create Folder
```

এর মাধ্যমে আপনার প্রয়োজন অনুযায়ী Folder তৈরি করতে পারবেন।

উদাহরণ:

```text
picture
website
assets
projects
```

---

# 📤 File Upload

File Upload করার সময়:

1. Repository নির্বাচন করুন
2. Folder নির্বাচন করুন
3. File নির্বাচন করুন
4. প্রয়োজন হলে File Name নির্ধারণ করুন
5. Upload করুন

PocketHost Studio GitHub REST API ব্যবহার করে File-টি সরাসরি নির্দিষ্ট Repository Folder-এ Upload করবে।

---

# 🖼️ Image Upload

Image Upload-এর ক্ষেত্রেও একই পদ্ধতি অনুসরণ করা যাবে।

উদাহরণ:

```text
picture/
└── myphoto.jpg
```

Upload সম্পন্ন হলে Live URL হবে:

```text
https://username.github.io/repository/picture/myphoto.jpg
```

---

# 🌐 HTML Hosting

আপনার HTML File যদি:

```text
website/index.html
```

পাথে Upload করা হয়, তাহলে GitHub Pages-এর মাধ্যমে সেটি Live Website হিসেবে ব্যবহার করা যাবে।

উদাহরণ:

```text
https://username.github.io/repository/website/
```

অথবা:

```text
https://username.github.io/repository/website/index.html
```

---

# 🔗 Automatic URL Generation

Upload সম্পন্ন হওয়ার পর PocketHost Studio স্বয়ংক্রিয়ভাবে আপনার File-এর Live URL তৈরি করবে।

### 📄 File URL

```text
https://USERNAME.github.io/REPOSITORY/FOLDER/FILENAME
```

### 🖼️ Image URL

```text
https://USERNAME.github.io/REPOSITORY/FOLDER/IMAGE.jpg
```

### 🌐 HTML URL

```text
https://USERNAME.github.io/REPOSITORY/FOLDER/index.html
```

এতে আপনাকে আলাদাভাবে GitHub Repository খুলে File-এর URL খুঁজে বের করতে হবে না।

---

# 📱 Mobile Friendly

PocketHost Studio মূলত Mobile User-এর কথা মাথায় রেখে তৈরি।

এটি ব্যবহার করা যাবে:

* 📱 Android Phone
* 🌐 Mobile Browser
* 💻 Desktop Browser
* 📲 WebView-based App

অর্থাৎ, কম্পিউটার ছাড়াও মোবাইল থেকেই আপনার GitHub Hosting পরিচালনা করা সম্ভব।

---

# 🧩 Architecture

PocketHost Studio-এর মূল প্রযুক্তি:

| Technology      | ব্যবহার                      |
| --------------- | ---------------------------- |
| HTML5           | User Interface               |
| CSS3            | Responsive UI & Design       |
| JavaScript      | Application Logic            |
| GitHub REST API | File & Repository Management |
| GitHub Pages    | Static Hosting               |
| LocalStorage    | Local Configuration Storage  |

---

# 🔒 Privacy & Security

PocketHost Studio-এর মূল Architecture Client-Side হওয়ায় ব্যবহারকারীর GitHub Account-এর সঙ্গে API Communication সরাসরি Browser থেকেই করা হয়।

আপনার Personal Access Token:

```text
Browser
   ↓
Local Storage
   ↓
GitHub API
```

ব্যবহার করা হয়।

### ⚠️ গুরুত্বপূর্ণ নিরাপত্তা সতর্কতা

আপনার Personal Access Token অত্যন্ত গুরুত্বপূর্ণ।

কখনো:

* Public Repository-তে Token রাখবেন না
* Source Code-এর মধ্যে Token লিখে রাখবেন না
* অন্য কাউকে Token দেবেন না
* Screenshot-এ Token প্রকাশ করবেন না

---

# 📜 Terms of Use

## 🕊️ Copyright-Free Project

PocketHost Studio-এর Source Code **Copyright-Free** হিসেবে প্রকাশ করা হয়েছে।

যেকোনো ব্যক্তি নিজের প্রয়োজন অনুযায়ী এই Project:

* ব্যবহার করতে পারবেন
* পরিবর্তন করতে পারবেন
* নিজের Project-এ যুক্ত করতে পারবেন
* Redistribute করতে পারবেন
* নিজের মতো করে Customize করতে পারবেন

কোনো Commercial বা Personal Project-এর জন্যও এটি ব্যবহার করা যাবে।

---

## 🤲 একটি বিশেষ মানবিক শর্ত

এই Project ব্যবহারের আগে প্রত্যেক ব্যবহারকারীকে **কমপক্ষে ৫০ টাকা অথবা তার বেশি** কোনো ভালো কাজে দান করার অনুরোধ/শর্ত রাখা হয়েছে।

দান করা যেতে পারে:

* 🕌 কোনো মসজিদে
* 📚 কোনো মাদ্রাসায়
* 🍚 কোনো অসহায় বা ক্ষুধার্ত মানুষকে
* ❤️ প্রয়োজনগ্রস্ত কোনো ব্যক্তিকে

### ন্যূনতম পরিমাণ

```text
৳50
```

এর বেশি দান করলে কোনো সমস্যা নেই।

এই শর্ত পূরণ না করে কেউ Project ব্যবহার করলে তার সেই সিদ্ধান্তের নৈতিক দায়ভার সম্পূর্ণ তার নিজের।

> ❤️ **কোডটি বিনামূল্যে — তবে এর ব্যবহারের আগে একটি ভালো কাজ করুন।**

---

# 👨‍💻 Developer

### Muhammed Omor

**Developer:** Muhammed Omor
**GitHub:** [@halalcodes](https://github.com/halalcodes)
**Email:** [muhammedomor.studio@gmail.com](mailto:muhammedomor.studio@gmail.com)

---

# 🌐 Official Demo

🔗 **Live Demo:**
https://halalcodes.github.io/pockethost

---

# 📥 Download

PocketHost Studio-এর সম্পূর্ণ Single-File Version:

**Download:**
https://github.com/HalalCodes/pockethost/releases/download/v1.2026.33/index.html

---

# 🚀 Quick Start

```text
1. PocketHost Studio Open করুন
          ↓
2. GitHub Username সেট করুন
          ↓
3. Personal Access Token যুক্ত করুন
          ↓
4. Repository নির্বাচন করুন
          ↓
5. Folder তৈরি করুন
          ↓
6. Image / HTML / File Upload করুন
          ↓
7. Live URL পান
          ↓
8. আপনার File ব্যবহার করুন
```

---

# 💡 কেন PocketHost Studio?

GitHub ব্যবহার করে File Hosting করতে সাধারণত Repository, Folder, File Upload এবং Pages Configuration-এর মতো বিভিন্ন ধাপ অনুসরণ করতে হয়।

**PocketHost Studio** সেই কাজগুলোকে একটি সহজ Mobile-Friendly Interface-এর মধ্যে নিয়ে আসে।

### এক কথায়:

> **GitHub Repository-কে আপনার নিজের Personal Hosting Panel-এ পরিণত করুন। 🚀**

---

## ❤️ Built with GitHub

PocketHost Studio তৈরি করা হয়েছে GitHub-এর শক্তিশালী API এবং GitHub Pages-এর সুবিধা ব্যবহার করে।

**Simple. Free. Mobile-Friendly. Developer-Friendly.**

---

### ⭐ Project Support

Project-টি ভালো লাগলে GitHub Repository-তে ⭐ **Star** দিয়ে Support করতে পারেন।

**Developed with ❤️ by Muhammed Omor**
