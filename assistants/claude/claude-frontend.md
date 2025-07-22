# Claude Code Guidelines for Frontend Development

This file contains guidelines for Claude Code to follow when working on frontend projects, focusing on modern JavaScript/TypeScript development with Tailwind CSS.

## Core Technologies

* **Language:** Prefer TypeScript to JavaScript for better type safety and developer experience
* **Framework:** Follow the established framework patterns (Vue, Angular, Svelte, etc.) - avoid React/JSX
* **Styling:** Use Tailwind CSS as the primary styling solution with utility-first approach
* **Build Tools:** Use modern build tools like Vite, Webpack, or the framework's recommended tooling
* **Package Manager:** Use the project's existing package manager (npm, yarn, pnpm)

## Component Architecture

* **Component Design:** Create reusable, single-responsibility components
* **Props/API Design:** Design clear, minimal component APIs
* **State Management:** Use appropriate state management patterns (local state, context, external stores)
* **Component Structure:** Organize components logically with clear naming conventions

## Styling Approach

* **Tailwind CSS First:** Use Tailwind utility classes as the primary styling method
* **Tailwind CSS Plus:** Leverage Tailwind CSS Plus templates and components when available for faster development
* **Utility Composition:** Compose complex designs using Tailwind utilities rather than custom CSS
* **Component Extraction:** Extract repeated utility patterns into reusable components
* **Custom Utilities:** Create custom utilities in tailwind.config.js when needed
* **Responsive Design:** Use Tailwind's responsive prefixes (sm:, md:, lg:, xl:, 2xl:) for mobile-first design
* **Design Tokens:** Utilize Tailwind's design system (spacing, colors, typography) for consistency
* **Accessibility:** Use Tailwind's accessibility utilities and include proper ARIA labels with semantic HTML

## Performance

* **Bundle Size:** Be mindful of bundle size when adding dependencies
* **Tailwind Optimization:** Ensure Tailwind's purge/content configuration removes unused styles
* **JIT Compilation:** Use Tailwind's Just-in-Time compiler for faster builds and smaller CSS
* **Lazy Loading:** Implement code splitting and lazy loading where appropriate
* **Component Optimization:** Use framework-specific optimization patterns (memoization, computed properties)
* **Asset Optimization:** Optimize images and other assets using modern formats (WebP, AVIF)

## Type Safety (TypeScript)

* **Strict Types:** Use strict TypeScript configuration
* **API Types:** Define proper types for API responses and component props
* **Generic Types:** Use generics appropriately for reusable components
* **Type Guards:** Implement type guards for runtime type safety

## Testing

* **Unit Tests:** Test component logic and behavior
* **Integration Tests:** Test component interactions and user workflows
* **Testing Library:** Use appropriate testing libraries for your framework (Vue Test Utils, Svelte Testing Library, etc.)
* **Visual Testing:** Consider visual regression testing for Tailwind-styled components
* **E2E Tests:** Include end-to-end tests for critical user paths

## Development Experience

* **Hot Reload:** Ensure development server supports fast refresh
* **Linting:** Use ESLint with appropriate rules for the project
* **Formatting:** Use Prettier for consistent code formatting
* **Dev Tools:** Leverage framework-specific dev tools and browser extensions