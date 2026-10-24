# TenWords 📖✨

> **Master vocabulary one day at a time — 100% offline, privacy-first, and beautifully designed for phones, tablets, and large wireless displays.**

[![Platform](https://img.shields.io/badge/Platform-Android%208.0%2B-green.svg)](https://android.com)
[![Version](https://img.shields.io/badge/Version-v2.6%20(Build%2026)-blue.svg)](https://github.com/lazy-4n-2/Tenwords-)
[![License]([!![MIT License](assets/mit.svg)](LICENSE)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose%20%2B%20M3-4285F4.svg)](https://developer.android.com/jetpack/compose)
[![Offline First](https://img.shields.io/badge/Storage-Room%20SQLite%20(Offline)-purple.svg)](https://developer.android.com/training/data-storage/room)

---

## 📌 Table of Contents
- [Why TenWords?](#-why-tenwords)
- [Key Highlights](#-key-highlights)
- [Core Features & How to Use Them](#-core-features--how-to-use-them)
  - [1. Dictionary & Word Finder (Launch Screen)](#1-dictionary--word-finder-launch-screen)
  - [2. Daily Learning & Habit Tracker](#2-daily-learning--habit-tracker)
  - [3. Interactive Lesson Activity Calendar](#3-interactive-lesson-activity-calendar)
  - [4. Smart Quizzes & Flashcards](#4-smart-quizzes--flashcards)
  - [5. Pronunciation (Text-to-Speech)](#5-pronunciation-text-to-speech)
  - [6. English & Bengali Bilingual Experience](#6-english--bengali-bilingual-experience)
- [Adaptive Large & Wireless Screen Support](#-adaptive-large--wireless-screen-support)
- [Complete Offline Architecture](#-complete-offline-architecture)
- [Backup & Restore Guide](#-backup--restore-guide)
  - [How to Export a Backup](#how-to-export-a-backup)
  - [How to Restore from a Backup](#how-to-restore-from-a-backup)
- [Tech Stack](#-tech-stack)
- [Feature Requests & Bug Reporting](#-feature-requests--bug-reporting)

---

## 💡 Why TenWords?

Most dictionary and vocabulary apps bombard you with intrusive ads, paywalls, mandatory account registrations, and heavy tracking scripts that stop working the moment you go into airplane mode or lose network connectivity.

**TenWords was built with a different philosophy:**
1. **Zero Distractions & Zero Ads:** No popups, banners, or subscriptions.
2. **True Privacy:** No accounts, no telemetry, no analytics. Your data lives exclusively on your device.
3. **100% Offline Durability:** Everything you save is backed by a local **Room SQLite** database.
4. **Adaptive Multitasking:** Runs seamlessly on compact smartphones, folding phones, Android tablets, Chromebooks, and wireless cast displays.
5. **Human Pace:** Learn 5–10 meaningful words every day without cognitive overload.

---

## 🌟 Key Highlights

- **Direct-to-Dictionary Startup:** Opens immediately into search so you can look up words in under a second.
- **Accurate Human-Curated Definitions:** Nuanced Bengali and English translations with parts of speech, phonetics, and contextual examples.
- **Collapsible Activity Shutter:** A clean calendar dropdown that lets you inspect your learning history without cluttering the screen.
- **Flexible Learning Modes:** Switch between goal-oriented streak tracking (e.g. 5 or 10 words daily) or relaxed, open-ended exploration.
- **Universal Backup System:** Export your entire vocabulary repository as a clean JSON file or copy it directly to your clipboard.

---

## 🚀 Core Features & How to Use Them

### 1. Dictionary & Word Finder (Launch Screen)
The app starts directly in the **Dictionary** tab so you can immediately find or learn words.
- **How to use:**
  1. Type any English word into the search bar.
  2. Instant auto-suggestions will appear as you type.
  3. View accurate definitions, phonetic transcriptions, grammatical parts of speech, synonyms, antonyms, and bilingual Bengali meanings.
  4. Tap the **Add to My Vocabulary** button to save it to your personal learning collection.

### 2. Daily Learning & Habit Tracker
Build a sustainable daily habit using curated daily sets or your own custom words.
- **How to use:**
  - Navigate to the **Today** tab to see your current words for the day.
  - Review definitions, hear audio pronunciations, and see where you first learned the word (book, podcast, chat, article).
  - Check your **Streak Counter (🔥)** at the top of the screen to stay motivated each consecutive day.
  - *Casual Mode:* If you prefer studying at your own pace without daily quota notifications, toggle **Casual Learning Mode** in Settings.

### 3. Interactive Lesson Activity Calendar
Track which days you studied with an elegant, collapsible shutter calendar.
- **How to use:**
  - On the **Today** screen, tap the **Lesson Activity Calendar** bar.
  - It opens smoothly like a shutter to reveal a monthly calendar grid with dots highlighting every active lesson day.
  - Tap any past date to view exactly which words you mastered on that specific day.
  - Tap the header bar again to collapse the shutter and keep your interface neat.

### 4. Smart Quizzes & Flashcards
Solidify your long-term memory through active recall.
- **How to use:**
  - Open the **Quiz** tab.
  - Choose between multiple-choice meaning quizzes or quick flashcard flips.
  - Answer questions to measure retention and review words that require extra practice.

### 5. Pronunciation (Text-to-Speech)
- Tap the **Speaker 🔊** icon on any word card to hear accurate audio pronunciation powered locally by your device's Android Text-to-Speech engine.

### 6. English & Bengali Bilingual Experience
- **English by Default:** Clean English interface for global learners.
- **One-Tap Language Toggle:** Easily switch the entire app interface and meanings to Bengali (বাংলা) directly from Settings.

---

## 🖥️ Adaptive Large & Wireless Screen Support

TenWords is built using responsive Jetpack Compose container-based design:

- **Smartphones (Compact Mode):** Standard ergonomic bottom navigation bar with fluid vertical scrolling.
- **Tablets, Foldables & Large Screens (Expanded Mode):** 
  - Automatically transitions from a bottom bar to an ergonomic **NavigationRail**.
  - Expands into multi-pane and wider cards with centered content containers (`widthIn(max = 600.dp)`) so text never stretches awkwardly.
- **Wireless Displays & Casting:**
  - Fully compatible with Android Desktop Mode (Samsung DeX, Motorola Ready For) and wireless cast monitors/TVs.
  - Supports mouse, trackpad, and physical keyboard navigation.

---

## 🔒 Complete Offline Architecture

| Component | Offline Status | Details |
|---|---|---|
| **Database** | ✅ 100% Offline | Stored locally on device using Room SQLite (`tenwords_database.db`). |
| **Starter Vocabulary** | ✅ 100% Offline | Bundled with rich, verified academic and everyday English words. |
| **Streaks & Progress** | ✅ 100% Offline | Computed on-device from your local lesson timestamps. |
| **Audio Pronunciation**| ✅ 100% Offline | Powered by Android's local device TTS engine (no internet streaming). |
| **Backup & Restore**  | ✅ 100% Offline | Generates local JSON files without cloud server involvement. |
| **Extended Online Lookup** | 🌐 Optional | If you search for an obscure word not in the built-in offline set, you can connect online to query the Free Dictionary API. |

---

## 💾 Backup & Restore Guide

Your learning progress should never be lost when upgrading or switching devices. TenWords gives you 100% control over your data.

### How to Export a Backup
1. Open the **Settings ⚙️** tab.
2. Scroll to the **Backup & Restore (অফলাইন ডাটা)** section.
3. You have two convenient options:
   - **Option A (Export File):** Tap **Export Backup (ব্যাকআপ সংরক্ষণ)**. Choose a folder on your device or SD card (e.g. `Downloads` or `Documents`) to save `TenWords_Backup_YYYYMMDD.json`.
   - **Option B (Copy JSON):** Tap **Copy JSON (JSON কপি করুন)** to copy the complete raw backup payload directly to your clipboard. You can paste it into a safe note or send it to your email/drive.

### How to Restore from a Backup
1. Install or open TenWords on your target device.
2. Open the **Settings ⚙️** tab and go to **Backup & Restore**.
3. Tap **Import Backup Data (ব্যাকআপ রিস্টোর করুন)**.
4. Select your previously saved `.json` file or paste your backup JSON text.
5. The app instantly verifies the data structure and restores all your words, notes, categories, and progress seamlessly!

---

## 🛠️ Tech Stack

- **Language:** [Kotlin 2.0+](https://kotlinlang.org)
- **UI Toolkit:** [Jetpack Compose](https://developer.android.com/jetpack/compose) with Material Design 3 (M3)
- **Local Persistence:** [Android Jetpack Room](https://developer.android.com/training/data-storage/room) (SQLite)
- **Architecture:** MVVM (Model-View-ViewModel) + Kotlin Coroutines & StateFlow
- **Audio Engine:** Android Native `TextToSpeech`
- **Network (Optional):** OkHttp3 + JSON Parser (graceful offline fallback)

---

## 🤝 Feature Requests & Bug Reporting

We welcome community feedback and suggestions! If you encounter an issue, find a bug, or have an idea for a new feature:

👉 **Report it directly on our GitHub Issues page:**  
[**https://github.com/lazy-4n-2/Tenwords-**](https://github.com/lazy-4n-2/Tenwords-)
