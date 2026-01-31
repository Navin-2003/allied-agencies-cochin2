# GitHub Repository Setup Guide

This guide will help you properly set up your Allied Agencies Cochin website on GitHub Pages.

## Step 1: Create GitHub Repository

1. **Go to GitHub** and create a new repository
2. **Repository name**: Use a descriptive name like `allied-agencies-cochin` or `water-pump-website`
3. **Visibility**: Choose **Public** (required for free GitHub Pages hosting)
4. **Initialize**: Do NOT initialize with README, .gitignore, or license (we already have these files)

## Step 2: Push Your Code

### Option A: Command Line (Recommended)

```bash
# Navigate to your project directory
cd /path/to/your/project

# Initialize git
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Allied Agencies Cochin website with GitHub Actions"

# Create and switch to main branch
git branch -M main

# Add remote origin (replace with your repository URL)
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git push -u origin main
```

### Option B: GitHub Desktop

1. Open GitHub Desktop
2. Click "File" → "Add Local Repository"
3. Select your project folder
4. Set local path and name
5. Click "Publish Repository"
6. Choose your GitHub account and repository name
7. Click "Publish Repository"

### Option C: Manual Upload

1. Go to your GitHub repository
2. Click "Upload files"
3. Drag and drop all your project files
4. Add commit message: "Initial commit: Allied Agencies Cochin website"
5. Click "Commit changes"

## Step 3: Enable GitHub Pages

1. **Go to Repository Settings**
   - Click on your repository
   - Click "Settings" tab
   - Scroll down to "Pages" section in left sidebar

2. **Configure Pages**
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch
   - Select "/" (root) folder
   - Click "Save"

3. **Wait for Deployment**
   - GitHub will process your site (1-5 minutes)
   - You'll see a success message with your site URL
   - URL format: `https://yourusername.github.io/your-repo-name`

## Step 4: Verify Deployment

1. **Visit Your Site**
   - Open the URL provided in the GitHub Pages settings
   - Test both `index.html` (main site) and `admin.html` (content management)

2. **Check GitHub Actions**
   - Go to "Actions" tab in your repository
   - Verify that workflows are running successfully
   - Check for any failed workflows and fix issues if needed

## Step 5: Update Configuration Files

### Update robots.txt
Replace `yourusername.github.io/your-repo-name` with your actual GitHub Pages URL in:
- `robots.txt`
- `sitemap.xml`

### Update Contact Information
If needed, update the contact information in:
- `src/data/contact.json`
- `admin.html` (if you prefer to use the admin panel)

## Step 6: Custom Domain (Optional)

### If Using Custom Domain

1. **Create CNAME file** in your repository root:
   ```
   yourdomain.com
   ```

2. **Configure DNS** with your domain provider:
   ```
   A record: 185.199.108.153
   A record: 185.199.109.153
   A record: 185.199.110.153
   A record: 185.199.111.153
   ```

3. **Enable HTTPS** in GitHub Pages settings

## Troubleshooting

### Common Issues

#### 404 Error
- **Cause**: `index.html` not in root directory or incorrect branch
- **Solution**: Ensure `index.html` is in repository root and Pages is configured for main branch

#### Admin Panel Not Working
- **Cause**: Browser console errors or LocalStorage issues
- **Solution**: Check browser console for errors, clear LocalStorage if needed

#### Images Not Loading
- **Cause**: Incorrect image URLs or missing images
- **Solution**: Verify image URLs are correct, replace placeholder images with real ones

#### Slow Loading
- **Cause**: Large images or network issues
- **Solution**: Optimize images, check network connection

#### GitHub Actions Failures
- **Cause**: Workflow configuration issues
- **Solution**: Check Actions tab for error details, ensure repository has proper permissions

### Checking Workflow Status

1. Go to "Actions" tab in your repository
2. Look for workflow runs
3. Check for any failed runs (red X)
4. Click on failed runs to see error details
5. Fix issues and push new changes to trigger workflows again

## Performance Optimization

### Image Optimization
- Compress images before uploading
- Use appropriate image formats (WebP when possible)
- Implement lazy loading (already included in the code)

### Code Optimization
- Minify CSS and JavaScript (optional, not required for this project)
- Use efficient CSS selectors
- Optimize font loading

### Caching
- GitHub Pages provides automatic caching
- Consider adding cache headers if using custom domain

## Security Best Practices

### Repository Security
- Keep repository private if sensitive data is present
- Use branch protection rules for main branch
- Enable required reviews for pull requests

### Content Security
- Regularly update any external dependencies
- Monitor for security vulnerabilities
- Use HTTPS for all external resources

## Maintenance

### Regular Updates
- Update content through `admin.html`
- Monitor GitHub Actions for any failures
- Check site performance regularly
- Update contact information as needed

### Backup Strategy
- GitHub automatically backs up your repository
- Consider exporting data from admin panel periodically
- Keep local copies of important files

## Support

### GitHub Documentation
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Repository Management](https://docs.github.com/en/repositories)

### Project-Specific Help
- Check the `.github/README.md` for workflow documentation
- Review the main `README.md` for project information
- Use the admin panel for content management

## Next Steps

1. **Customize Content**: Use the admin panel to update products, brands, and contact info
2. **Add Real Images**: Replace placeholder images with actual product photos
3. **SEO Optimization**: Update meta tags and content for better search engine visibility
4. **Analytics**: Consider adding Google Analytics or other tracking
5. **Monitoring**: Set up monitoring for site uptime and performance

Your Allied Agencies Cochin website is now ready for production use with automated deployment and quality assurance through GitHub Actions!