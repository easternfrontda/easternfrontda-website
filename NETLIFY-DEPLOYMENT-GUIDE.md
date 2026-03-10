# 🚀 NETLIFY DEPLOYMENT GUIDE
## Eastern Front Defense Academy Website

**Date:** March 10, 2026  
**Domain:** easternfrontda.com  
**Status:** Ready to Deploy ✅

---

## 📦 WHAT YOU'RE DEPLOYING

### Website Files (31 HTML Pages):
✅ **Main Pages (9):**
- index.html (Homepage)
- about.html (About/Instructor)
- courses.html (Course Catalog)
- blog.html (Blog Hub)
- contact.html (Contact Form)
- book.html (Booking Page)
- faq.html (FAQ)
- gallery.html (Photo Gallery)
- gifts.html (Gift Certificates)

✅ **Course Pages (13):**
- Pistol: p1-pistol-safety.html → p5-advanced-defensive.html
- Rifle: r1-rifle-safety.html → r5-advanced-rifle.html
- Specialty: s1-tactical-medical.html → s3-situational-awareness.html

✅ **Blog Posts (3):**
- blog-ukraine-lessons.html
- blog-new-gun-owner.html
- blog-fort-wayne-guide.html

✅ **Legal Pages (3):**
- privacy-policy.html
- terms-conditions.html
- waiver.html

✅ **Assets:**
- css/new-theme.css (main stylesheet)
- css/styles.css (backup)
- js/main.js (JavaScript)
- images/logo-full.png
- images/logo-transparent.svg

✅ **Contact Information (Already Updated):**
- Phone: (260) 209-4178
- Email: info@easternfrontda.com
- Domain: easternfrontda.com

---

## 🎯 STEP-BY-STEP DEPLOYMENT

### **STEP 1: CREATE DEPLOYMENT FOLDER**

**On Your Computer:**
1. Create a new folder on your desktop called `EFDA-Website`
2. Inside that folder, you need these files and folders:

```
EFDA-Website/
├── index.html
├── about.html
├── courses.html
├── blog.html
├── contact.html
├── book.html
├── faq.html
├── gallery.html
├── gifts.html
├── p1-pistol-safety.html
├── p2-marksmanship-basics.html
├── p3-defensive-pistol.html
├── p4-concealed-carry.html
├── p5-advanced-defensive.html
├── r1-rifle-safety.html
├── r2-defensive-rifle.html
├── r3-tactical-movement.html
├── r4-cqb.html
├── r5-advanced-rifle.html
├── s1-tactical-medical.html
├── s2-home-defense.html
├── s3-situational-awareness.html
├── blog-ukraine-lessons.html
├── blog-new-gun-owner.html
├── blog-fort-wayne-guide.html
├── privacy-policy.html
├── terms-conditions.html
├── waiver.html
├── css/
│   ├── new-theme.css
│   └── styles.css
├── js/
│   └── main.js
└── images/
    ├── logo-full.png
    └── logo-transparent.svg
```

**NOTE:** You can download all files from this project using the file browser on the left side of this interface.

---

### **STEP 2: SIGN UP FOR NETLIFY**

1. Go to: **https://www.netlify.com**
2. Click **"Sign up"** (top right)
3. Choose **"Email"** option
4. Use your business email: **info@easternfrontda.com**
5. Create a strong password
6. Verify your email (check inbox)

---

### **STEP 3: DEPLOY YOUR SITE**

**Option A: Drag-and-Drop (EASIEST)**
1. Log into Netlify
2. You'll see: **"Want to deploy a new site without connecting to Git? Drag and drop your site output folder here"**
3. **Drag the entire `EFDA-Website` folder** onto the Netlify window
4. Wait 30-60 seconds while it uploads
5. **Done!** Your site is live at: `https://random-name-12345.netlify.app`

**Option B: Manual Upload**
1. Click **"Add new site"** → **"Deploy manually"**
2. Drag your `EFDA-Website` folder
3. Wait for deployment
4. Site goes live

---

### **STEP 4: TEST YOUR LIVE SITE**

Netlify will give you a temporary URL like:
- `https://magnificent-paprenjak-a1b2c3.netlify.app`

**Test these things:**
1. ✅ Homepage loads correctly
2. ✅ Navigation menu works (all links)
3. ✅ Course pages load
4. ✅ Blog posts display properly
5. ✅ Contact form appears (won't send emails yet - we'll fix that)
6. ✅ Footer links work
7. ✅ Phone number shows: (260) 209-4178
8. ✅ Email shows: info@easternfrontda.com
9. ✅ Mobile version looks good (resize browser window)

**If something is broken:** Let me know and I'll help fix it!

---

### **STEP 5: CONNECT YOUR DOMAIN (easternfrontda.com)**

**In Netlify Dashboard:**
1. Click on your site name
2. Go to **"Domain settings"**
3. Click **"Add custom domain"**
4. Enter: **easternfrontda.com**
5. Click **"Verify"**
6. Netlify will ask: **"Do you own this domain?"** → Click **"Yes, add domain"**

**You'll see a warning:** "Check DNS configuration"

---

### **STEP 6: UPDATE YOUR DOMAIN DNS**

You need to point your domain to Netlify. This varies by domain registrar:

#### **Where did you buy easternfrontda.com?**
- GoDaddy
- Namecheap
- Google Domains
- Other?

**General DNS Setup (works for most registrars):**

1. Log into your domain registrar (where you bought easternfrontda.com)
2. Find **DNS Settings** or **DNS Management**
3. Look for **"A Record"** or **"DNS Records"**
4. **Delete any existing A records** for `@` or `easternfrontda.com`
5. **Add new A record:**
   - **Type:** A
   - **Name:** @ (or leave blank)
   - **Value:** `75.2.60.5` (Netlify's IP)
   - **TTL:** 3600 (or "Automatic")
6. **Add CNAME record for www:**
   - **Type:** CNAME
   - **Name:** www
   - **Value:** `YOUR-SITE-NAME.netlify.app` (from Step 4)
   - **TTL:** 3600

**Save changes.**

**⏰ Wait Time:** DNS changes take 1-48 hours (usually 2-4 hours)

---

### **STEP 7: ENABLE HTTPS (FREE SSL)**

Netlify automatically provides free HTTPS once your domain is connected.

**After DNS propagates (2-4 hours):**
1. Go back to Netlify → Domain settings
2. Scroll to **"HTTPS"**
3. You'll see: **"Awaiting DNS propagation"** → then → **"Provisioning certificate"**
4. After a few minutes: **"Certificate active"** ✅
5. Enable **"Force HTTPS"** (redirects http:// to https://)

**Your site will be:**
- https://easternfrontda.com ✅
- https://www.easternfrontda.com ✅

---

## 🔧 AFTER DEPLOYMENT

### **1. Set Up Form Notifications**

Your contact forms currently open email (mailto:). To get form submissions in Netlify:

**In Netlify Dashboard:**
1. Go to **"Forms"**
2. Click **"Enable form detection"**
3. Add **"Form notifications"** → **"Email notification"**
4. Enter: **info@easternfrontda.com**

(We can set this up after deployment)

---

### **2. Set Up Google Analytics (Optional)**

Track your website visitors:

1. Go to: https://analytics.google.com
2. Create account for easternfrontda.com
3. Get tracking code
4. Add to all HTML pages (I can help with this)

---

### **3. Submit to Google Search Console**

Help Google find your site:

1. Go to: https://search.google.com/search-console
2. Add property: easternfrontda.com
3. Verify ownership (Netlify makes this easy)
4. Submit sitemap (I can create one for you)

---

## 📊 DEPLOYMENT CHECKLIST

**Before You Start:**
- [ ] Download all website files from this project
- [ ] Create `EFDA-Website` folder with proper structure
- [ ] Have domain login information ready (easternfrontda.com registrar)

**Deployment Steps:**
- [ ] Sign up for Netlify account
- [ ] Upload website folder to Netlify
- [ ] Test temporary Netlify URL
- [ ] Add custom domain (easternfrontda.com)
- [ ] Update DNS records at domain registrar
- [ ] Wait for DNS propagation (2-4 hours)
- [ ] Enable HTTPS/SSL
- [ ] Test live site at easternfrontda.com
- [ ] Set up form notifications
- [ ] Submit to Google Search Console

**Post-Launch:**
- [ ] Request Google Business verification postcard
- [ ] Publish Instagram posts
- [ ] Create Facebook Business Page
- [ ] Start accepting bookings!

---

## 🆘 TROUBLESHOOTING

### **"My site isn't loading after DNS change"**
- Wait 2-4 hours for DNS propagation
- Clear browser cache (Ctrl+F5)
- Try incognito/private browsing window
- Check DNS propagation: https://dnschecker.org

### **"Images/CSS not loading"**
- Check file paths are correct
- Make sure you uploaded the `css/`, `js/`, and `images/` folders
- File names are case-sensitive (use exact names)

### **"Contact form isn't working"**
- This is expected initially
- We'll set up Netlify Forms after deployment
- Or we can connect to an external form service

### **"HTTPS not working"**
- Wait 10-20 minutes after DNS propagates
- Netlify automatically provisions SSL
- Check Netlify dashboard → Domain settings → HTTPS

---

## 📞 NEED HELP?

If you get stuck at any step, just tell me:
1. Which step you're on
2. What you see on your screen
3. Any error messages

I'll guide you through it!

---

## 🎉 ESTIMATED TIMELINE

- **File preparation:** 10 minutes
- **Netlify signup:** 5 minutes
- **Upload & deploy:** 2 minutes
- **Testing:** 10 minutes
- **DNS setup:** 10 minutes
- **DNS propagation wait:** 2-4 hours
- **HTTPS setup:** Automatic (5 minutes)

**Total active work time:** ~40 minutes  
**Total time to live site:** 3-5 hours (including DNS wait)

---

**You're ready to go! Start with Step 1 and let me know when you're ready for the next step.** 🚀
