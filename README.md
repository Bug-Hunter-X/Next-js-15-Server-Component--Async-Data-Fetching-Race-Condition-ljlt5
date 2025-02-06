# Next.js 15 Server Component: Async Data Fetching Race Condition

This repository demonstrates a subtle bug in Next.js 15 server components related to asynchronous data fetching. When a server component attempts to use data fetched asynchronously within the same component before the fetch completes, it may lead to unexpected `undefined` values being used, which can cause component rendering errors.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe the unexpected behavior on the page.