# BTM Designs — Setup Guide

## 📁 Files
- `btm-public.html` — Public website (visitor-facing)
- `btm-admin.html` — Admin dashboard (owner only)

## 🚀 Quick Start

### Option 1 — Local (Simplest)
1. Download both HTML files to the **same folder**
2. Open `btm-public.html` in your browser → Public site
3. Open `btm-admin.html` in your browser → Admin panel
4. Both files share the **same localStorage**, so admin changes appear on the public site immediately

### Option 2 — Web Hosting (Recommended)
Upload both files to any static host:
- **Netlify** (free): drag-and-drop both files at netlify.com
- **GitHub Pages**: create a repo, push both files, enable Pages
- **Vercel**: same as Netlify
- **Your own server**: place both files in the same directory

---

## 🔐 Admin Access
- URL: `btm-admin.html`
- Password: `BTM2026BTM/*/ZINTOX18@TRT`
- Session persists until browser tab/window is closed

---

## 🌐 Features

### Public Website
- Sticky header with BTM gold logo
- Hero section (content editable from admin)
- Portfolio gallery with filters (All / T-Shirts / Drawings / Logos / Newest)
- Full-screen lightbox for each item
- Categories section with item counts
- About the Artist section
- Contact section
- Footer with admin link

### Admin Dashboard
- Secure login page
- Overview stats (total designs, featured, per category)
- Portfolio management (Add / Edit / Delete)
- Hero section editor (EN + AR)
- About section editor (EN + AR)
- Site Settings (email, Instagram, taglines)
- Preview public site button

### Bilingual Support
- Full Arabic + English with RTL layout
- Language switcher on both sites
- All content editable in both languages via admin

---

## 🔄 How Data Syncs
Both files use **localStorage** (browser storage) with key `btm_designs_data`.
- Any save in Admin → instantly reflected in Public Site (same browser)
- For multi-device sync → upgrade to a backend (see below)

## ⬆️ Upgrade to Real Backend (Optional)
For production with multiple devices, replace the localStorage calls with:
- **Firebase Firestore** (free tier available)
- **Supabase** (free tier, PostgreSQL)
- **Airtable API**

The data structure is ready — just swap `localStorage.getItem/setItem` with your API calls.

---

## 🎨 Customization
- Colors: Edit CSS `:root` variables at the top of each file
- Fonts: Change Google Fonts imports
- Logo: Replace the SVG in the hero section or upload via Settings
- Add portfolio items: Admin → Portfolio → Add Design

---

## 📞 Support
BTM Designs © 2026
