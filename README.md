
🏛️ **From Concept to Launch: Building a Full Tourism Website for Visit Swaida — A Front-End Journey**

After weeks of planning, designing, and coding, I'm proud to share the complete development story behind **Visit Swaida** — a tourism platform showcasing the ancient Roman cities, medieval castles, and Druze heritage of southern Syria's Swaida Governorate.


---

**1️⃣ The Brief & My Role**

As the sole Front-End Developer on this project, I was responsible for everything — from initial concept and architecture to the final responsive, animated, production-ready website. The goal was clear: build a platform that could compete visually with international tourism sites while staying true to the cultural identity of the region. No templates. No shortcuts. Built from scratch.

---

**2️⃣ Initial Planning**

Before a single line of code was written, I spent time on:

✅ **Content architecture** — mapping all destinations (Kanawat, Shahba, Salkhad, Swaida City) and identifying what each page needed to communicate
✅ **User flow analysis** — from hero section → destinations → booking → confirmation, every click had a purpose
✅ **Wireframing** — low-fidelity layouts for desktop and mobile to validate structure before styling
✅ **Design tokens** — defined a CSS custom property system (colors, shadows, transitions) upfront so the entire site feels visually unified

The key constraint: the client's audience is mixed — Arabic-speaking locals AND international tourists. Every design decision had to serve both.

---

**3️⃣ Technical Stack & Challenges**

The project runs on **pure HTML5 / CSS3 / JavaScript + jQuery + Bootstrap 4** — deliberately no heavy framework, keeping the site fast and maintainable.

Key technical challenges I solved:

🔧 **Horizontal scroll bug** — `contact-map iframe` had a `margin-left: 100px` applied globally in the original stylesheet, causing overflow on all screen sizes. Fixed by overriding at the CSS layer without touching the original file.

🔧 **CSS override architecture** — rather than editing the base `style.css`, I created a dedicated `enhancements.css` loaded after it. This means all enhancements are isolated, reversible, and clearly traceable.

🔧 **`background-attachment: fixed` parallax** — works beautifully on desktop but breaks on iOS Safari due to the mobile rendering engine. Implemented a `@media` fallback with `scroll` attachment for touch devices.

🔧 **Pannellum 360° viewer integration** — embedded a lazy-loaded virtual panorama that only initializes when the user clicks "Launch Tour," avoiding a 3MB+ asset blocking the initial page load.

---

**4️⃣ Development Phases**

**Phase 1 – Foundation**
Built the semantic HTML structure, navbar with glassmorphism scroll effect, hero with parallax and animated typed destination names, and responsive grid system.

**Phase 2 – Feature Modules**
Developed as self-contained, independently testable units:
- 📅 Interactive Tour Calendar (available / limited / full / past day states)
- 🌦️ Weather Widget (12-month tabs with crowd level, travel tip, and events)
- ❤️ Wishlist / Save Trip system (localStorage persistence, animated FAB + drawer)
- ⏱️ Urgency Banner with real-time countdown timer (sessionStorage dismiss)
- 🗺️ Interactive Map with destination tab switching
- ⭐ Verified Review Badges (Google / TripAdvisor / Booking.com)
- 💬 Live Chat widget with quick-reply buttons and bot responses
- 📜 Horizontal drag-scroll History Timeline (9 eras, colour-coded by period)

**Phase 3 – New Pages**
Built four standalone pages with consistent design language:
`gallery.html` · `packages.html` · `about.html` · and four destination detail pages

**Phase 4 – UX Polish**
Added AOS scroll animations, page loader, back-to-top, sticky mobile Book Now bar, media mentions marquee, and a WhatsApp floating button (critical for Arab-market audiences).

**Phase 5 – Bilingual Support**
Implemented a one-click **Arabic / English toggle** with RTL layout switching (`dir="rtl"`), Arabic nav labels, and section heading translation — no page reload required.

---

**5️⃣ Testing & Optimization**

📱 **Responsive testing** across 5 breakpoints: 1440px / 1024px / 768px / 576px / 360px
🌐 **Cross-browser** — Chrome, Firefox, Safari, Edge, and Samsung Internet (the most common browser in the Arab market)
⚡ **Performance** — lazy-loaded images, deferred non-critical scripts, CSS animations using `transform` and `opacity` only (GPU-accelerated, no layout thrashing)
♿ **Accessibility** — semantic HTML, ARIA labels on interactive elements, keyboard-navigable modals and accordions
🔍 **SEO basics** — descriptive `<title>` tags, `alt` text on all images, logical heading hierarchy (`h1` → `h2` → `h3`)

---

**6️⃣ Final Outcome**

The site launched with:
✔️ 7 fully responsive pages
✔️ 15+ interactive feature modules
✔️ Bilingual (EN / AR) support with RTL
✔️ Masonry photo gallery with destination filters
✔️ 6 curated trip packages with live pricing
✔️ About page with auto-rotating testimonials carousel
✔️ Zero horizontal scroll. Zero layout breaks. Across all tested devices.

🔗 **Live site:** [https://tourist-kohl.vercel.app/](#)
