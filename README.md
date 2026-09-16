# \# GermanMitAbid A1 - 33 Lessons German LMS 🇩🇪

# 

# !\[Live](https://img.shields.io/badge/Live-GitHub%20Pages-success) !\[Status](https://img.shields.io/badge/Status-LIVE-brightgreen) !\[Lessons](https://img.shields.io/badge/Lessons-33-blue) !\[Cards](https://img.shields.io/badge/Cards-400%2B-orange)

# 

# \### 🌐 Live Links

# \- \*\*GitHub Pages (Permanent):\*\* https://syedfoodc-png.github.io/GermanMitAbid-A1/

# \- \*\*Netlify (Backup):\*\* https://mellifluous-souffle-d363fd.netlify.app

# \- \*\*GitHub Repo:\*\* https://github.com/syedfoodc-png/GermanMitAbid-A1

# 

# \---

# 

# \### 🎯 Project Overview - KT Document

# \*\*GermanMitAbid A1\*\* is a complete A1 Level German Learning Management System (LMS) built as a single static HTML file. Designed to teach German from scratch with interactive cards, full German voice, and GRID-based lesson navigation.

# 

# \*\*Problem Solved:\*\* Needed a lightweight, fast, offline-capable German course for students without backend dependency.

# 

# \*\*Solution:\*\* 1 File = 44KB = 33 Lessons = 400+ Cards = Full Voice = 100% Working.

# 

# \---

# 

# \### 🚀 Features

# 

# \#### 1. 33 GRID UI System

# \- \*\*4 Columns Responsive Grid\*\* - Desktop: 4, Tablet: 2, Mobile: 1

# \- \*\*Hover Animation\*\* - Scale + Shadow on hover

# \- \*\*Color Coded Cards\*\* - Each lesson has unique gradient + icon

# \- \*\*Click → Full Syllabus Inside\*\* - Each card expands to show full A1 content

# 

# \#### 2. 400+ Interactive Learning Cards

# \- Alphabet (26 Letters A-Z with examples)

# \- Numbers (0-1000+)

# \- Greetings, Articles, Verbs, Family, Colors, Time, Food, Shopping, Body, House

# \- Grammar: sein/haben/werden, kein/nicht/nein, Possessive, Pronouns, W-Fragen, Articles Cases

# 

# \#### 3. Full German Voice System - Core Innovation

# \- \*\*Web Speech API\*\* with `de-DE` language

# \- \*\*Fixed Double Voice Bug:\*\* Implemented debounce logic

# ```javascript

# let lastText = "";

# let lastTime = 0;

# function speakGerman(text) {

# &#x20; const now = Date.now();

# &#x20; if (text === lastText \&\& now - lastTime < 1500) return; // Block double trigger

# &#x20; lastText = text; lastTime = now;

# &#x20; const msg = new SpeechSynthesisUtterance(text);

# &#x20; msg.lang = 'de-DE'; msg.rate = 0.9;

# &#x20; speechSynthesis.speak(msg);

# }

