# Frequently Asked Questions (FAQ)

### Q1: How do I change the main title and description in the hero section?

**A:** Open the `index.html` file and locate the `<main>` section with the comment `<!-- Splash Page -->`. Inside this, find the `<h1>` and `<p>` tags within the `div` with class `pr-12`. Edit the text content directly within these tags.

```html
<!-- Text Over Main Background -->
<div class="container relative mx-auto">
  <div class="items-center flex flex-wrap">
    <div class="w-full lg:w-6/12 px-4 ml-auto mr-auto text-center">
      <div class="pr-12">
        <!-- MODIFIED Animation -->
        <h1 class="text-white font-semibold text-5xl" data-aos="zoom-in">
          <!-- EDIT THIS LINE -->
          Your New Title Here.
        </h1>
        <!-- MODIFIED Animation & Delay -->
        <p class="mt-4 text-lg text-gray-300" data-aos="fade-left" data-aos-delay="800">
          <!-- EDIT THIS LINE -->
          Your new description goes here. Change this paragraph content.
        </p>
      </div>
    </div>
  </div>
</div>
```

### Q2: How can I change the background image in the hero section?

**A:** In the `index.html` file, find the `div` immediately inside the `<main>` section that has an inline `style` attribute setting the `background-image`. Replace the URL within `url(...)` with the path or URL to your desired image.

```html
<!-- Background Image -->
<div
  class="absolute top-0 w-full h-full bg-center bg-cover"
  style="background: url(YOUR_IMAGE_URL_OR_PATH_HERE);">
  <!-- Overlay -->
  <span id="blackOverlay" class="w-full h-full absolute opacity-75 bg-black"></span>
</div>
```

### Q3: How do I modify the animations or their timing?

**A:** Animations are controlled by the AOS.js library using `data-aos` attributes on HTML elements.
*   To change the animation type, modify the value of `data-aos` (e.g., `data-aos="fade-up"`). See [AOS documentation](https://github.com/michalsnik/aos) for available animation types.
*   To change the duration, add or modify `data-aos-duration="ms"` (e.g., `data-aos-duration="1500"` for 1.5 seconds).
*   To change the delay, add or modify `data-aos-delay="ms"` (e.g., `data-aos-delay="300"` for 0.3 seconds).
*   To change the easing function, add or modify `data-aos-easing="function-name"` (e.g., `data-aos-easing="ease-in-out"`).

Example:
```html
<!-- Change animation type, add duration -->
<div class="lg:pt-12 pt-6 w-full md:w-4/12 px-4 text-center"
     data-aos="fade-up"
     data-aos-duration="1200"
     data-aos-delay="500"
     data-aos-easing="ease-out-quad">
  <!-- Card content -->
</div>
```
You can also adjust the global AOS settings in the `<script>` tag at the bottom of `index.html`.

### Q4: Is this template responsive? How can I test it?

**A:** Yes, the template uses Tailwind CSS, which is a utility-first framework designed for building responsive layouts. You can test the responsiveness by:
1.  Resizing your browser window.
2.  Using your browser's Developer Tools (usually opened by pressing F12) and selecting the device emulation mode to view the page on different screen sizes (like iPhone, iPad, Android devices).

### Q5: Do I need to install anything to use this template?

**A:** No installation or build process is required. The template uses Content Delivery Networks (CDNs) to load Tailwind CSS, Font Awesome, and AOS.js. You only need a web browser and an internet connection (at least for the first time the page loads to cache the CDN files).

### Q6: How do I make the contact form work?

**A:** The contact form in `index.html` is purely frontend structure. To make it functional (i.e., actually send the message when the button is clicked), you need to:
1.  **Add Backend Logic:** Create a server-side script (e.g., using Node.js, PHP, Python) that receives the form data and sends an email or stores it in a database. You would update the `<form>` tag's `action` attribute to point to your backend endpoint and potentially add JavaScript for submission handling (e.g., using `fetch` or AJAX).
2.  **Use a Third-Party Service:** Integrate a service like [Formspree](https://formspree.io/), [Netlify Forms](https://docs.netlify.com/forms/setup/), [Getform](https://getform.io/), etc. These services typically provide an endpoint URL that you set as the form's `action` attribute, handling the backend processing for you.

### Q7: Can I change the icons used in the template?

**A:** Yes. The template uses Font Awesome icons via `<i>` tags with specific classes (e.g., `<i class="fas fa-robot"></i>`). To change an icon:
1.  Find the icon you want on the [Font Awesome website](https://fontawesome.com/icons).
2.  Copy its class (e.g., `fas fa-star`).
3.  Replace the existing class in the `<i>` tag in `index.html`.

