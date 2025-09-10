# Mortgage Repayment Planner

A simple **Svelte 5 web app** that helps you explore different repayment strategies for a mortgage (or any loan). You can:

- Enter your current balance and annual interest rate
- Set a baseline monthly repayment
- Compare it against two alternative repayment amounts
- Visualize the **loan balance over time** with a chart
- See a **comparison table** showing payoff time, interest, total repayment, and savings

This tool is currency agnostic — just input your values in your local currency.

---

## Features
- Built with **Svelte 5**
- Interactive loan payoff simulation
- Dynamic **line chart** using ApexCharts
- Side-by-side **comparison table**
- Configurable repayment amounts
- Shows **interest saved** and **months saved** vs baseline

---

## Setup Instructions

### 1. Initialize a new project
```bash
npm create vite@latest mortgage-planner -- --template svelte
cd mortgage-planner
```

### 2. Install dependencies
```bash
npm install
npm install svelte-apexcharts apexcharts tailwindcss postcss autoprefixer -D
```

### 3. Configure Tailwind (optional, for styling)
```bash
npx tailwindcss init -p
```
Update `tailwind.config.cjs` to include:
```js
content: [
  "./index.html",
  "./src/**/*.{svelte,js,ts}"
]
```

Add Tailwind imports in `src/app.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 4. Add the planner component
Replace `src/App.svelte` with the provided code from this repo.

### 5. Run the dev server
```bash
npm run dev
```

---

## Packages Required
- **svelte** (v5)
- **svelte-apexcharts**
- **apexcharts**
- **tailwindcss** (optional, for styling)

---

## Notes
- This planner is approximate. It assumes fixed interest and ignores special cases like moratoriums or progressive disbursements.
- Use it as a planning tool, not an exact financial calculator.

---

## License
MIT
