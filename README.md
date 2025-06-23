# 🍔 Berger Hut - Burger Restaurant Website

Welcome to **Berger Hut**, a modern, fully responsive burger shop website built using HTML, CSS, and Font Awesome. This project showcases a fictional burger restaurant with sections for menu, gallery, contact, and more.

![Berger Hut Screenshot](./website%20for%20burger%20shop/gallery1.webp)

---

## 🔗 Live Demo

👉 [View Website on GitHub Pages](https://your-username.github.io/your-repo-name)

> Replace `your-username` and `your-repo-name` with your actual GitHub details.

---

## 📂 Project Structure


---

## 📌 Features

- ✅ Responsive layout
- ✅ Homepage hero section
- ✅ About and Menu sections
- ✅ Reservation form (frontend only)
- ✅ Contact section
- ✅ Image gallery
- ✅ Font Awesome social icons
- ✅ Footer with navigation and links

---

## 🛠 Technologies Used

- HTML5
- CSS3
- Font Awesome CDN
- WebP images (for performance)

---

## ✉️ Contact Form

Currently, the form is frontend-only. To make it functional without a backend, you can integrate [EmailJS](https://www.emailjs.com/) like this:

```html
<script src="https://cdn.jsdelivr.net/npm/emailjs-com@2.6.4/dist/email.min.js"></script>
<script>
  emailjs.init("YOUR_PUBLIC_KEY");

  document.querySelector(".contact-form").addEventListener("submit", function(e) {
    e.preventDefault();
    emailjs.sendForm("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", this)
      .then(() => alert("✅ Message sent!"))
      .catch(() => alert("❌ Error sending message"));
  });
</script>
