# share-your-knowledge

A React (Create React App) course-registration form UI. The package name is `web23`.

## Overview

`src/App.js` sets up `BrowserRouter` with a `/register` route (`src/container/register/register.js`; a `home` container also exists). The register screen collects name, number, e-mail, age and available hours, lets the user pick courses, shows course details and a confirmation modal, and ends with a success illustration; a no-data illustration is shown on failure.

Course data is fetched with `hooks/get.js` (`APIGet`) from a hard-coded mock API URL (a mockapi.io `/courses` endpoint) and cached in a React context (`src/context/dataContext.js`). The form does not submit to a backend in this repository.

UI pieces: `components/cta` (buttons), `components/form` (input), `components/modals`, `components/navigation/header.js`. Styles are SCSS with Bootstrap.

## Scripts

```
npm start       # development server on http://localhost:3000
npm run build   # production build
npm test        # test runner
```
