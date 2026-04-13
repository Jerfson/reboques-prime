# Design System: Industrial Precision & Artisanal Soul

## 1. Overview & Creative North Star
The Creative North Star for this design system is **"The Kinetic Workshop."** 

This system rejects the "template" aesthetic in favor of a high-end editorial experience that mirrors the craftsmanship of an industrial motorcycle trailer. We are moving away from generic digital patterns to create a layout that feels forged, heavy, and intentional. By leveraging the **0px roundedness scale**, we embrace a "Brutalist Professionalism"—sharp edges, massive typographic weights, and a total absence of decorative fluff. The experience should feel like a premium printed catalog from a high-end custom garage: sober, masculine, and unyielding.

The design breaks the grid through **monolithic symmetry**. Instead of fluid, airy layouts, we use centered, heavy-duty content blocks that command authority.

## 2. Colors & Tonal Depth
Our palette is rooted in the materials of the forge and the workshop: iron, raw timber, and heat.

*   **Primary (#AC3300 / #D4450C):** Represents "Heat & Ignition." Use this exclusively for the most critical actions and highlights.
*   **Secondary (#8E4E08 / #C47A35):** Represents "Cured Wood." This provides the artisanal warmth that balances the industrial coldness.
*   **Surface & Background (#F5F0E8 / #FEF9F1):** A "Bone & Parchment" base that prevents the site from feeling like a standard "dark mode" tech site, giving it a premium gallery feel.

### The "No-Line" Rule
**Standard 1px borders are strictly prohibited.** To separate sections, use **Tonal Shifts**. A section transition is achieved by moving from `surface` to `surface-container-low` (#F8F3EB). The eye should perceive a change in "material" rather than a drawn line.

### Surface Hierarchy & Nesting
Treat the UI as a series of stacked metal plates. 
*   **Base:** `surface` (#FEF9F1)
*   **Elevated Content:** `surface-container` (#F2EDE5)
*   **Floating "Tech" Specs:** `surface-container-highest` (#E7E2DA)

### Signature Textures
To add "soul," apply a subtle noise grain overlay (2-3% opacity) across the entire background. For CTAs, use a vertical gradient from `primary` (#AC3300) to `primary-container` (#D4450C) to simulate the depth of automotive paint.

## 3. Typography: The Editorial Engine
The typography is the "engine" of this design system. It is high-contrast and unapologetically bold.

*   **Display & Headlines ('Bebas Neue'):** These are your "Structural Beams." Use `display-lg` (3.5rem) for hero statements. All headlines must be **Uppercase** with a slight tracking increase (+0.05em) to enhance the industrial, "stamped metal" look.
*   **Body & Labels ('Barlow'):** The "Technical Manual." Barlow provides a clean, geometric readability that feels engineered. 
*   **Hierarchy:** 
    *   `headline-lg`: The primary product features.
    *   `title-md`: Technical specifications.
    *   `body-lg`: Persuasive artisanal storytelling.

## 4. Elevation & Depth
In an industrial aesthetic, "soft" is a weakness. We do not use traditional drop shadows.

*   **The Layering Principle:** Depth is achieved by "stacking" sharp-edged containers. To highlight a specific trailer feature, place a `surface-container-lowest` card on a `surface-dim` background.
*   **The "Ghost Border":** If a technical spec grid requires definition, use the `outline-variant` (#E3BFB4) at **15% opacity**. It should be felt, not seen—like a faint machining mark on steel.
*   **Glassmorphism (Industrial Variant):** For floating WhatsApp CTAs or sticky "Reserve Now" bars, use `surface` color at 80% opacity with a heavy `backdrop-blur` (20px). This creates a "Frosted Industrial Glass" effect that maintains the sober, premium tone.

## 5. Components

### Buttons (The "Machined" Variant)
*   **Primary:** Sharp 0px corners. Background: `primary-container`. Text: `on-primary` (White), Uppercase Bebas Neue. 
*   **Secondary:** Sharp 0px corners. 2px "Ghost Border" using `secondary`. 
*   **Interaction:** On hover, the button should shift from `primary` to `secondary` color, mimicking the tempering of metal under heat.

### Information Cards (The "Spec Sheet")
*   **Structure:** No borders. Background: `surface-container-low`.
*   **Spacing:** Use extreme vertical padding (64px+) to allow the product photography to breathe.
*   **Separation:** Instead of divider lines, use a 40px vertical gap.

### The "WhatsApp" Float
*   **Color:** `#25D366`.
*   **Style:** A square (0px radius) anchor in the bottom right. Use an `ambient-shadow` (4% opacity, 30px blur, tinted with the primary orange) to make it feel like it's hovering over a drafting table.

### Input Fields
*   **Style:** Underline only. Use `outline` token (#8E7067) for the bottom border. When focused, the border transitions to `primary` (#AC3300) and thickens to 2px.

## 6. Do's and Don'ts

### Do:
*   **Use Massive Imagery:** Use high-contrast, desaturated photography of the motorcycle trailer against industrial backdrops.
*   **Embrace Symmetry:** Center-align main headlines and CTAs to create a "sober," grounded feeling.
*   **Respect the 0px Radius:** Every single element must have sharp, 90-degree corners.

### Don't:
*   **No Rounded Corners:** Never use a border-radius. It breaks the masculine, industrial language.
*   **No Generic Icons:** Use heavy-stroke, geometric icons. Avoid "friendly" or "bubbly" icon sets.
*   **No Navigation Menu:** Per the requirements, keep the flow linear and focused on the "Sales Landing" objective.
*   **No Standard Blue Links:** All links must use the `destaque` (#D4450C) color or the `madeira` (#C47A35) color to stay within the artisanal palette.