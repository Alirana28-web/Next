# Client-Side Rendering (CSR) vs Server-Side Rendering (SSR) in Next.js

## Client-Side Rendering (CSR)
In **CSR**, the browser (client) is responsible for rendering the content. Initially, an HTML file is sent to the client, and JavaScript is used to fetch the required data and render the page dynamically.

### Characteristics:
- Loads a layout or spinner first, then fetches the actual data/content.
- Better for interactive apps where SEO isn't critical.
- Client-side components are rendered in the browser.

---

## Server-Side Rendering (SSR)
In **SSR**, the server generates the full HTML for the page before sending it to the browser. This allows the page to be displayed with content already present when it arrives at the client.

### Characteristics:
- Improves **SEO** (Search Engine Optimization).
- Reduces the loading time.
- Server components render on the server, and the HTML output is sent to the client.
- Can access files and folders, improving speed.
- Faster processing for data-intensive apps.

---

## Features in Next.js

### Latest Enhancements:
- **Next.js 15** fully supports **React 19**.
- **Turbopack**: A Rust-based bundler offering faster builds and improved performance during development.
- APIs that rely on request-specific data, such as headers, cookies, params, and `searchParams`, have transitioned to asynchronous functions.

---

## "use client" Directive
- The `"use client"` directive is used to render client-side components in the browser, ensuring dynamic interactivity where needed.
- **Event Handling**: Buttons, forms, modals, and other interactive UI elements need client-side JavaScript to handle events like onClick, onSubmit, etc.
- **State Management**: Dynamic behavior requiring hooks like useState or useEffect can only work in Client Components.
---

## Routing
- **Dynamic Routing**: Use square brackets `[]` for dynamic route parameters.
  
  Example:
  - Dynamic route for user profiles: `dashboard/users/[userId]`
    - Here, `userId` is a dynamic parameter that changes for each user.

---

## Layouts
You can use **layouts** in Next.js to display components across multiple pages, keeping the structure of the app clean and reusable.

### Example:
A layout can include components like a navigation bar or footer that appear on every page.

---

## Route Groups
Route Groups help organize and modularize routes within your application.
- Folder names can be written in parentheses (e.g., `(dashboard)`), and their content can be accessed without including the folder name in the URL.
  
### Example:
For a `dashboard` folder:
- Structure: `dashboard/users`
- URL: `/users` (no need to include `dashboard` in the URL).

---

## Additional Features
- **HMR (Hot Module Replacement)**: Enables instant updates to components without refreshing the page.
- **AMD (Automatic Request Deduplication)**: Optimizes API requests by avoiding duplicate calls.

---

For more information on Next.js, visit the [official Next.js documentation](https://nextjs.org/docs).

