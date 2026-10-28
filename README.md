# DevTools & Comprehensive Testing Note

I tested the Internship Portfolio website using browser DevTools.

**1. Responsive Layout Testing:**
- **Mobile (375px):** Header uses `<details>` for the menu. Hero and About sections stack vertically. Grid cards stack in 1 column.
- **Tablet (768px):** Desktop navigation appears. Hero and About switch to 2-column layouts. Footer becomes 3 columns.
- **Desktop (1024px+):** Skills grid locks to 3 columns.
- **Container Query (Assignments):** Resized the `.assignment-card` using DevTools to verify the layout responds to its container, not the viewport.

**2. Feature Verification:**
- **CSS Variables:** Checked that all colors, spacing, and fonts use the `:root` tokens.
- **CSS Functions:** Verified `clamp()` is applied to typography (`--fs-3xl`). 
- **Selectors:** Confirmed `:has()` highlights the card containing the "Pending" badge. Confirmed `:not(:placeholder-shown):valid` turns form borders green.
- **Print CSS:** Opened DevTools -> Rendering -> Emulate CSS Media -> Print. Verified the header, footer, and form are hidden, leaving a clean text document.
- **Reduced Motion:** Toggled `prefers-reduced-motion: reduce` in DevTools to verify the fade-in and pulse animations are disabled.