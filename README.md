
Prodesk IT Landing Page — Sprint 1 Submission

🚀 Student Intern Project Submission

Intern Name: Alok Kumar Mishra

Role: Full Stack Developer Intern

Sprint Objective: Build and deploy a responsive, pixel-perfect landing page module for the Prodesk IT digital marketing wing.

🎯 Sprint Overview & Achievement Summary

This landing page serves as my validation task for foundational frontend architecture before migrating into Prodesk IT's core React/Node.js repositories.

I have executed all three phases of the sprint timeline, going beyond the Base MVP to implement advanced UI/UX modifications, sandbox-safe local storage, and high-performance layouts.

📸 Dashboard Mockup Preview

Below is a screenshot of the responsive dashboard mockup built entirely with utility classes and custom modern animations:
<img width="1269" height="613" alt="image" src="https://github.com/user-attachments/assets/ee0eccd8-b6fc-4a90-8629-e204cec91616" />


🛠️ Phased Implementations

Phase 1: Base MVP (Mandatory Deliverables)

Semantic DOM structure: Designed with native HTML5 tags (<header>, <main>, <section>, <article>, <footer>) to secure a maximum accessibility baseline.

Grid & Flexbox Mechanics: Utilized responsive grid alignment for layout cards and flex-row configurations for navigation items, avoiding horizontal viewport overflow at any scale.

Three-Column Services: Configured a dynamic layout displaying SEO Dominance, Bespoke Web Development, and Digital Marketing modules.

Phase 2: UI/UX Enhancements (Priority 1 Features)

Sandbox-Safe Theme Engine: Configured a native Light/Dark toggle. If browser iframe security blocks localStorage with a SecurityError, the engine gracefully transitions to an in-memory theme array to prevent a system crash.

Micro-Interactions: Magnetic scale hover states (active:scale-95, hover:-translate-y-2) applied to all Call-To-Action elements and service cards to create visual depth on the Z-axis.

Sticky Dynamic Header: Programmed a scroll event handler that detects scroll positioning to add dynamic box shadows and update color transparency on the fly.

Phase 3: Optimizations & Refactoring (Priority 2 Features)

Utility Styling Refactor: Integrated full Tailwind CSS logic for modular design tokens and transition styles.

Frosted Glassmorphism: Utilized Backdrop Filter styles (backdrop-blur-md) to ensure the fixed navigation layout seamlessly overlays underlying page content.

Floating Accents: Programmed CSS-only floating ambient gradient blobs utilizing infinite delayed keyframe loops for an immersive environment.

⚙️ Technical Blueprint & Logic

Safe Storage Theme Wrapper

To prevent iframe exceptions in sandbox runtime execution, the theme uses this check:

let isStorageAccessAllowed = true;
try {
    const testKey = '__storage_test__';
    window.localStorage.setItem(testKey, testKey);
    window.localStorage.removeItem(testKey);
} catch (e) {
    isStorageAccessAllowed = false;
}

If allowed, it saves themes to localStorage. If not, it preserves user preferences in-memory for that session!

🏃‍♂️ How to Run the Project Locally

Clone this repository or download the source folder.

Navigate to the directory containing index.html.

Double-click index.html to open it in any modern web browser, or run it using a local live server (e.g., Live Server extension in VS Code).

Toggle the Sun/Moon icon in the header to preview the dark theme transition!

💡 Key Learning Outtakes as a Student Intern

Learned how to design clean fallback architectures for browser features inside secured sandbox platforms.

Discovered the impact of semantic structural grids on Lighthouse accessibility audits.

Mastered pure CSS keyframe coordinate changes without relying on heavy third-party animation runtimes.
