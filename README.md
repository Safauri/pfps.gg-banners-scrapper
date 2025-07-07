# 🖼️ pfps.gg Banners Scraper

This Node.js script automates the process of downloading banner images from [pfps.gg](https://pfps.gg)

---

## 🚀 Features

- Scrapes banner images from multiple paginated pages.
- Filters standard image formats: PNG, JPEG, GIF, and WebP.
- Organizes downloads into folders by file type.
- Skips files that have already been downloaded.
- Clean logging for progress and error tracking.

Each folder in the output directory contains banner images sorted by detected file extension.

---

## 🛠️ Usage

1. **Install dependencies:**

   ```bash
   npm install axios cheerio
   ```

2. **Run the script:**

   ```bash
   node scrape.js
   ```

3. **Downloaded images will be saved in the `downloads_by_type/` folder.**

---

## ⚙️ How It Works

- Loops through paginated content on `pfps.gg`.
- Parses HTML to extract `<img>` tags linked to banner URLs.
- Identifies valid image URLs and extracts file extensions.
- Saves each image into a corresponding folder using streams.

---

## Credits

Original code authored by [Yuki](https://github.com/simplyangelic)  
