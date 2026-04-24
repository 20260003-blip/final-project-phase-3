# Project Handoff: Climbros Baguio

## 1. Architectural Logic (Exam Criteria: 12 pts)
* **Design Choice:** I utilized CSS Grid and Flexbox for the primary layout because Grid handles page-level section placement, while Flexbox is better for aligning items inside cards, navigation, headers, and forms.
* **Structural Flow:** The site flows from `header` to `main` to `footer`. The header contains the logo and navigation, the main area holds the page-specific content sections, and the footer closes the page with supporting links and credits. Each page follows the same structure so the experience stays consistent across Home, About, Services, and Contact.

## 2. Design Token System (Exam Criteria: 12 pts)
* **Color Palette:** `--color-primary: #3f6b4f`, `--color-primary-dark: #214d36`, `--color-secondary: #e5e1d8`, `--color-secondary-soft: #f2f0eb`, `--color-neutral-100: #ffffff`, `--color-neutral-200: #f3f3f3`, `--color-neutral-700: #3e4a46`, `--color-neutral-900: #1f2b28`, `--color-primary-yellow: #ffda03`, `--color-accent: #b08d57`, `--color-forest: #214d36`, `--color-moss: #5f7a53`, `--color-fern: #7da37b`.
* **Typography:** `--font-body: "Oswald", sans-serif`, `--font-display: "Oswald", sans-serif`, `--text-sm: 0.95rem`, `--text-md: 1.08rem`, `--text-lg: 1.45rem`, `--text-xl: 2.2rem`, `--text-2xl: 3.4rem`.
* **Spacing:** `--space-xs: 0.25rem`, `--space-sm: 0.5rem`, `--space-md: 1rem`, `--space-lg: 1.5rem`, `--space-xl: 2rem`, `--space-2xl: 3rem`, `--space-3xl: 4rem`.
* **System Proof:** All major styles are linked to these variables in `:root`, so changing one token updates the site consistently.

## 3. Responsive Fluidity (Exam Criteria: 12 pts)
* **Mobile Breakpoint:** < 768px — The layout stacks vertically, navigation stays readable, cards become single-column, and spacing is reduced for smaller screens.
* **Tablet Breakpoint:** 768px - 1024px — The layout shifts into two-column grids where appropriate, and content sections gain more breathing room without overcrowding.
* **Desktop Breakpoint:** > 1024px — The layout expands into fuller multi-column arrangements, with wider containers, larger typography, and stronger visual hierarchy.
* **Fluidity Check:** The site maintains design integrity without horizontal scrollbars because widths are controlled with responsive containers, flexible grids, and media queries.

## 4. Accessibility & Performance (Exam Criteria: 12 pts)
* **Lighthouse Score:** 90+ accessibility score.
* **Compliance:** Accessibility was improved through semantic HTML landmarks, descriptive `alt` text for images, labeled form inputs, clear navigation states, and readable color contrast.
* **[Insert Image of Lighthouse Score Snapshot]**

## 5. BEM Component Index (Exam Criteria: 12 pts)
* **Block `page`:** Full-page layout wrapper.
* **Block `header`:** Top site header containing logo and navigation.
* **Block `nav`:** Primary navigation system.
* **Block `content`:** Main centered content container.
* **Block `css-slider`:** Homepage image slider component.
* **Block `card`:** Reusable destination and feature card component.
* **Block `feature-grid`:** Services grid layout.
* **Block `about`:** About page content wrapper.
* **Block `form`:** Contact form component.
* **Block `home__cta`:** Homepage call-to-action section.
* **Block `country-carousel`:** Country slideshow section on the About page.

* **Elements:** `page__header`, `page__main`, `page__footer`, `header__brand`, `header__logo`, `header__title`, `nav__list`, `nav__item`, `nav__link`, `nav__link--active`, `content__panel`, `css-slider__item`, `css-slider__controls`, `css-slider__prev`, `css-slider__next`, `card__figure`, `card__image`, `card__body`, `card__title`, `card__text`, `feature-card__title`, `feature-card__text`, `about__figure`, `about__image`, `about__caption`, `about__eyebrow`, `about__title`, `about__text`, `form__group`, `form__label`, `form__input`, `form__textarea`, `home__cta-panel`, `home__cta-title`, `home__cta-text`, `home__cta-link`, `country-carousel__title`, `country-carousel__text`, `contact__social`, `contact__links`, `contact__link`.
* **Modifiers:** `nav__link--active`.


## Final Notes
The project uses a consistent visual theme, semantic structure, and reusable components to keep the site maintainable and easy to understand. The shared stylesheet acts as the single source of truth for layout, spacing, color, and typography.