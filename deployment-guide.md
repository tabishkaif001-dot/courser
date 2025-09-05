# Deployment Guide

## GitHub Pages Deployment

### Step-by-Step Instructions

1. **Create GitHub Repository**
   - Go to GitHub and create a new repository
   - Name it `course-selling-platform` or your preferred name
   - Make it public (required for free GitHub Pages)

2. **Clone and Setup**

3. **Add Your Files**
- Copy all the application files to your repository
- Update `yourusername` in package.json with your GitHub username

4. **Initial Commit**

5. **Enable GitHub Pages**
- Go to repository Settings
- Navigate to Pages section
- Select "Deploy from a branch"
- Choose "main" branch and "/ (root)" folder
- Save settings

6. **Access Your Live Site**
- Site will be available at: https://yourusername.github.io/course-selling-platform
- May take 2-3 minutes to deploy

### Alternative: Using gh-pages Package

1. **Install gh-pages**

2. **Deploy with Command**

## Other Deployment Options

### Vercel Deployment
1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow prompts

### Netlify Deployment
1. Drag and drop your folder to Netlify
2. Or connect your GitHub repository
3. Auto-deploy on every push

### Firebase Hosting
1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize: `firebase init hosting`
4. Deploy: `firebase deploy`

## Custom Domain Setup

### GitHub Pages Custom Domain
1. Add CNAME file to your repository root
2. Add your domain name to the file
3. Configure DNS settings with your domain provider

### DNS Configuration
- Add A records pointing to GitHub Pages IPs:
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

## SSL Certificate

GitHub Pages provides automatic HTTPS for:
- github.io domains
- Custom domains (may take up to 24 hours)

## Environment Configuration

### Production Settings
- Update API URLs if using backend
- Configure payment gateway settings
- Set production analytics IDs
- Enable production error logging

### Performance Optimization
- Minify CSS and JavaScript for production
- Optimize images
- Enable caching headers
- Use CDN for assets

## Troubleshooting

### Common Issues
1. **404 Error**: Check file paths and case sensitivity
2. **Blank Page**: Check browser console for JavaScript errors
3. **Styling Issues**: Verify CSS file paths
4. **Mobile Issues**: Test responsive design on actual devices

### Debug Steps
1. Test locally first
2. Check browser developer tools
3. Verify all file paths are correct
4. Ensure no hardcoded localhost URLs

## Monitoring

### Analytics Setup
- Add Google Analytics
- Monitor user behavior
- Track conversion rates
- Set up error tracking

### Performance Monitoring
- Use Lighthouse for performance audits
- Monitor Core Web Vitals
- Set up uptime monitoring
- Track loading speeds

## Security Considerations

### Best Practices
- Never commit sensitive data
- Use environment variables for API keys
- Implement proper input validation
- Enable HTTPS only
- Regular security audits

### Content Security Policy
Add CSP headers for enhanced security:
