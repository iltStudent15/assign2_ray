# Design Rationale

I structured the site into three focused pages (Home, Projects, and Contact) so each page has one clear purpose while still sharing a consistent navigation pattern. Each page uses semantic HTML5 landmarks: header for branding and primary navigation, main for core content, section and article for grouped content blocks, and footer for closing information. This structure keeps the document hierarchy logical for both readers and assistive technologies.

For CSS, I used a single organized stylesheet with reusable component classes and grouped rules by purpose: global tokens and resets first, then layout and component styles, then responsive breakpoints. The layout relies on Flexbox so cards, navigation, and page sections can adapt naturally to available screen space. I also used custom CSS variables for color and spacing consistency, which makes future editing easier.

Accessibility was handled through clear heading order, meaningful image alt text, and explicit form labels tied to inputs with matching for/id attributes. Form fields include focus styles and helper text where useful, so keyboard users receive stronger visual cues and context.

The responsive strategy is mobile-first. Base styles target smaller screens, then expand at 48rem (tablet) and 72rem (desktop) using media queries. This approach keeps the smallest experience lightweight and readable first, while larger layouts gain multi-column cards and side-by-side hero content without rewriting the core structure.
