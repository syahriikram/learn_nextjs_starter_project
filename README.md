<img src="https://img.shields.io/badge/status-development-green?logo=GitHub" alt="In Progress"> 
<br/>
Next Step: Chapter 11

# Project Introduction
A dashboard application containing different features of NextJS. This serves as a great refresher and an opportunity to seek for feature candies that I have missed previously, especially after working on more infrastructure and backend projects in my professional life. This project repository is a follow along from the [NextJS official](https://nextjs.org/learn/dashboard-app/) website.


## Personal notes/learning points
- A really great refresher of the core NextJS features to work with, and extra helpful if you've worked with `React` before. 
- `clsx` library is great for toggling `if else` clauses on classes.
- `next/font` to build fonts instead of runtime load.
- `next/image` to allow automatic optimisation of images by using `<Image>` tag instead of usual `<img>` (place it in `/public`). 
- `className="hidden md:block"` helps to remove image from DOM on mobile screens and md:block to show on desktop screens, and inversely `block md:hidden`.
- `page.tsx` for base navigation routes in a particular folder and `layout.tsx` for sharing UI between multiple pages (helps with partial rendering).
- Use `<Link>` instead of `<a>` for navigation as the latter performs full page refresh.
- `usePathname` with `clsx` combo for active links.
- By default NextJS uses React Server Componments which executes on the server which helps with directly querying a database without an additional API layer.
- `Promise.all(..)` can help with parallel calls instead of default waterfall fetches 
- Always consider which components should be statically vs dynamically rendered.
- Note that with dynamic rendering, your application is only as fast as your slowest data fetch.
- Streaming helps to overcome it to a degree, `loading.tsx` is a special file built on top of `Suspense`.
- Folders with () won't be included in URL path, e.g. /abc/(a)/b.tsx becomes /abc
- Partial Prerendering, an experimental feature that allows you to render a route with static loading shell, while keeping some parts dynamic
- URL search params allows bokmarkable and shareable URLs, Server-Side rendering and initial load with Analytics/Tracking.
- `useSearchParams` allows you to retrieve URL query strings in JSON format
- `usePathname` loads current URL pathname (e.g. /dashboard/invoices)
- `useRouter` enables navigation between routes within client components programmatically.
- `use client` to use event listeners and hooks for client-side.
- Utilise debouncing to limit rate at which function can fire.
- `use server` for server-side works, such as utilising React Server Actions which essentially creates internal APIs for you to directly talk to DBs.
- in `form`, the return values even for type=`number` is string
- use `Zod` a typescript-first validation library to simplify validation works (similar to `pydantic` in python).
- it's generally good practice to store monetary values in cents in database.
- `revalidatePath` is great to clear cache and trigger a new request to server
- Dynamic Route Segments creates routes based on data, if you add square brackets to the folders, e.g. `[id]` 
- `error.tsx` servers as a catch-all for unexpected er rors and allows to display fallback UI to users.
- `error.tsx` needs to be a client component.
- use `notFound` function instead of catch all for a resource that doesn't exist, special page: `not-found.tsx`.
- `notFound` will take precedence over `error.tsx`

- There are quizzes during the walkthrough to test your understanding which was extremely helpful.

## What's next after this repository?
Time to utilise the knowledge to dish out some fancy frontends in my side projects.

### Technology Stack
```NextJS, TypeScript, Tailwind, Vercel, Postgres```

### Core Concepts
`Frontend`, `Database`

# This is cool, can you help me do the same?
Happy to work with you, contact me at `syahriikram@gmail.com`

[![GitHub Syahri](https://img.shields.io/github/followers/syahriikram?label=follow&style=social)](https://github.com/syahriikram)