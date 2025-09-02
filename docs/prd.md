# 📄 Product Requirements Document (PRD)

**Project:** VEX Robotics Club Website
**Owner:** \[Your Club Name / Team 11702]
**Date:** Aug 2025
**Version:** Draft 1.0

---

## 1. 🎯 Purpose & Goals

The VEX Robotics Club website will serve as the **public face** of the team. It should:

* Showcase the **club identity** (team colors: red, black, white).
* Highlight **who we are** and **ways to support us**.
* Provide a **gallery of photos** from events/competitions.
* Introduce the **team members** with role-based profiles.
* Be **static, fast, and reliable** (Astro.js, TailwindCSS).

---

## 2. 📂 Scope

### In Scope

* Static pages: Home, Gallery, Meet the Team.
* Responsive design (mobile, tablet, desktop).
* Image optimization for gallery.
* Donation call-to-action.
* Theming with red (#FF0000), black (#000000), and white (#FFFFFF).

### Out of Scope

* User accounts / login.
* Dynamic CMS (all content static/manual).
* Competition live updates.

---

## 3. 🏗️ Features & Requirements

### **Navigation Bar**

* Positioned at the top of every page.
* **Left side:** team logo and name ("Team 11702").
* **Right side:** CTA-style tabs linking to each section/page (Home, About Us, Gallery, Meet the Team, Donate).
* Responsive: collapses into a hamburger menu on mobile.

---

### **Home Page**

* **Hero Banner:**

  * A **designed image** created by the team’s design group and imported into the site.
  * No text overlay required; the banner itself will visually represent the team branding.

* **About Us Section:**

  * **Centered block** with short paragraph about the club’s mission, history, and competition highlights. Use **full‑bleed red/black bands** for emphasis.

* **Donate CTA:**

  * Centered, prominent **block CTA** (white text on red with black stroke).
  * Redirects to donation platform (e.g. PayPal, school donation portal).

---

### **Gallery Page**

* Centered 3×3 grid photo gallery.
* Images of equal sizes.
* Hover effect: expand or show caption.

---

### **Meet the Team Page**

* Centered grid of **cards** (3×5).
* Each card includes:

  * Profile photo (optional, fallback to default silhouette).
  * Name.
  * Role (e.g., Captain, Programmer, Builder).
  * Short description (1–2 sentences).

---

## 4. 🎨 Design & Branding

**Visual direction matches your attached mockups (tall banner, knight emblem, bold pride aesthetic).**

* **Overall Style:**

  * **Propaganda‑poster / heraldic** vibe; **minimal but assertive**.
  * **Hero Banner** will be a **pre‑designed static image** provided by the design team.
  * **Hard edges, bold strokes, thick borders**, subtle texture optional.

* **Color Palette (team colors)**

  * **Primary Red:** `#D32F2F` (crimson)
  * **Black:** `#0A0A0A`
  * **White:** `#FFFFFF`
  * **Optional Off‑White for backgrounds:** `#F5F5F5`
  * Use **black keylines** (1–2px) and **white outlines** around emblems on red.

* **Typography**

  * **Headings:** Condensed, uppercase sans (e.g., **Bebas Neue**, **Anton**, **Oswald**). Tight tracking, **ALL CAPS**.
  * **Body:** Neutral sans (e.g., **Inter**, **Montserrat**).

* **Motifs & Components**

  * **Chevrons / Stripes** sparingly as section separators.

* **Layout Patterns**

  * **Hero:** imported static image.
  * **Section blocks:** full‑bleed **red or black** bands with centered white text; alternate to keep contrast.
  * **Gallery:** centered 3×3 grid.
  * **Team cards:** centered, black cards, white text, **red top border** (4px), subtle shadow.

* **Accessibility**

  * Maintain **WCAG AA contrast** (≥ 4.5:1 for body text).
  * Avoid pure #FF0000 on white for small text; prefer #D32F2F or add black outline.

---

## 5. ⚙️ Tech Stack

* **Framework:** Astro.js
* **Styling:** TailwindCSS
* **UI:** ShadCN (if needed for cards)
* **Deployment:** Vercel (recommended)
* **Image Optimization:** Astro Image / Cloudinary (optional)

---

## 6. 🧪 Success Criteria

* Pages load in <2s on desktop and mobile.
* Fully responsive across breakpoints.
* Visual brand consistency (red/black/white).
* Easy for non-technical team members to update content.

---

## 7. 📅 Timeline

| Phase  | Tasks                         | Duration |
| ------ | ----------------------------- | -------- |
| Week 1 | PRD + Wireframes              | 2 days   |
| Week 2 | Implement Home Page           | 3 days   |
| Week 3 | Implement Gallery + Team Page | 3 days   |
| Week 4 | Styling, polish, deployment   | 2 days   |

---

## 8. 📐 ASCII Wireframes

### Home Page

```
 ---------------------------------------------------------
|                   [ HERO IMAGE IMPORTED ]              |
 ---------------------------------------------------------
|                   ABOUT US (full‑bleed band)           |
|                   Short text about team mission        |
|                   + highlights                         |
 ---------------------------------------------------------
|                   DONATE CTA (wide banner/button)      |
 ---------------------------------------------------------
```

### Gallery Page

```
 ---------------------------------------------------------
|                   GALLERY GRID                        |
|                   [ Img ] [ Img ] [ Img ]             |
|                   [ Img ] [ Img ] [ Img ]             |
|                   [ Img ] [ Img ] [ Img ]             |
 ---------------------------------------------------------
```

### Meet the Team Page

```
 ---------------------------------------------------------
|                   TEAM MEMBERS GRID                   |
|                   [Photo] [Photo] [Photo]             |
|                   [Photo] [Photo] [Photo]             |
|                   [Photo] [Photo] [Photo]             |
|                   [Photo] [Photo] [Photo]             |
|                   [Photo] [Photo] [Photo]             |
 ---------------------------------------------------------
```
