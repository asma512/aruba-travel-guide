Aruba Travel Guide: "One Happy Island"
A responsive, multi-page static website acting as a comprehensive travel guide for Aruba. This project demonstrates modern web development practices including semantic HTML5, accessible form design, and a mobile-first responsive layout using CSS Flexbox.

📁 Repository Structure
Plaintext
aruba-travel-guide/
├── css/
│   └── style.css      # Consolidated stylesheet for all pages
├── images
│   └── arikok_national_park.jpg
│   ├── eagle_beach.jpg
│   ├── island.jpeg
├── index.html         # Landing page (Explore)
├── activities.html    # Destination activities page (Things to Do)
├── contact.html       # Inquiry and planning page (Plan Your Trip)
└── README.md          # Project documentation and Design Rationale
📘 Design Rationale
1. HTML Structure & Semantics
The site is built with a multi-page architecture to improve SEO and content organization. I utilized HTML5 semantic landmarks to create a predictable document hierarchy:

<header> and <nav> provide a consistent global navigation experience across all three files.

<main> identifies the unique primary content of each page.

<section> and <article> are used to group thematic content (like the "Endless Adventures" section) and standalone content pieces (like specific activity cards).

Logical Heading Flow: Each page starts with an h1 and follows a strict hierarchy (h2, h3) to ensure screen readers can navigate the outline of the site.

2. CSS Organization & Layout Strategy
I opted for custom CSS over a framework like Bootstrap to demonstrate a deep understanding of the Flexbox layout module.

Modularity: Styles are grouped by component (Header, Cards, Forms). By using shared classes like .info-card across the "Explore" and "Things to Do" pages, I ensured visual consistency while keeping the CSS file maintainable.

Flexbox: Flexbox is used for the navigation alignment and the card-based grid system. It allows the "Activities" cards to wrap naturally as screen sizes change.

3. Accessibility Considerations
Accessibility was integrated from the start, not as an afterthought:

Visual Aids: Every image includes descriptive alt text to provide context for visually impaired users.

Forms: In contact.html, every input is explicitly linked to a <label> via id and for attributes, ensuring the largest possible hit target and clear instruction for assistive technology.

Navigation: I used aria-current="page" to programmatically identify the active page in the navigation bar.

4. Responsive Design Strategy
The site follows a Mobile-First approach.

Mobile (Base Styles): The default view is a single-column layout with stacked navigation elements, optimized for easy scrolling on touch devices.

Desktop (Breakpoint): A media query at 768px triggers the Flexbox layout to shift. The navigation moves to a horizontal bar, and the activity/info cards transition from a vertical stack to a multi-column grid. This strategy ensures the site remains functional and beautiful on everything from a small smartphone to a large desktop monitor.
