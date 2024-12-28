# Next.js 15 Runtime Error: Invariant Violation

This repository demonstrates a common runtime error in Next.js 15 applications. The error occurs when a page component omits the necessary `React` import, even if it uses JSX.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to `/about`.

You should encounter the following error:

```
Invariant Violation: Element type is invalid: expected a string (for built-in components) or a class/function (for composite components) but got: undefined
```

## Solution

The error is resolved by explicitly importing `React` at the top of the `pages/about.js` file.  The solution is detailed in `bugSolution.js`

## Lessons Learned

- Always ensure you import `React` when using JSX in your Next.js components, even if your IDE doesn't explicitly show an error.
- This kind of error highlights the importance of thorough testing and careful attention to detail when developing Next.js applications. 