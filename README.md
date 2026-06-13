# Math Planet — ম্যাথ প্ল্যানেট

Personal academic branding & HSC Higher-Mathematics coaching website for
**Hasan Uzzaman Samir** (হাসান উজ্জামান সমীর) — 36th BCS (Education Cadre),
Lecturer (Mathematics), Chittagong Govt. Women's College.

Built mobile-first with **Astro + Alpine.js + Tailwind CSS v4**. All content is in **Bangla**.

## ✨ Features

- Sticky navigation with Alpine-powered mobile menu
- Hero with qualification highlights + statistics cards
- About (timeline), Qualifications cards, "Why choose us" grid
- HSC 1st/2nd year course cards with "ভর্তি চলছে" badges
- Horizontal teaching-methodology timeline
- Animated result counters (Bangla numerals, IntersectionObserver-driven)
- Testimonial carousel + FAQ accordion (Alpine.js)
- Lead-capture admission form with success state
- Contact section, sticky mobile CTA bar, floating WhatsApp button
- Full SEO: meta, Open Graph, Twitter cards, and JSON-LD
  (Person, EducationalOrganization, FAQ, Breadcrumb schemas)

## 🗂 Structure

```text
src/
├── components/   # SEO, Navbar, Hero, About, Qualifications, WhyChoose,
│                 # Courses, Methodology, Results, Testimonials, FAQ,
│                 # AdmissionForm, Contact, Footer, FloatingActions,
│                 # Icon, SectionHeading
├── data/site.ts  # Single source of truth for all Bangla content
├── layouts/      # Layout.astro (fonts, global CSS, scroll-reveal)
├── styles/       # global.css (Tailwind v4 theme tokens + utilities)
└── pages/        # index.astro
```

To edit content (name, courses, testimonials, FAQs, etc.), change `src/data/site.ts`.

## 🧞 Commands

| Command           | Action                                       |
| :---------------- | :------------------------------------------- |
| `npm install`     | Install dependencies                         |
| `npm run dev`     | Start local dev server                       |
| `npm run build`   | Build production site to `./dist/`           |
| `npm run preview` | Preview the production build locally         |

## 📝 Notes

- The admission form is wired for a front-end success state only. Connect it to
  an email/CRM endpoint (or a service like Formspree) to receive submissions.
- Replace the lecturer photo placeholder in `Hero.astro` with a real image.
