# Brasha Moments Wellness Website

Professional mental health and addiction recovery services website for Brasha Moments Wellness in Nairobi, Kenya.

## 🌟 Features

- **Modern, Clean Design**: Professional aesthetic with custom typography and color scheme
- **Fully Responsive**: Optimized for all devices (desktop, tablet, mobile)
- **24/7 Crisis Banner**: Prominent emergency support contact
- **Interactive Navigation**: Smooth scrolling and mobile-friendly menu
- **Comprehensive Sections**:
  - Hero section with key stats
  - About Us with CEO message
  - 6 Service offerings
  - Intervention plan overview
  - 5-step recovery journey timeline
  - 3 pricing packages
  - 4-step admission process
  - Contact form with appointment booking
- **Accessibility**: Semantic HTML and keyboard navigation support
- **SEO Optimized**: Meta tags and structured content
- **Performance**: Optimized loading and animations

## 📁 Project Structure

```
brasha-moments-wellness/
├── index.html          # Main HTML file
├── styles.css          # CSS styling
├── script.js           # JavaScript functionality
├── vercel.json         # Vercel deployment configuration
└── README.md           # This file
```

## 🚀 Deployment to Vercel (Free)

### Option 1: Deploy via Vercel Dashboard (Easiest)

1. **Create a Vercel Account**
   - Go to [vercel.com](https://vercel.com)
   - Sign up with GitHub, GitLab, or Bitbucket

2. **Create a New Project**
   - Click "Add New" → "Project"
   - Choose "Import Git Repository" or "Deploy from Template"

3. **Upload Your Files**
   - If using GitHub: Push these files to a repository, then import it
   - If deploying directly: Use Vercel CLI (see Option 2)

4. **Configure Settings**
   - Framework Preset: Other
   - Root Directory: ./
   - Build Command: (leave empty)
   - Output Directory: ./

5. **Deploy**
   - Click "Deploy"
   - Your site will be live at: `https://your-project-name.vercel.app`

### Option 2: Deploy via Vercel CLI (Recommended)

1. **Install Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**
   ```bash
   vercel login
   ```

3. **Deploy**
   Navigate to your project folder and run:
   ```bash
   vercel
   ```
   
   Follow the prompts:
   - Set up and deploy: Y
   - Which scope: (select your account)
   - Link to existing project: N
   - Project name: brasha-moments-wellness (or your choice)
   - Directory: ./
   - Override settings: N

4. **Production Deployment**
   ```bash
   vercel --prod
   ```

5. **Your Website URL**
   After deployment, you'll get a URL like:
   - `https://brasha-moments-wellness.vercel.app`

### Option 3: GitHub Integration (Best for Updates)

1. **Create GitHub Repository**
   - Go to [github.com](https://github.com)
   - Create a new repository named `brasha-moments-wellness`

2. **Push Code to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/brasha-moments-wellness.git
   git push -u origin main
   ```

3. **Import to Vercel**
   - Go to [vercel.com/new](https://vercel.com/new)
   - Import your GitHub repository
   - Click "Deploy"

4. **Automatic Updates**
   - Every time you push to GitHub, Vercel will auto-deploy
   - Changes are live in seconds

## 🔧 Customization

### Update Contact Information
Edit `index.html` and search for:
- Phone: `+254 763 400 917`
- Email: `brashamomentswellness@gmail.com`
- LinkedIn: Update the URL in the contact section

### Change Colors
Edit `styles.css` variables at the top:
```css
:root {
    --primary: #0A2463;        /* Main brand color */
    --accent: #FB8B24;         /* Accent color */
    /* Adjust other colors as needed */
}
```

### Modify Services
Edit the services section in `index.html` to add/remove/modify service offerings.

### Update Pricing
Edit the pricing section in `index.html` to change packages and prices.

## 📧 Form Submission Setup

The contact form currently simulates submission. To connect it to a real backend:

### Option 1: Email Service (Formspree - Free)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form
3. Update the form in `script.js`:
   ```javascript
   const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
       method: 'POST',
       body: JSON.stringify(formData),
       headers: { 'Content-Type': 'application/json' }
   });
   ```

### Option 2: Google Sheets (Free)
Use Google Apps Script to save form submissions to a spreadsheet.

### Option 3: Custom Backend
Integrate with your own backend API or email service.

## 🌐 Custom Domain Setup

To use a custom domain (e.g., brashamoments.co.ke):

1. **Purchase Domain**
   - Buy from Namecheap, GoDaddy, or Kenya Web Experts

2. **Add to Vercel**
   - Go to Project Settings → Domains
   - Add your domain
   - Update DNS records as instructed

3. **DNS Configuration**
   Add these records to your domain:
   - Type: A, Name: @, Value: 76.76.21.21
   - Type: CNAME, Name: www, Value: cname.vercel-dns.com

## 🔒 SSL Certificate

Vercel automatically provides free SSL certificates for all domains, including custom ones.

## 📊 Analytics Setup (Optional)

Add Google Analytics:
1. Get tracking ID from [analytics.google.com](https://analytics.google.com)
2. Add before `</head>` in `index.html`:
   ```html
   <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
   <script>
     window.dataLayer = window.dataLayer || [];
     function gtag(){dataLayer.push(arguments);}
     gtag('js', new Date());
     gtag('config', 'GA_MEASUREMENT_ID');
   </script>
   ```

## 🐛 Troubleshooting

**Issue**: Form doesn't submit
- **Solution**: Check console for errors, implement real form backend

**Issue**: Images not loading
- **Solution**: Ensure image paths are correct and files are uploaded

**Issue**: Mobile menu not working
- **Solution**: Clear browser cache, check JavaScript console

**Issue**: Styling broken
- **Solution**: Verify CSS file is loading, check browser compatibility

## 📱 Testing

Test your website on:
- Desktop browsers (Chrome, Firefox, Safari, Edge)
- Mobile devices (iOS Safari, Android Chrome)
- Tablet devices
- Different screen sizes

## 🔄 Updates

To update your live website:
1. Make changes to your files
2. If using GitHub: Push changes
3. If using CLI: Run `vercel --prod`
4. Changes are live immediately

## 📞 Support

For technical support with the website:
- Vercel Documentation: [vercel.com/docs](https://vercel.com/docs)
- Contact: brashamomentswellness@gmail.com

## 📄 License

© 2026 Brasha Moments Wellness. All rights reserved.

---

**Website URL**: https://brasha-moments-wellness.vercel.app (after deployment)

**Deployment Date**: February 2026

**Version**: 1.0.0