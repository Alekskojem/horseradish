# Copilot Instructions for horseradish

## Project Overview
This is a React application bootstrapped with Create React App. The main entry point is `src/index.js`, and the root component is `src/App.js`. Static assets and configuration files are located in the `public/` directory.

## Key Workflows
- **Install dependencies:** `npm install`
- **Start development server:** `npm start` (serves at http://localhost:3000)
- **Run tests:** `npm test` (Jest, interactive watch mode)
- **Build for production:** `npm run build` (outputs to `build/`)

## File Structure
- `src/` — Main source code
  - `App.js` — Root React component
  - `index.js` — Entry point, renders `App`
  - `App.css`, `index.css` — Stylesheets
  - `App.test.js` — Example test file
  - `reportWebVitals.js` — Performance reporting (optional)
  - `setupTests.js` — Jest setup
- `public/` — Static assets
  - `index.html` — Main HTML template
  - `manifest.json` — PWA manifest
  - `robots.txt` — Crawler rules

## Patterns & Conventions
- **Component organization:** All components are currently in a flat structure under `src/`. For new features, create additional components in `src/` or a subfolder if complexity grows.
- **Styling:** Use CSS files imported directly into JS modules. No CSS-in-JS or styled-components by default.
- **Testing:** Use Jest and React Testing Library. Example test in `App.test.js`.
- **Performance:** Optional web vitals reporting via `reportWebVitals.js`.

## Integration Points
- No custom backend or API integration is present by default. Add API calls in new components as needed.
- No Redux, MobX, or other state management libraries are used unless added manually.

## Project-Specific Notes
- This project follows Create React App conventions. Avoid ejecting unless absolutely necessary.
- All build and test commands are standard; no custom scripts or build steps are present.
- For deployment, use the output in the `build/` directory.

## Example: Adding a New Component
1. Create `src/MyComponent.js`:
   ```js
   import React from 'react';
   export default function MyComponent() {
     return <div>Hello from MyComponent!</div>;
   }
   ```
2. Import and use in `App.js`:
   ```js
   import MyComponent from './MyComponent';
   // ...
   <MyComponent />
   ```

## References
// Документацію по Create React App та React шукайте онлайн, зовнішні посилання тут не підтримуються.

---
_If any conventions or workflows are unclear, please provide feedback to improve these instructions._
