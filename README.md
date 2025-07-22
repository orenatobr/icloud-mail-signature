# 📩 iCloud Mail Signature for macOS Mail

A modern, responsive HTML email signature for Apple Mail on macOS, featuring clickable icons for **LinkedIn**, **GitHub**, and **WhatsApp**. Ideal for professionals who want a clean, stylish, and functional email footer.

---

## ✨ Preview

```html
Renato F. Pereira  
Data Scientist & AI Engineer | Remote | Computer Vision, LLMs, MLOps & Scalable AI Systems  
Matosinhos, Porto, Portugal  

[LinkedIn Icon]  [GitHub Icon]  [WhatsApp Icon]
```

(See `signature.html` for the actual layout with clickable icons.)

---

## 🚀 Features

- HTML-based signature compatible with Apple Mail
- External icons with links to your professional profiles
- Clean design with semantic markup and inline CSS
- Works with iCloud, Gmail (via Mail.app), and custom domains

---

## 📂 Files

- `signature.html`: The main signature file
- `README.md`: This file with usage instructions
- `.resources/`: (optional) Icons if you want to host them locally instead of using external links

---

## 🛠️ Installation Guide (macOS Mail)

1. **Create a placeholder signature**  
   - Open **Mail.app > Preferences > Signatures**
   - Create a new signature (e.g., `Renato Signature`) and close Mail (`Cmd + Q`)

2. **Navigate to the Signatures folder**  
   Open Finder and press `Cmd + Shift + G`, then paste:

   ```bash
   ~/Library/Mail/V*/MailData/Signatures
   ```

3. **Find the signature file**  
   - Locate the `.mailsignature` file with the most recent timestamp
   - Open it in a text editor (like VSCode or Sublime Text)

4. **Replace its HTML content**  
   - Delete everything below the `Content-Type: text/html` header
   - Paste the contents of `signature.html` directly
   - ⚠️ Do not include images as attachments; use hosted image URLs

5. **Lock the file**  
   - Right-click on the `.mailsignature` file > **Get Info** > check “Locked”
   - This prevents Mail from overwriting it

6. **Reopen Mail.app and test**  
   - Open a new email and select your signature from the dropdown

---

## 🔗 Customize Your Links

Update the following lines in `signature.html` with your actual profiles:

```html
<a href="https://www.linkedin.com/in/your-username">
<a href="https://github.com/your-username">
<a href="https://wa.me/351xxxxxxxxx">
```

---

## 🧩 Optional: Host Your Own Icons

If you prefer not to rely on external icon CDNs (e.g., Icons8), you can:

1. Place PNG icons in a `.resources/` folder
2. Use `cid:` references or `file://` URLs (less portable)
3. Or host the icons on GitHub Pages or your own site and update the `<img src="">`

---

## 📄 License

MIT License. Free to use and adapt.

---

## 🙋‍♂️ Author

**Renato F. Pereira**  
[LinkedIn](https://www.linkedin.com/in/orenatobr) • [GitHub](https://github.com/orenatobr)
