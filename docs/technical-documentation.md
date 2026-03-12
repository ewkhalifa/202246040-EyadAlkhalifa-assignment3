# Technical Documentation – Assignment 1

## Overview
This project is a static portfolio website using:
- HTML for structure and semantic sections
- CSS for styling and responsive layout
- JavaScript for interactivity (theme toggle, greeting message, form validation)

## Sections Implemented
1. **About Me**
   - Intro paragraph + optional skills/hobbies cards.
2. **Projects**
   - Two project cards with title, description, and placeholder image areas.
3. **Contact**
   - Contact form (Name, Email, Message) with client-side validation (no backend).

## Responsive Design
- Uses CSS Grid for major layouts:
  - Hero uses a 2-column grid on desktop and 1-column on mobile.
  - About section uses a 3-column grid on desktop and stacks on mobile.
  - Projects display in 2 columns on desktop and 1 column on mobile.
- Breakpoint at `max-width: 900px` changes navigation and layout for smaller screens.

## JavaScript Features
### Theme Toggle
- Button toggles `data-theme` attribute on `:root`.
- Saves preference to `localStorage` so it persists after refresh.

### Greeting Message
- Displays a greeting (“Good morning/afternoon/evening”) based on the user's local time.

### Contact Form Validation
- Prevents form submission.
- Validates:
  - Name is not empty
  - Email matches a basic email pattern
  - Message has at least 10 characters
- Displays inline error messages.
- Shows a success message indicating no backend is connected.

## Accessibility Notes
- Uses semantic HTML (header/nav/main/section/footer).
- Form inputs have labels.
- Includes a "Skip to content" link.
- Adds `aria-expanded` for mobile menu toggle.

## Known Limitations
- No backend: messages are not actually sent.
- Project links are placeholders until real URLs are added.