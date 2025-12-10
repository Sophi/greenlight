# Greenlight Website

Hardware validation & design engineering services website.

## Files
- `index.html` - Main website page
- `styles.css` - Stylesheet with green/orange/white color scheme
- `script.js` - JavaScript for smooth scrolling and animations

## Deploying to GitHub Pages

### Option 1: Quick Deploy
1. Create a new repo on GitHub (e.g., `greenlight-site`)
2. Clone the repo locally
3. Copy these three files into the repo
4. Commit and push:
   ```bash
   git add .
   git commit -m "Initial site launch"
   git push origin main
   ```
5. Go to repo Settings → Pages
6. Under "Source", select "Deploy from a branch"
7. Select "main" branch and "/ (root)" folder
8. Click Save

Your site will be live at: `https://[your-username].github.io/greenlight-site/`

### Option 2: Custom Domain (greenlight.place)
After deploying via Option 1:

1. In your repo, create a file named `CNAME` (no extension) with this content:
   ```
   greenlight.place
   ```

2. In your domain registrar (where you bought greenlight.place):
   - Add these DNS records:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   
   Type: A
   Name: @
   Value: 185.199.109.153
   
   Type: A
   Name: @
   Value: 185.199.110.153
   
   Type: A  
   Name: @
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: [your-username].github.io
   ```

3. Wait 15-60 minutes for DNS to propagate

4. In GitHub repo Settings → Pages, enter `greenlight.place` in the Custom domain field

Your site will be live at: `https://greenlight.place`

## Customization

### Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --green-primary: #00C853;
    --orange-primary: #FF6B35;
    --white: #FFFFFF;
}
```

### Content
- Edit `index.html` to change text, services, or sections
- Update the email in the contact section: `hello@greenlight.place`

### Fonts
Currently using:
- Work Sans (headers and body)
- DM Mono (labels and accents)

To change fonts, update the Google Fonts link in `index.html` and the CSS variables.

## Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile responsive
- Smooth scrolling animations

## License
© 2025 Greenlight
