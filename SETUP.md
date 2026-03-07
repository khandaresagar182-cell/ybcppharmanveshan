# Pharma Anveshan 2026 — YBCP Sawantwadi Setup Guide

This is a **separate instance** of the Pharma Anveshan website for **Yashwantrao Bhosale College of Pharmacy, Sawantwadi**.
It has its own separate backend and database.

---

## ✅ Already Updated
- College name → Yashwantrao Bhosale College of Pharmacy, Sawantwadi
- Event date → 16th March 2026
- Venue → Sawami Vivekanand Auditorium, Bhonsale Knowledge City, Sawantwadi
- Backend email templates → College name updated
- Package name → `pharmaanveshan-ybcp-sawantwadi-backend`

## 🔧 Still Need to Update

### 1. Logos & Images — `assets/images/`
- Replace `ybcp-logo.png` with your college logo
- Replace `npwa-logo.png` if using a different association logo
- Replace `poster-bg.jpg` with your event background
- Replace `poster.png` with your event poster

### 2. Committee Members — `index.html`
- Update `[Chairman Name]`, `[Secretary Name]`, etc. with actual names
- Add photos to `assets/images/` and update `src` attributes

### 3. Contact Details — `index.html` Footer
- Update `[College Website]`, `[College Email]`, `[College Phone]`
- Add social media links (Instagram, YouTube, etc.)

### 4. Email Domain — `backend/server.js`
- Replace `YOUR-DOMAIN.in` with your actual email domain (for Resend)

### 5. Backend API URL — `js/script.js`
- Replace `https://YOUR-YBCP-BACKEND.up.railway.app` with actual deployed URL

### 6. Environment Variables (Railway)
```
DATABASE_URL=postgresql://user:pass@host:5432/ybcp_db
RESEND_API_KEY=re_xxxxxxxxxxxx
NODE_ENV=production
```

---

## 🚀 Deployment

### Frontend (Vercel)
1. Push this folder to a new GitHub repo
2. Connect it to Vercel
3. Set your custom domain

### Backend (Railway)
1. Push `backend/` to a new GitHub repo
2. Deploy on Railway
3. Add a PostgreSQL database
4. Set environment variables
5. Update `API_URL` in `js/script.js`

---

## 📋 Checklist
- [x] Update college name in `index.html`
- [x] Update event date (16th March)
- [x] Update venue (Sawami Vivekanand Auditorium)
- [x] Update backend email templates
- [x] Replace logos and images
- [x] Update committee members
- [x] Update footer contact details
- [x] Deploy backend & set `API_URL`
- [x] Configure email domain in `server.js` → `ybcppharmaanveshan.in`
- [x] Set environment variables on Railway (DATABASE_URL, NODE_ENV)
- [x] Custom domain `ybcppharmaanveshan.in` added to Vercel
- [ ] Configure Resend API key on Railway (for confirmation emails)
- [ ] Test registration flow end-to-end on live domain
