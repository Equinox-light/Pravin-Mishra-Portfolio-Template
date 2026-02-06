# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://<public-ip>`

---

## How to add dynamic date:
Before you deploy, you MUST edit the footer and deploy date dynamic:

Original:

```html
Add a <span id="deployDate"></span> in footer where date goes
```

Add this code snippet:

```html
<script> 
          const d = new Date();
          const formattedDate = d.toISOString().split('T')[0];
          document.getElementById("deployDate").textContent = formattedDate;
        </script>
```

✅ This proof must be visible in your browser screenshot submission.
