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

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

## Footer Deployment Details

The portfolio website includes a footer showing:
- Website version
- Deploy date
- Author name

### Dynamic Deploy Date
The deploy date is generated automatically on page load using JavaScript.

### Code Snippet
```html
<footer>
  Pravin Mishra Portfolio v1.0 — Deployed on 
  <span id="deployDate"></span> — By Yinusa Kolawole
</footer>

<script>
  const deployDateEl = document.getElementById("deployDate");
  const today = new Date().toLocaleDateString("en-GB", {
    day: "2-digit",
    month: "short",
    year: "numeric"
  });
  deployDateEl.textContent = today;
</script>


```html
<p><strong>Deployed by:</strong> DMI Cohort 2 | Yinusa Kolawole Gbenga | Group 6 | Week 4 | 16-01-2026</p>
```

✅ This proof must be visible in your browser screenshot submission.