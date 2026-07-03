# Preference Setup Questions

Ask one question at a time. Keep questions provider-neutral and plain-language. Do not show recommended answers during setup mode.

## Project Defaults

1. For starting a new web app, do you prefer keeping frontend and backend together, splitting them when they need independent deployment, making a mostly static site for content-heavy pages, or choosing based on the app?
2. For projects with multiple apps or shared packages, do you prefer one repository, separate repositories, or deciding case by case?
3. For JavaScript-based projects, do you prefer TypeScript by default, plain JavaScript for small/simple work, or the framework's default?
4. For web apps, do you prefer pages prepared on the server, pages built mostly in the browser, or deciding page by page?
5. For new projects, do you prefer starting from a starter/template when it matches the goal, or creating the structure directly and adding only what is needed?
6. For development setup, do you prefer projects that run directly on your computer, container/dev-environment setups, or hosted cloud workspaces?
7. For project file organization, do you prefer feature-based folders, type/layer-based folders, or the framework's default?

## Frontend Frameworks

1. For React apps, do you prefer a full framework like Next.js when routing/backend/SEO matter, a lighter Vite-style setup for browser-only apps, or deciding case by case?
2. For forms, do you prefer native browser forms, a form library, or framework-provided form handling when available?
3. For normal app state like open menus, selected items, and draft form values, do you prefer keeping state close to each component, or using a shared state library when many parts of the app need the same state?
4. For state that affects what the user is viewing, like filters, search terms, tabs, and pagination, do you prefer putting it in the URL or keeping it internal when the state is temporary?
5. For backend/API data that needs caching, refetching, loading states, and retry behavior, do you prefer a dedicated data-fetching library, or keeping data loading simple until those needs appear?
6. For motion, do you prefer using it freely for personality, only when it clarifies feedback/transitions, or rarely unless it clearly improves the experience?
7. For useful motion, do you prefer simple CSS, a dedicated animation library like Motion/GSAP, or whatever the existing project already uses?

## Frontend Design

1. For app navigation, do you prefer sidebars, top bars, command/search navigation, or choosing based on the workflow?
2. For dashboards and admin tools, do you prefer dense layouts with compact tables, filters, and metrics visible at once, or roomier layouts with fewer items on screen and more breathing room?
3. For repeated operational workflows like review queues, CRMs, and internal tools, do you prefer compact controls and faster scanning, or larger controls and more guided spacing?
4. For marketing, portfolio, and editorial pages, do you prefer immersive visual storytelling, restrained product-focused layouts, or copy-led pages with minimal decoration?
5. For creative tools and canvas-like products, do you prefer panels and toolbars around the workspace, docked side/bottom panels, a minimal interface that stays out of the way, or mode-specific controls that appear only when needed?
6. For new interfaces, do you prefer light mode by default, dark mode by default, system setting, or a custom theme for the product?
7. For color palettes, do you prefer restrained palettes, bold/high-contrast palettes, brand-heavy palettes, or palettes derived from the product/content?
8. For shapes and corners, do you prefer sharper geometry, softly rounded UI, strongly rounded/pill-like UI, or following the product's existing style?
9. For overall visual style, do you prefer minimal/utilitarian for tools, polished/glassy for premium surfaces, brutalist/edgy for bold brands, native-platform for familiarity, or highly custom/brand-specific?
10. For controls, do you prefer icon-only controls, icons with labels, or text-first buttons and links?
11. For icon-only buttons, do you prefer tooltips on every icon button, tooltips only for unclear or destructive actions, or avoiding icon-only buttons unless the action is obvious?
12. For clickable controls, do you prefer a pointer cursor on all clickable controls, only on button/link-like controls, or following the platform/browser default?
13. For headlines and sections, do you prefer never using eyebrow/kicker text or small decorative elements above them, using them only when they add real structure, or allowing them freely as part of the visual style?
14. For responsive design, do you prefer starting from mobile layouts, desktop layouts, or the most important user workflow regardless of screen size?
15. For adapting layouts across screen sizes, do you prefer preserving the same structure when possible, or redesigning the layout substantially for mobile and desktop when the workflow benefits?

## UI Component Systems

1. For new interfaces, do you prefer starting from an existing component system like shadcn/ui, Radix, Chakra UI, or MUI, custom components, or a mix where primitives are reused but final components are tailored?
2. For using a component system, do you prefer copying editable components into the project for control and customization, installing package components for easier updates, or choosing based on how much customization the design needs?
3. For styling new interfaces, do you prefer Tailwind by default, plain CSS/CSS Modules, a component library's styling system, or choosing based on the existing stack?
4. For layout implementation, do you prefer CSS Grid for page-level two-dimensional layouts, Flexbox for one-direction rows/columns, a mixed approach, or following the existing project style?
5. For component reuse, do you prefer starting with feature-specific components and extracting shared components only after reuse appears, or creating shared components earlier when a pattern seems likely?
6. For components that become shared, do you prefer keeping them flexible with variants/props, or keeping them narrow and creating separate components for meaningfully different uses?
7. For table implementation, do you prefer native HTML tables for simple display, TanStack Table for flexible custom tables, a full data grid like AG Grid/MUI DataGrid for spreadsheet-like features, or choosing based on complexity?
8. For table filtering, do you prefer filters visible above the table, tucked into a filter panel/drawer, built into column headers, or shown only when the user asks for filters?
9. For table sorting, do you prefer sortable columns by default when sorting makes sense, sortable only for key columns, or unsortable columns unless explicitly needed?
10. For table density, do you prefer compact rows that show more records, comfortable rows with more spacing, or a user-controlled density toggle?
11. For large tables, do you prefer pagination, infinite scrolling, virtualized scrolling, or choosing based on how users compare records?
12. For table row actions, do you prefer actions visible inline, hidden in a row menu, shown in a toolbar after selecting rows, or chosen based on action frequency?
13. For table exports, do you prefer CSV/Excel export by default for admin/reporting tables, export only for data-heavy business workflows, or export only when specifically requested?
14. For editing an item from a list or table, do you prefer opening a side drawer, opening a modal, navigating to a dedicated edit page, or inline editing when possible?
15. For reversible actions like archiving, removing from a list, or changing status, do you prefer an undo-after-action pattern, a confirmation step, or immediate action with no extra prompt?
16. For destructive actions like deleting records or cancelling something important, do you prefer a confirmation modal, an inline confirmation step, or typed confirmation for extra friction?
17. For confirmations, do you prefer concise plain-language warnings, detailed warnings that explain consequences, or stronger friction only for irreversible actions?
18. For small secondary choices like filters, sort options, and quick settings, do you prefer popovers/menus, always-visible controls, or side panels?
19. For user changes, do you prefer the UI updating immediately while saving in the background, waiting for server confirmation before showing the change, or choosing based on how costly a wrong temporary state would be?

## Databases

1. For small local tools, prototypes, and single-user apps, what database do you prefer by default: SQLite, local files/JSON, DuckDB, or something else?
2. For production web apps with normal relational data like users, accounts, orders, and settings, what database do you prefer by default: Postgres, MySQL, SQLite-compatible hosted databases, or something else?
3. For analytics-heavy or local data exploration projects, what database do you prefer by default: DuckDB, Postgres, BigQuery/Snowflake-style warehouses, or something else?
4. For apps with flexible document-like records, do you prefer a document/NoSQL database, Postgres with JSON fields, or staying relational unless there is a strong reason not to?
5. For prototypes, do you prefer using the same kind of database the real product would use, or using the simplest temporary storage that proves the idea fastest?
6. For working with relational databases, do you prefer writing SQL directly for control, using a query builder like Kysely/Drizzle for safer SQL-shaped code, or using an ORM like Prisma/SQLAlchemy for higher-level models?
7. For projects where the framework has a common database tool, do you prefer following that ecosystem default for smoother integration, or choosing the database layer independently?
8. For database libraries, which tools do you prefer by default: Prisma, Drizzle, Kysely, SQLAlchemy, raw SQL helpers, or choosing based on language/framework?
9. For database changes over time, do you prefer migration files generated by tooling, hand-written migrations, platform-managed migrations, or following the framework/database default?
10. For deleted records, do you prefer permanent deletion by default, keeping recoverable hidden records by default, or deciding based on whether the data needs audit/history/recovery?
11. For record IDs, do you prefer UUIDs, ULIDs/CUIDs, auto-incrementing numbers, database-native IDs, or following the stack default?
12. For apps with multiple customers or organizations, do you prefer shared tables with a customer ID, separate schemas/databases, or deciding only once multi-tenancy is actually needed?

## Backend and API

1. For API style, do you prefer REST-style endpoints for broad compatibility, typed app-specific calls for one frontend talking to its own backend, or GraphQL when screens need flexible custom data queries?
2. For typical web app backends, what language/runtime do you prefer by default: Node/TypeScript, Python, Go, Ruby, .NET, Java/Kotlin, or decide by project?
3. For data, automation, scraping, AI, or internal tooling backends, what language/runtime do you prefer by default: Python, Node/TypeScript, Go, or something else?
4. For high-performance services, background workers, or infrastructure tools, what language/runtime do you prefer by default: Go, Rust, Node/TypeScript, Python, or something else?
5. For projects where the frontend is TypeScript, do you prefer using TypeScript on the backend too for one shared language, or choosing the backend language independently?
6. For a new backend, do you prefer starting as one application unless there is a clear reason to split it, or starting with separate services when the project has distinct responsibilities?
7. For a backend that starts as one app, do you prefer creating separate areas for each feature early, or keeping most backend code together until the app has enough complexity to justify splitting it up? For example, separate areas can help a SaaS app with billing, accounts, and admin tools; a small internal form app may not need that structure yet.
8. For validating inputs, do you prefer a schema validation library, framework-native validation, simple manual checks for small cases, or following the stack default?
9. For API documentation and external handoff, do you prefer formal OpenAPI/spec files, generated docs from code, human-written integration guides, examples-first documentation, lightweight notes while the API stabilizes, or no separate docs for private app-only APIs?
10. For background work like email/uploads, do you prefer queues, scheduled jobs, managed workflow tools, serverless tasks, or keeping small jobs inline until they become slow or unreliable?
11. For realtime updates, do you prefer WebSockets, Server-Sent Events, polling, a managed realtime service, or avoiding realtime until the product clearly needs it?
12. For normal app settings like public URLs, app limits, or environment-specific options, do you prefer simple environment variables, a typed config file checked by the app, or the hosting platform's built-in settings? For example, environment variables are common for small apps; typed config helps when a team needs safer, clearer settings.
13. For private secrets like API keys and database passwords, do you prefer local `.env` files for development, hosting-platform secret managers, shared team vaults, dedicated secrets tools for larger projects, or platform-specific secret bindings?
14. For missing or invalid required settings, do you prefer the app failing immediately at startup, warning during development, or being lenient only for quick prototypes?
15. For backend errors, do you prefer letting the framework handle most errors, returning explicit success/error results from important functions, or routing errors through one central handler? For example, framework handling is fastest for small apps, explicit results make payment or billing flows easier to reason about, and a central handler keeps API error responses consistent.

## Auth, Users, and Permissions

1. For login and user accounts, do you prefer a hosted auth service for speed, an auth library built into the app for more control, the hosting platform's built-in auth when available, or custom auth only when the product has unusual requirements?
2. For login methods, do you prefer magic links or one-time codes, email and password, Google/GitHub/social login, passkeys, business SSO, or choosing based on the audience?
3. For permissions, do you prefer simple roles, specific per-action permissions, policy rules for complex authorization, or owner/admin checks until more is needed?
4. For public apps or SaaS products, do you prefer open signup, invite-only signup, approved email domains, or a waitlist before users can join?
5. For internal tools, do you prefer admin-created accounts, approved company email domains, single sign-on, or no user accounts when the tool is private enough?
6. For team or organization products, do you prefer users joining by invite, requesting access, joining automatically by approved email domain, or letting admins create accounts manually?
7. For users who do not have access to something, do you prefer hiding the page/action entirely, showing it disabled with an explanation, or letting them request access?
8. For backend permission checks, do you prefer checking permissions inside each important action, using shared permission helpers/policies, or relying on the framework/auth tool's recommended pattern?
9. For hosted auth providers, do you prefer storing basic profile fields like name and avatar in the provider, copying them into the app database, or keeping provider data and app-specific profile data separate?
10. For projects without a hosted auth provider, do you prefer keeping profile data in the main users table, splitting it into a separate profile table, or following the framework/auth library default?
## Email, Notifications, and Messaging

1. For sending email, which provider style do you prefer: AWS SES, Resend/Postmark, Loops/Customer.io, SendGrid/Mailgun, or choosing by app?
2. For transactional and marketing email, do you prefer separate tools, one shared tool when possible, or choosing based on email volume and who edits the messages?
3. For email templates, do you prefer keeping them in the codebase, editing them in the email provider dashboard, managing them in a CMS/database, or starting with simple plain text/Markdown? For example, code works well for transactional emails with app data, while provider dashboards or CMS editing work better when non-developers update messages.
4. For outbound email sending, do you prefer queueing emails by default, sending directly for simple low-volume flows, or queueing only important emails that need retries?
5. For email domain authentication setup, do you prefer doing it during initial setup for production email, waiting until launch/sending volume grows, or using provider defaults for prototypes?
6. For product notifications, which channels do you prefer by default: in-app messages, email, mobile/browser push, Slack/Discord-style team alerts, or as few notifications as possible? For example, in-app works for routine activity, email works for account updates, and push works only when timing matters.
7. For non-critical emails, do you prefer including unsubscribe/preference links in every message, only in recurring or marketing-style messages, or following the email provider's compliance defaults?
8. For system status or error alerts, do you prefer sending them to the app owner, a shared team inbox, Slack/Discord-style team alerts, an incident tool, or logs only?
9. For products where email is important, what level of email observability do you prefer: basic send logs, delivery and bounce tracking, full user-facing email history, or provider dashboards only?

## Blog, CMS, and Content

1. For blogs and marketing content, do you prefer developer-owned content in Markdown/code, a visual CMS/editor for non-developer editing, a built-in database editor, or the framework's content system? For example, Markdown fits personal or developer-owned sites, while a CMS fits teams that edit content without code.
2. For content-heavy sites, do you prefer static pages rebuilt on publish, dynamic pages loaded from a CMS/database, or choosing based on how often content changes?
3. For blog or docs pages, do you prefer MDX when content needs custom components, plain Markdown for writing simplicity, or the framework default?
4. For content images, do you prefer keeping them in the repo, using the hosting platform's media storage, using object storage, or letting the CMS manage them?
5. For content search, do you prefer adding search from the start for sites expected to grow, adding it only after there is enough content, or using the CMS/framework search if available?
6. For organizing content, do you prefer tags, categories, collections/series, or keeping the structure flat until the content needs more organization?
7. For blog post metadata, which pieces do you prefer by default: author profiles, publish dates, updated dates, reading time, related posts, or only the minimum needed for the site?
8. For SEO metadata and social sharing images, do you prefer generating them automatically, writing them manually for important pages, or handling them through the CMS?
9. For content previews and drafts, do you prefer supporting them from the start for editorial review, adding them only for CMS/non-developer workflows, or skipping them for developer-owned content?

## Payments and Billing

1. For payments and subscriptions, which provider style do you prefer: Stripe, a merchant-of-record provider like Paddle or FastSpring, PayPal/Braintree, Adyen, platform-native payments, or choosing by business model?
2. For checkout, do you prefer a payment-provider hosted checkout, an embedded checkout inside the app, or a custom checkout only when the product requires it?
3. For pricing models, do you prefer subscriptions, one-time payments, usage-based billing, free trials, freemium plans, or choosing based on the product?
4. For billing customer records, do you prefer keeping most billing data in the payment provider, mirroring key billing fields in the app database, or storing enough in both places for app logic and support?
5. For payment events like successful payments, failed payments, and subscription changes, do you prefer handling provider webhooks from the start, adding them only when the app needs automated reactions, or using provider-dashboard follow-up only for very early low-volume products?
6. For paid-plan access, do you prefer basing access on user/account type, feature flags, plan checks stored in the database, billing-provider entitlements, or simple checks until the app grows?
7. For invoices, receipts, tax handling, and billing portals, do you prefer delegating them to the payment provider, building the customer-facing parts in-app, or using provider defaults first and customizing later?
8. For free trials, do you prefer requiring a payment method, allowing trials without a payment method, offering freemium instead of trials, or choosing by product?
9. For cancellation, plan changes, and failed-payment recovery, do you prefer handling them fully in-app, sending users to the payment provider portal, or using a hybrid where common changes happen in-app and complex billing actions use the provider portal?
10. For billing analytics, what level do you prefer by default: provider dashboard only, basic revenue metrics in the app, detailed SaaS metrics like MRR/churn/conversion, or custom analytics only once revenue becomes central?

## SaaS Product Defaults

1. For SaaS account structure, do you prefer organizations/teams from the start for B2B or collaboration products, or individual accounts first for simpler products?
2. For admin and support tools, do you prefer a basic admin area from the start, using existing provider dashboards or simple internal tools at first, or building admin screens only when operational needs appear?
3. For feature flags, do you prefer building them in from the start, using simple config-based flags at first, or adding a flag system only when rollout/testing complexity appears?
4. For onboarding, do you prefer a guided setup flow, an empty-state checklist, sample/demo data, minimal onboarding, or choosing by product complexity?
5. For usage limits and quotas, do you prefer adding them from the start for billing/abuse control, adding soft limits first, or waiting until real usage shows the need?
6. For product audit logs, what level do you prefer: none until needed, logs for admin/sensitive actions only, logs for most user actions, or full audit history for compliance-heavy products?
7. For settings pages, do you prefer fewer grouped pages with multiple related settings together, more focused pages where each settings area is separate, or choosing based on how many settings the product has?
8. For user feedback and support, do you prefer in-app forms, email links, chat widgets, issue trackers for technical users, or choosing by audience?
9. For customer support at launch, do you prefer a shared email inbox, help desk tool, in-app support, knowledge base first, or lightweight support until volume grows?
10. For import/export tools, do you prefer including basic export from the start, adding import/export when users ask for it, or building robust data portability for business products by default?

## Files, Media, and Storage

1. For user-uploaded files, do you prefer object storage like S3/R2/GCS, platform-managed file storage, database-backed storage only for small files, or choosing by project?
2. For file uploads, do you prefer direct-to-storage uploads with signed URLs, uploads through the app backend, or using a hosted upload service?
3. For image handling, do you prefer optimizing and resizing images automatically, storing originals and generating variants on demand, or keeping image processing minimal until needed?
4. For user-generated media that other users can see, do you prefer review before publishing, publish first with report-and-remove tools, or no moderation unless the product needs it?
5. For uploaded files that may contain unsafe content, do you prefer automated scanning from the start, scanning only for public/shared files, or adding scanning when the product risk requires it?
6. For organizing stored files, do you prefer readable folder paths by customer/user/project, storing files in flatter buckets and tracking organization in the database, or following the storage provider's common pattern?
7. For large imports and exports, do you prefer background processing with progress tracking, synchronous processing for small files, or hosted data-import tools?
8. For file retention, do you prefer deleting unused files aggressively, keeping files as long as related records exist, or setting explicit retention windows by file type?

## Integrations and Automation

1. For third-party integrations, do you prefer building direct integrations in-app, using automation platforms like Zapier/Make, or adding integrations only for high-value workflows?
2. For connecting to outside services, do you prefer users pasting their own API keys, OAuth sign-in/connection flows, one shared admin-managed connection, or choosing by integration type?
3. For integration sync, do you prefer scheduled sync jobs, event/webhook-driven sync, manual sync buttons, or choosing by data freshness needs?
4. For public APIs, do you prefer exposing them early for extensibility, waiting until the product stabilizes, or keeping the app private unless customers need API access?
5. For automation inside the product, do you prefer built-in workflow rules, simple notification/action triggers, external automation tools, or no automation until patterns repeat?

## Security, Privacy, and Compliance

1. For sensitive user data, do you prefer collecting the minimum possible, collecting what improves the product with clear retention, or deciding by business requirements?
2. For personally identifiable information, do you prefer keeping it in the main app database, isolating it in separate tables/services, or avoiding storage when a provider can hold it?
3. For encryption needs, do you prefer relying on managed platform/database encryption, adding app-level encryption for sensitive fields, or using dedicated data protection tools for regulated products? For example, normal account data may fit platform encryption, while medical or financial fields may need stronger protection.
4. For data retention, do you prefer short retention windows by default, keeping data while accounts are active, or configurable retention by customer/project?
5. For account deletion, do you prefer self-serve user controls, admin-assisted deletion, or adding deletion workflows when privacy/compliance needs require them?
6. For user data export, do you prefer self-serve export controls, admin-assisted exports, scheduled exports for business accounts, or adding export only when users/compliance require it?
7. For legal and policy pages, do you prefer adding boilerplate Terms/Privacy pages from the start, adding them as a final launch checklist item, or only adding them when the product collects sensitive data, payments, or public users?

## Analytics and Telemetry

1. For product analytics tools, do you prefer privacy-friendly analytics, full-featured product analytics like PostHog/Amplitude, simple web analytics like Plausible/GA, or choosing by product maturity?
2. For analytics event detail, do you prefer minimal tracking for core flows only, moderate tracking for important user actions, or deep tracking for most interactions including small ones?
3. For user identification in analytics, do you prefer anonymous analytics by default, account-level identification, user-level identification, or choosing by privacy needs?
4. For dashboards and reporting, do you prefer provider dashboards, custom in-app dashboards, BI tools, or simple exports until reporting needs grow?
5. For keeping analytics data long term, do you prefer relying on the analytics provider, periodically exporting important data, or storing key analytics in your own database/warehouse when reporting becomes important?

## Internationalization and Localization

1. For language support, do you prefer English-only until there is demand, i18n-ready structure from the start, or full localization early for global products?
2. For translation management, do you prefer translation files in the repo, a hosted translation platform, CMS-managed translations, or manual translation only when needed?
3. For dates, times, and time zones, do you prefer always showing user-local values, showing product/business time zones, or choosing per workflow?
4. For currency and number formatting, do you prefer locale-aware formatting from the start, simple fixed formatting until international users appear, or choosing by billing/geography needs?
5. For mobile reach, do you prefer responsive web first, PWA capabilities, cross-platform native apps like Expo/React Native, or native iOS/Android only when required?
6. For offline or unreliable-network use, do you prefer offline-first behavior, limited offline drafts/cache, or online-only unless the product clearly needs offline support?

## Documentation and Handoff

1. For project documentation, do you prefer a concise README, fuller setup/architecture docs, docs generated from tooling, or minimal docs until the project grows?
2. For architecture decisions, do you prefer lightweight decision notes, formal ADRs, inline code comments near decisions, or documenting only major irreversible choices?
3. For frontend component documentation, do you prefer Storybook-style catalogs, simple examples in docs, inline usage examples near components, or documenting components only once reused widely?

## Deployment, Infrastructure, and Hosting

1. For hosting new apps, which platforms do you generally prefer: Vercel/Netlify, Cloudflare, Fly/Render/Railway, AWS/GCP/Azure, Hetzner/VPS, or choosing per project?
2. For where apps run, do you prefer edge/serverless deployments, a normal regional app server, a traditional VPS, or choosing based on latency and operational needs?
3. For infrastructure ownership, do you prefer managed services, self-hosted services, or managed defaults with self-hosting only when cost/control matters?
4. For Docker, do you prefer using it by default, using it only when deployment needs it, or avoiding it unless it clearly helps?
5. For infrastructure setup, do you prefer defining servers/services in code files, configuring things in provider dashboards, using CLI scripts, or doing manual setup for small projects?
6. For release environments, do you prefer local/staging/production, local/preview/production, local/preview/staging/production, or the simplest path to production until the project grows?
7. For production visibility, what level do you prefer at launch: basic logs only, logs plus error tracking, logs/metrics/error tracking from day one, or adding observability after the first deployment?
8. For backups and recovery, do you prefer provider-managed backups only, explicit database backups with restore testing, point-in-time recovery for production apps, or adding stronger recovery once the product has real users?
9. For hosting tradeoffs, do you prefer optimizing for lowest cost, lowest maintenance, strongest platform fit, easiest deployment, or choosing per project?

## Testing, Quality, and Workflow

1. For prototypes and new apps, when do you prefer writing tests: before code, after the first version works, only smoke tests at first, or after the project stabilizes?
2. For JavaScript/frontend testing tools, do you prefer Vitest/Jest, Testing Library, browser-flow tools like Cypress, framework defaults, or choosing by project?
3. For the first tests added to a project, what kind do you prefer: unit tests for small logic, integration tests for connected behavior, end-to-end tests for critical flows, contract tests for APIs, or visual tests for UI regressions?
4. For linting and formatting, do you prefer enforcing them immediately with tools like ESLint/Prettier or Biome, relying on framework defaults for small projects, or adding stricter tooling after the app structure stabilizes?
5. For CI checks, do you prefer running them on every push, only on pull requests, before release, or only once the project needs them?
6. For commit messages, do you prefer a formal convention, plain descriptive messages, or convention only for projects that generate changelogs/releases?
7. For branching workflow, do you prefer feature branches, working directly on main for solo projects, or choosing by team size?
