<img src="https://img.shields.io/badge/status-development-green?logo=GitHub" alt="In Progress"> 
<br/>
Next Step: Chapter 9

# Project Introduction
A dashboard application containing different features of NextJS. This serves as a great refresher and an opportunity to seek for feature candies that I have missed previously, especially after working on too many infrastructure and backend projects recently. This project repository is a follow along from the [NextJS official](https://nextjs.org/learn/dashboard-app/) website.


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