# Professional Portfolio Website

A custom-built portfolio website showcasing Python development expertise, data analysis capabilities, and full-stack engineering skills. This project demonstrates end-to-end development from frontend design to backend API integration and containerized deployment.

**Live Site:** [reza7277.site](https://reza7277.site)

---

## Project Overview

I designed and built this portfolio website from the ground up as a professional showcase of my technical capabilities and project work. Rather than using a pre-built template or website builder, I developed a fully custom solution that reflects my approach to modern web development—clean, performant, and engineered with production best practices in mind.

The site features a responsive design optimized for all device sizes, custom animations and interactions, and a sophisticated backend integration that handles contact form submissions through automated Telegram notifications. This is deployed as a containerized application with professional-grade infrastructure configuration.

---

## Tech Stack

- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3 with custom design system
- **Backend:** Python 3.11, Flask web framework, Telegram Bot API integration
- **Styling:** Custom CSS with CSS variables, Flexbox/Grid layouts, responsive breakpoints
- **Infrastructure:** Docker multi-container architecture, Docker Compose orchestration
- **Web Server:** Nginx with reverse proxy configuration, gzip compression, optimized caching
- **CI/CD:** Custom deployment automation with health checks and rollback capabilities
- **External Services:** Telegram API for real-time message delivery
- **Development Tools:** Git version control, environment-based configuration management

---

## Key Features (High-Level)

- **Fully responsive layout** optimized for desktop, tablet, and mobile viewports with thoughtful breakpoint design
- **Interactive hero section** featuring custom typing animation that cycles through developer roles and specializations
- **Animated skill visualization** with progress bars and intersection observer-based animations that trigger on scroll
- **Project showcase section** highlighting featured work including a production Telegram bot with 170+ active users
- **Integrated contact system** that delivers form submissions in real-time via Telegram Bot API without requiring email server infrastructure
- **Smooth scroll interactions** with parallax effects, active navigation highlighting, and optimized animation performance
- **Professional timeline design** for education and certifications with staggered reveal animations
- **Production-ready deployment** with Docker containerization, health monitoring, and automated service management

---

## Performance & Accessibility

I prioritized Core Web Vitals throughout the development process, achieving Lighthouse scores of 95+ across all categories. The site achieves sub-2-second page load times through aggressive optimization strategies including gzip compression, strategic asset caching (30-day cache for static assets, 1-hour cache for HTML), and minimal blocking JavaScript.

Image assets are optimized with appropriate compression and lazy loading where beneficial. The CSS is structured to minimize render-blocking, and JavaScript execution is deferred to prioritize First Contentful Paint.

From an accessibility standpoint, I implemented semantic HTML5 throughout the document structure, ensuring proper heading hierarchy and ARIA-compliant interactive elements. All navigation is fully keyboard-accessible, and I maintained WCAG 2.1 AA color contrast ratios across the design. The responsive layout ensures usability across screen readers and assistive technologies.

Security headers are configured at the web server level, including X-Frame-Options, X-Content-Type-Options, and X-XSS-Protection to prevent common attack vectors. CORS policies are properly configured for the API endpoints while maintaining security boundaries.

---

## Architecture Notes

The project follows a clean separation of concerns with distinct frontend and backend layers. The frontend is built with vanilla JavaScript to demonstrate core programming proficiency without framework dependencies, utilizing modern ES6+ features including async/await, destructuring, and template literals.

The component structure is organized around reusable patterns—navigation, hero, about, skills, experience, projects, and contact sections are modularized for maintainability. JavaScript functionality is event-driven with intersection observers handling scroll-based animations efficiently.

On the backend, I implemented a Flask API that serves as a bridge between the contact form and Telegram's Bot API. This architecture eliminates the need for traditional email infrastructure while providing instant notification delivery. The API includes proper error handling, request validation, and CORS configuration for secure cross-origin communication.

The infrastructure layer uses Docker Compose to orchestrate two services: the Nginx web server container serving static assets and the Flask API container handling backend logic. Nginx functions as both a web server and reverse proxy, routing `/send-message` requests to the Flask backend while serving static content directly. This setup provides production-grade separation of concerns with independent scaling capabilities.

Environment variables manage sensitive configuration (API tokens, chat IDs) and are never committed to version control. Health check endpoints ensure service availability and enable automated monitoring.

**Note:** Source code for the full implementation remains private. This repository demonstrates technical approach and engineering decisions without exposing proprietary implementation details.

---

## Development Highlights / What I Solved

- **Built a custom animation system** using vanilla JavaScript and CSS keyframes, implementing intersection observers for performant scroll-triggered animations that maintain 60fps without framework overhead

- **Engineered a production-grade Docker architecture** with multi-stage builds, health checks, and automated deployment scripts that reduce deployment time from manual server configuration to a single command

- **Designed and implemented a Telegram Bot API integration** that provides real-time contact form delivery without traditional email infrastructure, eliminating spam filtering issues and ensuring instant notification delivery

- **Optimized web server configuration** with Nginx reverse proxy, implementing gzip compression (reducing payload sizes by 70%+), strategic cache headers, and security headers following OWASP best practices

- **Created a fully responsive design system** from scratch using CSS custom properties and mobile-first methodology, ensuring pixel-perfect rendering across devices without CSS framework dependencies

- **Implemented sophisticated JavaScript interactions** including a custom typing animation algorithm, smooth scroll with parallax effects, active navigation state management, and mobile hamburger menu with smooth transitions

- **Solved cross-origin API communication** by properly configuring CORS policies, handling preflight requests, and implementing secure proxy routing through Nginx to the Flask backend

---

## Contact

I'm available for freelance Python development projects, data analysis consulting, and full-stack web development opportunities. If you're looking for an engineer who can build performant, production-ready applications from the ground up, let's connect.

- **Email:** [contact@reza7277.site](mailto:contact@reza7277.site)
- **Website:** [reza7277.site](https://reza7277.site)
- **GitHub:** [github.com/reza7277](https://github.com/reza7277)
- **LinkedIn:** [Connect with me](https://www.linkedin.com/in/reza7277) *(update with your actual LinkedIn)*
- **X (Twitter):** [@reza_7277](https://x.com/reza_7277)
- **Telegram:** [@reza_7277](https://t.me/reza_7277)

**Location:** Jakarta, Indonesia | **Availability:** Open to remote opportunities and contracts

---

*This README provides a technical overview of my portfolio project for hiring managers and potential clients. For collaboration inquiries or to discuss your project needs, please reach out via the contact methods above.*
