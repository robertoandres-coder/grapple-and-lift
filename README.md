# Grapple & Lift Training Website - Setup Guide

## Project Structure

This is a Next.js 15 website with:
- **Home page** (`/`) - Showcases your training program with three pillars
- **Contact page** (`/contact`) - Contact form that emails you directly
- **Styling** - Tailwind CSS for a modern, professional look
- **Email** - Nodemailer integration for sending contact form submissions

## Local Development

1. **Install dependencies:**
   ```
   npm install
   ```

2. **Set up email configuration:**
   - Edit `.env.local` and add your Gmail credentials
   - For Gmail: Use an [App Password](https://support.google.com/accounts/answer/185833)
   - If using another email service, adjust accordingly

3. **Run development server:**
   ```
   npm run dev
   ```
   - Open http://localhost:3000 in your browser

## Deploying to Vercel

1. **Push to GitHub:**
   - Create a GitHub repository
   - Push this project to GitHub

2. **Connect to Vercel:**
   - Go to [vercel.com](https://vercel.com)
   - Sign up or log in
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will auto-detect Next.js

3. **Add Environment Variables:**
   - In Vercel project settings, go to "Environment Variables"
   - Add: `EMAIL_USER` = your email
   - Add: `EMAIL_PASSWORD` = your app password or SMTP password

4. **Deploy:**
   - Click "Deploy"
   - Your site will be live in minutes!

## Customization

### Home Page
Edit `app/page.tsx` to:
- Change colors, fonts, or layout
- Add more details about your program
- Add images or video

### Contact Page
Edit `app/contact/page.tsx` to:
- Customize the form fields
- Add more information

### Email
Edit `app/api/send-email/route.ts` to:
- Change email service (Gmail, SendGrid, etc.)
- Modify email template

## Support

For Next.js docs: https://nextjs.org/docs
For Vercel deployment: https://vercel.com/docs
For Tailwind CSS: https://tailwindcss.com/docs
