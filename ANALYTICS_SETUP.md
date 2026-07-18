# Google Analytics Setup Guide

## 🔒 Security Implementation

This setup uses **GitHub Secrets** to securely store your Google Analytics tracking ID, keeping it out of your public repository.

## 📋 Setup Steps

### 1. Create Google Analytics Property
1. Go to [Google Analytics](https://analytics.google.com/)
2. Create a new GA4 property for your website
3. Copy your **Measurement ID** (format: `G-XXXXXXXXXX`)

### 2. Add Secret to GitHub Repository
1. Go to your repository on GitHub
2. Navigate to **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret**
4. Name: `GOOGLE_ANALYTICS_ID`
5. Value: Your GA4 Measurement ID (e.g., `G-XXXXXXXXXX`)
6. Click **Add secret**

### 3. Deploy Your Site
1. Push your changes to the `main` branch
2. GitHub Actions will automatically build and deploy
3. Your analytics will start tracking immediately

## 📊 Analytics Features Implemented

### Basic Analytics
- ✅ Page views and sessions
- ✅ Traffic sources and geographic data
- ✅ Device/browser information
- ✅ Bounce rate and session duration

### Advanced Analytics
- ✅ Custom events for user interactions
- ✅ External link click tracking
- ✅ File download tracking (PDFs)
- ✅ Scroll depth measurement
- ✅ Time on page tracking
- ✅ IP anonymization for privacy

### Content Analytics
- ✅ Publication performance tracking
- ✅ Project engagement metrics
- ✅ Event/talk popularity
- ✅ Content type categorization
- ✅ Author and publication metadata

## 🎯 Custom Events Tracked

| Event | Description | Data Collected |
|-------|-------------|----------------|
| `click_external_link` | External link clicks | URL, link text, category |
| `file_download` | PDF downloads | File name, type, link text |
| `scroll_depth` | Page engagement | Scroll percentage |
| `time_on_page` | User engagement | Time in seconds |
| `view_publication` | Publication views | Title, type, authors, year |
| `view_project` | Project views | Title, tags |
| `view_event` | Event views | Title, date |

## 🔍 Viewing Your Analytics

1. Go to [Google Analytics](https://analytics.google.com/)
2. Select your property
3. Navigate to **Reports** → **Realtime** for live data
4. Use **Events** section to see custom events
5. Create custom reports for deeper insights

## 🛡️ Privacy & Security

- ✅ **IP Anonymization**: Enabled for GDPR compliance
- ✅ **Secret Management**: Tracking ID stored securely in GitHub Secrets
- ✅ **No Public Exposure**: Tracking ID never appears in repository
- ✅ **Enhanced Measurement**: Automatic event tracking enabled

## 🚀 Next Steps

1. **Set up the secret** as described above
2. **Deploy your site** to start collecting data
3. **Wait 24-48 hours** for initial data to appear
4. **Create custom reports** in GA4 for your specific needs
5. **Set up goals** for important actions (downloads, contact form submissions)

## 🔧 Troubleshooting

### Analytics Not Working?
1. Check that the secret `GOOGLE_ANALYTICS_ID` is set correctly
2. Verify the tracking ID format (should start with `G-`)
3. Check browser developer tools for any JavaScript errors
4. Ensure the site is deployed (not just local development)

### No Data Appearing?
1. Wait 24-48 hours for initial data
2. Check the **Realtime** report in GA4
3. Verify the tracking code is present in page source
4. Test with multiple browsers/devices

## 📈 Advanced Configuration

### Custom Dimensions (Optional)
You can add custom dimensions in GA4 to track:
- Content categories
- User types (student, researcher, industry)
- Content difficulty levels
- Publication impact metrics

### Goals and Conversions
Set up goals for:
- Resume downloads
- Contact form submissions
- Publication views
- Project page visits

---

**Note**: This implementation is production-ready and follows Google Analytics best practices for academic and professional websites.



