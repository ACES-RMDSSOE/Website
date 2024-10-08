# Website

**HTML:**

- **`<head>` section:**
  - Contains metadata about the webpage, such as the title, description, keywords, and links to external resources like stylesheet and scripts.
- **`<body>` section:**
  - Contains the visible content of the webpage.
    - **`<div id="welcome-screen">`:** This element defines the welcome screen that appears initially.
    - **`<main>` element:** Contains the main content that becomes visible after the welcome screen is hidden.
      - **`<header>` element:** Displays the ACES logo, title, and a short description.
      - **`<section id="links">`:** Contains buttons with links to various resources.
      - **`<footer>` element:** Displays a message from ACES.

**CSS:**

- Styles the overall layout and appearance of the webpage, such as font colors, background images, and spacing.
- Uses Tailwind CSS utility classes for responsive design and styling.
- May include custom styles for specific elements.

**JavaScript:**

- **`window.onload = function () { ... }`:** Defines a function that runs when the page is fully loaded.
- **`welcomeText.style.opacity = 1;`:** Makes the welcome text visible by setting its opacity to 1.
- **`textArray.forEach((letter, index) => { ... })`:** Iterates through each letter of the welcome text and animates it using GSAP.
- **`setTimeout(() => { ... })`:** Delays the execution of the code within the callback function by a specified amount of time.
- **`gsap.to(element, { ... })`:** Uses GSAP to animate an element with specified properties like `y` (position) and `opacity`.
- **`modal.addEventListener("click", (e) => { ... })`:** Adds a click event listener to the modal element.
- **`navigator.clipboard.writeText(link)`:** Copies the specified link to the user's clipboard.

**Explanation of Key Parts:**

- **Welcome Screen Animation:** The code uses GSAP to animate the welcome text, making it appear letter by letter with a bouncing effect. After a delay, the welcome screen slides up to reveal the main content.
- **Main Content Animation:** The code uses GSAP to animate the elements within the main content section, making them appear smoothly one by one.
- **Modal Functionality:** The code adds a click event listener to the three dots icon on some links. When clicked, it opens a modal window that allows users to share the link or copy it to the clipboard.

**Overall:**

This code combines HTML, CSS, and JavaScript to create a visually appealing and interactive webpage for the ACES student association. It includes a welcome screen animation, a main content section with links to various resources, and a modal for sharing links.
