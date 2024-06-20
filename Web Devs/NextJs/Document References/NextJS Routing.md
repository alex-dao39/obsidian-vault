## File Convention
| File Name                                                                                               | Used for                                                                                                         |
| ------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| [`layout`](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts#layouts)     | Shared UI for a segment and its children                                                                         |
| [`page`](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts#pages)         | Unique UI of a route and make routes publicly accessible                                                         |
| [`loading`](https://nextjs.org/docs/app/building-your-application/routing/loading-ui-and-streaming)     | Loading UI for a segment and its children                                                                        |
| [`not-found`](https://nextjs.org/docs/app/api-reference/file-conventions/not-found)                     | Not found UI for a segment and its children                                                                      |
| [`error`](https://nextjs.org/docs/app/building-your-application/routing/error-handling)                 | Error UI for a segment and its children                                                                          |
| [`global-error`](https://nextjs.org/docs/app/building-your-application/routing/error-handling)          | Global Error UI                                                                                                  |
| [`route`](https://nextjs.org/docs/app/building-your-application/routing/route-handlers)                 | Server-side API endpoint                                                                                         |
| [`template`](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts#templates) | Specialized re-rendered Layout UI                                                                                |
| [`default`](https://nextjs.org/docs/app/api-reference/file-conventions/default)                         | Fallback UI for [Parallel Routes](https://nextjs.org/docs/app/building-your-application/routing/parallel-routes) |
 ## Component Hierarchy
 
 The React components defined in special files of a route segment are rendered in a specific hierarchy:

- `layout.js`
- `template.js`
- `error.js` (React error boundary)
- `loading.js` (React suspense boundary)
- `not-found.js` (React error boundary)
- `page.js` or nested `layout.js`

![Component Hierarchy for File Conventions](https://nextjs.org/_next/image?url=%2Fdocs%2Flight%2Ffile-conventions-component-hierarchy.png&w=3840&q=75)

