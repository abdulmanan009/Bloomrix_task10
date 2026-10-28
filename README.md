# DevTools & Comprehensive Testing Note

I tested the Internship Portfolio website using browser DevTools.

**1. Responsive Layout Testing:**
- **Mobile (375px):** Header uses `<details>` for the menu. Hero and About sections stack vertically. Grid cards stack in 1 column.
- **Tablet (768px):** Desktop navigation appears. Hero and About switch to 2-column layouts. Footer becomes 3 columns.
- **Desktop (1024px+):** Skills grid locks to 3 columns.
- **Container Query (Assignments):** Resized the `.assignment-container` using DevTools to verify the `.assignment-card` shifts layout when the container is under 350px.

**2. Feature Verification:**
- **Active State:** Verified the "About" navigation link is styled with a blue underline using `aria-current="page"`.
- **CSS Functions:** Verified `clamp()` is applied to typography (`--fs-3xl`).
- **Selectors:** Confirmed `:has()` correctly highlights the card containing the "Pending" badge. Confirmed `label:has(+ input:required)::after` correctly adds the red asterisk.
- **Print CSS:** Opened DevTools -> Rendering -> Emulate CSS Media -> Print. Verified the header, footer, and form are hidden, leaving a clean text document.
- **Reduced Motion:** Toggled `prefers-reduced-motion: reduce` in DevTools to verify the fade-in and pulse animations are disabled.
- **Focus States:** Tabbed through the form to verify the blue focus ring is visible on inputs and buttons.