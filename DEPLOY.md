# Deploy to Vercel - Quick Guide

## 🚀 Method 1: Vercel Dashboard (Drag & Drop) - EASIEST

1. **Go to Vercel Dashboard**
   - Visit: https://vercel.com
   - Sign up or log in with your GitHub account

2. **Deploy via Drag & Drop**
   - Go to: https://vercel.com/new
   - Drag and drop the entire `boat-safari` folder
   - Wait for deployment (usually 1-2 minutes)
   - Your site will be live with a `.vercel.app` URL

3. **Done!** Your site is now live 🎉

---

## 🚀 Method 2: Vercel Dashboard (Git Integration)

1. **Push to Your GitHub Repository**
   - Create your own GitHub repository (or use one you have access to)
   - Push your code:
     ```bash
     git remote remove origin
     git remote add origin https://github.com/YOUR_USERNAME/boat-safari.git
     git push -u origin main
     ```

2. **Connect to Vercel**
   - Go to: https://vercel.com/new
   - Click "Import Git Repository"
   - Select your GitHub repository
   - Click "Import"

3. **Configure Deployment**
   - **Framework Preset**: Select "Other" or leave as default
   - **Root Directory**: Leave as `.` (root)
   - **Build Command**: Leave empty (no build needed)
   - **Output Directory**: Leave empty
   - Click "Deploy"

4. **Done!** Your site will be automatically deployed

---

## 🚀 Method 3: Vercel CLI (If you install Node.js)

1. **Install Node.js** (if not installed)
   - Download from: https://nodejs.org/
   - Install Node.js (this will also install npm)

2. **Install Vercel CLI**
   ```bash
   npm install -g vercel
   ```

3. **Deploy**
   ```bash
   cd c:\Users\PCG\Desktop\OOP\boat-safari
   vercel
   ```
   - Follow the prompts to log in
   - Select "Deploy" when asked
   - Your site will be deployed

4. **Deploy to Production**
   ```bash
   vercel --prod
   ```

---

## ✅ After Deployment

1. **Check Your Site**
   - Visit the URL provided by Vercel
   - Test all pages:
     - `/` - Homepage
     - `/event-detail.html` - Event detail page
     - `/event-listing.html` - Event listing page

2. **Custom Domain (Optional)**
   - Go to your project in Vercel Dashboard
   - Go to Settings → Domains
   - Add your custom domain
   - Follow the DNS configuration instructions

---

## 📝 Notes

- The `vercel.json` file is already configured with proper headers
- No build process is needed - this is a static site
- All files are in the root directory
- Vercel will automatically detect it as a static site

---

## 🔧 Troubleshooting

### If you get a 404 error:
1. Make sure `index.html` is in the root directory ✓
2. Check that `vercel.json` is present ✓
3. Verify all CSS, JS, and image files are in their respective folders ✓
4. Redeploy from Vercel Dashboard

### If assets don't load:
1. Check that file paths are relative (not absolute)
2. Verify all files are committed to Git
3. Check browser console for 404 errors

---

**Need help?** Check Vercel documentation: https://vercel.com/docs

