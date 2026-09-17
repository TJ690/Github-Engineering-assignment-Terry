ou are assisting with a small, public static portfolio website.
Project context:
- Purpose: present a student's skills and projects to internship reviewers.
- Existing system: an HTML/CSS/JavaScript portfolio template.
- Allowed changes: content, styling, and small front - end corrections only.
- Do not add: a backend, login system, analytics tracker, or external data
collection.
Acceptance criteria:
1. [paste your criteria]
2. [paste your criteria]
3. [paste your criteria]
4. [paste your criteria]
5. [paste your criteria]
Constraints:
- Do not invent education, work history, awards, links, or technical skills.
- Preserve required license and attribution.
- Keep the site usable on mobile screens.
- Maintain readable contrast, keyboard navigation, meaningful link text,
and useful image alternative text.
- Do not expose private information.
First provide:
1. A file - by - file implementation plan.
2. Any Assumptions or risks.
3. A proposed test checklist.
4. Any questions that must be answered before implementation.
Do not modify files unti

Response
File-by-File Implementation Planindex.htmlAudit and strip all default template placeholder content (e.g., "John Doe", "Web Developer", default contact info, dummy project cards).Update document metadata (<title>, meta description, Open Graph tags) to reflect student portfolio purpose without exposing private PII.Update image elements: enforce explicit dimensions (width and height attributes) to prevent layout shifts, refine alt attributes to describe image intent clearly, and adjust paths.Upgrade project section items with detailed, structured descriptions (problem statement, technologies used, student's contribution).Convert ambiguous link anchors ("Click Here", "Link") into descriptive, screen-reader-friendly text ("View Source Code on GitHub", "Live Project Demo").Ensure heading elements maintain a strict linear hierarchy (h1 $\rightarrow$ h2 $\rightarrow$ h3).Preserve the original open-source license attribution block in the footer/header comments.assets/css/style.css (or main stylesheet)Implement visual accessibility fixes: audit foreground/background color combinations to ensure WCAG AA compliance (minimum 4.5:1 ratio for standard text).Refine responsive design media queries (@media (max-width: 768px)) to keep navigation, skill badges, and project grids single-column and readable on mobile screens.Apply max-width: 100%; height: auto; object-fit: cover; to all image containers to avoid horizontal overflow or distortion on small viewports.Add visible focus outlines (:focus-visible) for keyboard navigation across all interactive controls.assets/js/script.js (or main JavaScript file)Audit scripts to ensure zero external data collection, analytics trackers, or backend API calls are present.Optimize mobile navigation toggle and section filtering logic for smooth accessibility without layout thrashing.Assumptions & RisksAssumptions:The student will supply real, uninvented details for education, technical skills, and project descriptions prior to final code edits.The site will remain hosted on static infrastructure (e.g., GitHub Pages) with no dynamic server dependencies.Original template assets (icons, layout CSS) are licensed under MIT or similar open-source licenses allowing attribution preservation.Risks:Hidden Placeholder Leak: Unnoticed filler text or default links in hidden UI elements (aria-labels, tooltip attributes, comments).Mobile Breakage: Pre-existing CSS grid/flex rules in the template causing horizontal scrolling on narrow screen widths ($\le$ 375px).Inadvertent Information Disclosure: Accidentally retaining personal phone numbers, physical addresses, or non-public email addresses.Proposed Test ChecklistAcceptance Criteria Verification[ ] Zero placeholder text remains (grep check for "Lorem", "John Doe", "example.com", "TODO").[ ] All project screenshots/images display with proper aspect ratios, crisp scaling, and useful alt text.[ ] All portfolio copy passes spellcheck and grammar review.[ ] Portfolio structure adheres to semantic web standards (<header>, <main>, <section>, <footer>, <nav>).[ ] Each project card includes a clear description covering purpose, tech stack, and key features.Constraints & Accessibility[ ] No invented skills, past roles, education history, or fabricated project metrics are added.[ ] Original template attribution and license comments are retained verbatim.[ ] Page is fully responsive and free of horizontal scrolling on mobile viewports ($\le$ 768px and $\le$ 375px).[ ] Color contrast meets WCAG AA standards across all text elements and interactive states.[ ] Full site functionality is accessible via keyboard navigation alone (Tab, Shift+Tab, Enter, Space).[ ] No backend code, tracking pixels, or third-party analytics scripts exist in the codebase.
