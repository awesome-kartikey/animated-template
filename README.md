# Awesome Kartikey Animated Template

A modern, responsive, single-page HTML template featuring smooth scroll animations powered by AOS.js and styled with Tailwind CSS. Based on the Tailwind Starter Kit by Creative Tim, modified by Kartikey.

## Description

This project provides a visually appealing and animated single-page website template. It includes common sections like a hero area, services, about, team, and a contact form. Animations are triggered on scroll, enhancing user engagement. It's built entirely with HTML, CSS (Tailwind), and minimal JavaScript for interactivity and animations.

## Features

- **Responsive Design:** Adapts beautifully to different screen sizes (desktops, tablets, mobiles) using Tailwind CSS.
- **Scroll Animations:** Engaging animations on elements as they enter the viewport, powered by AOS.js.
- **Modern UI:** Clean and professional look using Tailwind CSS utilities and components from Tailwind Starter Kit.
- **Component Sections:** Includes pre-built sections:
  - Navigation Bar (with mobile toggle)
  - Hero Section (with background image and overlay)
  - Services/Features Section (card-based layout)
  - About Section
  - Team Section
  - Contact Section (with form)
  - Footer
- **Easy Customization:** Built with standard HTML and utility-first CSS for straightforward modification.
- **Icon Integration:** Uses Font Awesome for icons.
- **CDN Usage:** Leverages CDNs for libraries (Tailwind CSS, Font Awesome, AOS.js), making setup minimal.

## Tech Stack

- **HTML5:** Base structure of the webpage.
- **Tailwind CSS v1.x:** (via Tailwind Starter Kit CDN) Utility-first CSS framework for styling and layout.
- **AOS.js (Animate On Scroll):** JavaScript library for scroll animations.
- **Font Awesome:** Icon library.
- **JavaScript:** Vanilla JS for mobile navigation toggle and AOS initialization.

## Setup Instructions

This project consists of a single HTML file and relies on CDNs for its dependencies. No complex build setup is required.

1.  **Clone or Download:** Get the project files.

    ```bash
    git clone https://github.com/awesome-kartikey/animated-template.git
    cd animated-template
    ```

    Alternatively, download the ZIP file and extract it.

2.  **Open the File:** Simply open the `index.html` file in your web browser.

    - On macOS: `open index.html`
    - On Windows: Double-click `index.html` or open it via your browser's File > Open menu.
    - On Linux: `xdg-open index.html` (or use your preferred browser command).

    **Note:** An active internet connection is required on the first load to fetch the CDN resources (Tailwind CSS, Font Awesome, AOS.js).

## Usage

1.  **Modify Content:** Open `index.html` in a text editor. Edit the text content within the HTML tags (e.g., headings `<h1>`, paragraphs `<p>`, list items `<li>`) to fit your needs.
2.  **Change Images:** Locate `<img>` tags and update the `src` attribute to point to your desired images. You can use local paths or URLs. Also, update background images specified in `style` attributes.
3.  **Customize Styles:** Modify Tailwind CSS classes directly on the HTML elements to change colors, spacing, layout, etc. Refer to the [Tailwind CSS Documentation](https://tailwindcss.com/docs).
4.  **Adjust Animations:** Change or remove animations by modifying the `data-aos` attributes on elements. Refer to the [AOS.js Documentation](https://github.com/michalsnik/aos).
5.  **Update Links:** Change placeholder `href="#"` values in `<a>` tags to your actual links (social media, internal navigation, etc.).
6.  **Contact Form:** The contact form is currently static HTML. To make it functional, you will need to add backend logic or integrate a third-party service (like Formspree, Netlify Forms, etc.).
