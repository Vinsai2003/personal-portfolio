# NERELLA VINSAI — Personal Portfolio Website

A professional, responsive personal portfolio website designed to showcase a modern tech stack and versatile projects. Built with **Bootstrap 5**, semantic **HTML5**, and JavaScript.

[**View on GitHub**](https://github.com/NerellaVinsai/personal-portfolio)

![Bootstrap 5](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## Table of Contents
- [Project Overview](#project-overview)
- [HTML Concepts & Project Structure](#html-concepts--project-structure)
- [Setup Instructions](#setup-instructions)
- [Code Structure](#code-structure)
- [Technical Details (Algorithms & Architecture)](#technical-details-algorithms--architecture)
- [Testing & Validation](#testing--validation)
- [Visual Documentation & UI Breakdown](#-visual-documentation--ui-breakdown)

---

## Project Overview

**Goals & Objectives:**
The primary goal of this project was to develop a high-performance, single-page portfolio that serves as a professional gateway for potential clients and employers. 
- **Objective 1**: Implement a fully responsive layout using the Bootstrap 5 grid system.
- **Objective 2**: Ensure cross-browser compatibility and high accessibility standards.
- **Objective 3**: Integrated a serverless contact solution (Formspree) with AJAX for better UX.
- **Objective 4**: Showcase a diverse set of web development projects ranging from logic games to landing pages.

---

## HTML Concepts & Project Structure

**Concepts Learned:**
- **Semantic HTML5**: Utilizing tags like `<header>`, `<main>`, `<section>`, and `<article>` to provide meaning to search engines and screen readers.
- **ARIA Attributes**: Integrating `aria-label` and roles to ensure the site is navigable for all users.
- **Form Manipulation**: Learning how to handle input validation and data submission using modern browser APIs and AJAX.
- **Responsive Frameworks**: Mastering Bootstrap 5 utilities for rapid, consistent layout development.

**Portfolio Structure:**
- **Navigation**: A sticky-top navbar for persistent accessibility.
- **Hero & About**: High-impact introduction followed by an experience overview with key metrics.
- **Toolkit**: Categorized skills covering Design (Canva), Development (MERN Stack), and Workflow Tools (Git).
- **Projects**: A responsive grid system showcasing multiple independent web applications.
- **Contact**: A functional form with real-time feedback and social media integration.

---

## Setup Instructions

**Step-by-Step Installation:**
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Vinsai2003/personal-portfolio.git
   ```
2. **Configure Formspree API**:
   - Create a free account at [Formspree.io](https://formspree.io/).
   - Create a "New Form" and copy your **Unique Form ID**.
   - Open `index.html` and find the contact form section (Line 326).
   - Replace `YOUR_FORMSPREE_ID` in the `action="..."` attribute with your copied ID.
3. **Launch the Application**:
   - Double-click `index.html` to view in your browser, or use the "Live Server" extension in VS Code.

---

## Code Structure

**File Hierarchy:**
```
personal-portfolio/
├── index.html          # Main application (HTML, CSS, JS)
├── README.md           # Documentation
├── images/
|   ├── profile.jpg     # Professional portrait
|   └── favicon.png     # Custom monogram logo
|
├── Visual-Documents/
      ├──about-section-view.png
      ├──android-view.png
      ├──contact-section.png
      ├──desktop-view.png
      ├──footer-section.png
      ├──hero-section.png
      ├──ios-view.png
      ├──project-grid.png
      ├──project-section-view.png
      ├──skill-section.png
      └──tablet-view.png
      

```

---

## Technical Details (Algorithms & Architecture)

**Architecture:**
The site follows a **Single Page Application (SPA)** architecture, utilizing internal styling and scripts for maximum portability and performance.

**Key Implementations:**
1. **Contact Engine**: Uses the `fetch()` API for AJAX submissions. It intercepts the submit event, prevents page reload, and provides immediate async feedback to the user.
2. **Bootstrap Grid**: Uses a mobile-first 12-column grid. Components are stacked on mobile and gracefully expand using responsive breakpoints (`col-lg-4`, `col-md-6`).
3. **Favicon Branding**: Integrated a custom-designed monogram logo as a favicon for browser tab brand recognition.

---

## Testing & Validation

**Validation Evidence:**
- **HTML**: 100% valid as per W3C Markup Validation service.
- **Responsiveness**: Verified via Chrome DevTools across Desktop, Tablet, and Mobile breakpoints.

**Test Cases:**
| Test Case | Interaction | Expected Result | Result |
|-----------|-------------|-----------------|--------|
| Form Validation | Click "Send" with empty fields | HTML5 "Required" tooltips appear | Pass |
| Internal Nav | Click "Work" in navbar | Page smooth-scrolls to #projects | Pass |
| Mobile View | Screen width < 992px | Menu collapses into hamburger icon | Pass |
| Contact API | Submit valid form | Form clears and Success message shown | Pass |

---

## 📸 Visual Documentation & UI Breakdown

This section documents the visual language and responsive design implementation of the portfolio.

### 🌓 Interface Showcase
The UI is built with a focus on **Visual Hierarchy** and **User Experience**, utilizing a custom-themed Bootstrap 5 framework.

<p align="center">
  <a href="Visual-Documents/desktop-view.png">
    <img src="Visual-Documents/desktop-view.png" width="90%" alt="Full Desktop View">
  </a>
  <br>
  <b>Master Layout</b>: A comprehensive view of the sticky navigation, hero impact, and section spacing.
</p>

---

### 📱 Performance & Responsiveness
The site uses a **Mobile-First** approach. The grid system transitions seamlessly from single-column mobile layouts to multi-column desktop views.

| **Mobile (Android)** | **Mobile (iOS)** | **Tablet (768px)** |
| :---: | :---: | :---: |
| <a href="Visual-Documents/android-view.png"><img src="Visual-Documents/android-view.png" width="180"></a> | <a href="Visual-Documents/ios-view.png"><img src="Visual-Documents/ios-view.png" width="180"></a> | <a href="Visual-Documents/tablet-view.png"><img src="Visual-Documents/tablet-view.png" width="280"></a> |
| Optimized for Small Screens | Fluid iOS Rendering | Scaled Tablet Layout |

---

### 🔍 Component Deep Dive
<details>
<summary><b>Expand to view detailed UI components</b></summary>

#### 1. Hero & Branding
The first point of contact, featuring high-contrast typography and a clear Call-to-Action.
[<img src="Visual-Documents/hero-section.png" width="600">](Visual-Documents/hero-section.png)

#### 2. Information Architecture (About & Skills)
Structured data presentation using Bootstrap cards and progress bars.
[<img src="Visual-Documents/about-section-view.png" width="600">](Visual-Documents/about-section-view.png)
[<img src="Visual-Documents/skill-section.png" width="600">](Visual-Documents/skill-section.png)

#### 3. Portfolio Gallery
A dynamic grid that showcases project diversity with hover-effect interactions.
[<img src="Visual-Documents/project-grid.png" width="600">](Visual-Documents/project-grid.png)
[<img src="Visual-Documents/project-section-view.png" width="600">](Visual-Documents/project-section-view.png)

#### 4. Interaction Points (Form & Footer)
Functional Formspree-powered contact section and a clean, minimalist footer.
[<img src="Visual-Documents/contact-section.png" width="600">](Visual-Documents/contact-section.png)
[<img src="Visual-Documents/footer-section.png" width="600">](Visual-Documents/footer-section.png)

</details>



---

Developed by Nerella Vinsai &copy; 2026
