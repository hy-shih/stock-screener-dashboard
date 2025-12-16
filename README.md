# Stock Screener Dashboard

A secure, password-protected web dashboard for viewing stock screening results.

## Features

- 🎭 **404 Disguise**: Home page looks like a 404 error
- 🔐 **Password Protection**: Hidden button and login page
- 📊 **CSV Viewer**: Display Bollinger Bands screening results
- 🔄 **Auto-sync**: Pulls latest CSV files from GitHub
- 📱 **Responsive**: Works on desktop and mobile

## Files Structure

```
stock-screener-dashboard/
├── index.html       # 404 home page with hidden button
├── login.html       # Password login page
├── viewer.html      # CSV data viewer
└── README.md        # This file
```

## How to Use

1. Visit: `https://hy-shih.github.io/stock-screener-dashboard/`
2. Hover over the top-right corner to find the hidden button
3. Click the button to access the login page
4. Enter password: `stockMDFKDBA`
5. Select a CSV file and load the data

## CSV Sources

Data is fetched directly from the stock_screener repository:
- Daily & Weekly breakouts
- Weekly & Monthly breakouts
- Daily, Weekly & Monthly combined breakouts

## Password

Default password: `stockMDFKDBA`

To change it, edit `login.html` and replace the `PASSWORD` variable.

## Customization

### Change Password
Edit `login.html` and modify:
```javascript
const PASSWORD = 'your-new-password';
```

### Add More CSV Files
Edit `viewer.html` and add to the `CSV_URLS` object:
```javascript
'new_file': 'https://raw.githubusercontent.com/hy-shih/stock_screener/main/your_file_{{DATE}}.csv'
```

## Deployment

This is deployed via GitHub Pages. Any changes pushed to the main branch will automatically update the website.

---

Created with ❤️ for stock screening
