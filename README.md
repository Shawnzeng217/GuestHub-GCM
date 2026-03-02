<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1VZ9JheXm_g_4iHlNLZ2VLhbASWCWh6Kw

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Deploy to GitHub Pages

This project is configured for automatic deployment to GitHub Pages.

### Setup Instructions:

1. **Enable GitHub Pages:**
   - Go to your repository Settings > Pages
   - Under "Source", select "GitHub Actions"

2. **Add Secret for API Key:**
   - Go to Settings > Secrets and variables > Actions
   - Click "New repository secret"
   - Name: `GEMINI_API_KEY`
   - Value: Your Gemini API key
   - Click "Add secret"

3. **Deploy:**
   - Push your code to the `main` or `master` branch
   - The GitHub Actions workflow will automatically build and deploy your app
   - Your site will be available at: `https://[your-username].github.io/[repository-name]/`

### Manual Build:

To build locally for testing:
```bash
npm run build
```

The built files will be in the `dist` folder.