# Client-Side Rendering (CSR) vs Server-Side Rendering (SSR) in Next.js

## Client-Side Rendering (CSR)

In **CSR**, the browser (client) is responsible for rendering the content. Initially, an HTML file is sent to the client, and JavaScript is used to fetch the required data and render the page dynamically.

### Characteristics:
- Loads a layout or spinner first, then fetches the actual data/content.
- Better for interactive apps where SEO isn't critical.
- Client-side components are rendered in the browser.

## Server-Side Rendering (SSR)

In **SSR**, the server generates the full HTML for the page before sending it to the browser. This allows the page to be displayed with content already present when it arrives at the client.

### Characteristics:
- Improves **SEO** (Search Engine Optimization).
- Reduces the loading time.
- Server components render on the server, and the HTML output is sent to the client.
- Can access files and folders, improving speed.

### Features in Next.js:
- **Next.js 15** fully supports **React 19**.
- **Turbopack**, a Rust-based bundler offering faster builds and improved performance during the development process.
- APIs that rely on request-specific data, such as headers, cookies, params, and `searchParams`, have transitioned to asynchronous functions.

## "use client" Directive

The `"use client"` directive is used to render client-side components (in the browser).

## Routing

In Next.js, dynamic routing is achieved using square brackets `[ ]`.

For example:
- **Dynamic route for user profiles**: `dashboard/users/[userId]`
  - Here, `userId` is a dynamic parameter that changes for each user.

## Route Groups

Route Groups allow you to create more organized and modular routes within your application.

## Layouts

You can use **layouts** in Next.js to display components that you want to show across multiple pages. This helps in keeping the structure of the app clean and reusable.

---

## Next Steps:

- To get started with **CSR** or **SSR** in your Next.js app, you can create components with the respective rendering strategy.
- Use dynamic routing for efficient handling of URLs with dynamic parameters.

---

For more information on Next.js, visit the [official Next.js documentation](https://nextjs.org/docs).
