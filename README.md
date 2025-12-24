# periuscomtr
## Perius Technology Executive Advisory Business Website, hosted on GitHub Pages. Built by Cagan Efe Calidag.
### Technologies used
- HTML, CSS, JavaScript
- i18n using /scripts/translations.js
thats all.

### RUNNING LOCALLY TO TEST
1. Install the Live Server extension on VS Code
2. Open index.html
3. - Right click on the code in index.html and select "Open with Live Server"
   - It will open immediately on the browser
   - The preview will get updated as you modify and save the file.

## Manual:

### Perius Technology Website – Update Manual

This guide explains how to update the website content, services, translations, and images **without any HTML or JavaScript knowledge**.

---

### 1. Change Texts (English & Turkish)

All main texts (titles, descriptions, navigation, etc.) are managed in the translation file:

- [scripts/translations.js](./scripts/translations.js)

**How to update:**
- Open `scripts/translations.js`.
- Find the `translations` object.
- Update the English (`en`) or Turkish (`tr`) values for any text you want to change.
- Save the file. The website will automatically use the new text.

---

### 2. Add or Edit Services

Each service has:
- A title
- A description
- Three bullet points
- An image

**How to update service texts:**
- Open [scripts/translations.js](./scripts/translations.js).
- Find the `service1_title`, `service1_desc`, `service1_li1`, etc. for each service.
- Add or edit the text in both `en` and `tr` sections.

**How to add a new service:**
1. **HTML:**  
   - Open [index.html](./index.html).
   - Find the `<div class="services-grid">` section.
   - Copy one `<div class="service-item">...</div>` block and paste it below the last one.
   - Change the image and structure as needed (ask a developer if unsure).

2. **Translations:**  
   - In [scripts/translations.js](./scripts/translations.js), add new keys for your new service (e.g., `service7_title`, `service7_desc`, `service7_li1`, etc.) in both `en` and `tr`.
   - Ask a developer to update the JavaScript to support more than 6 services if needed.

---

### 3. Add or Change Images

- All images are stored in the [`/files/images/`](./files/images/) folder.
- To change a service or logo image, replace the image file or update the `src` attribute in [index.html](./index.html).
- For new images, upload them to `/files/images/` and use the new filename in the HTML.

---

### 4. Add or Update Translations

- All translations are in [scripts/translations.js](./scripts/translations.js).
- To add a new language, copy the structure of `en` or `tr` and add a new language code (e.g., `fr` for French).
- Add all the necessary keys and values for the new language.
- Ask a developer to update the language switcher if you add a new language.

---

### 5. Change Navigation or Add Sections

- Navigation links are in [index.html](./index.html) inside `<ul class="navbar-links">`.
- To add a new section, add a new `<li>` in the navigation and a corresponding `<section>` in the HTML.
- Add translation keys for the new section in [scripts/translations.js](./scripts/translations.js).

---

### 6. Update Social Links

- The LinkedIn link in the footer is in [index.html](./index.html).
- To change it, update the `href` attribute of the `<a class="footer-linkedin">` element.

---

### 7. Styling

- All styles are in [styles/globals.css](./styles/globals.css).
- For layout or color changes, update this file. Most useful colors are in HEX.

---

### 8. Need Help?

If you want to add new features or need help with HTML/JS, contact [Cagan Efe Calidag](mailto:efecalidag@gmail.com)

---
