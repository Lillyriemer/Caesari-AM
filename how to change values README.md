# Caesari-AM Fund Performance Report

This is a custom-designed fund performance page, hosted via GitHub Pages and styled with brand-specific fonts and colors.

The page includes:
- Animated headline performance values
- A responsive performance history chart (powered by Chart.js)
- A performance comparison table
- Adobe Fonts integration

---

## ✅ How to Update Performance Data

You only need to edit **one file**: `index.html`

Click the file, press the ✏️ edit icon, and make your changes as described below.

---

### 1️⃣ Top Performance Cards

Located near the top of the file, in the JavaScript section:

```js
animateValue("lastMonth", 0, 2.1, 1500);
animateValue("ytd", 0, 3.2, 1500);
```

🟢 Change the `2.1` and `3.2` to your latest values.

You can also change the date labels here:

```html
<div class="card-subtext">Period: May 1 – May 31, 2025</div>
```

---

### 2️⃣ Performance Chart (Graph)

Located in the Chart.js section:

```js
labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May'],

datasets: [
  {
    label: 'Fund Performance',
    data: [0.5, 1.2, 1.8, 2.5, 3.2],
    ...
  },
  {
    label: 'Benchmark',
    data: [0.3, 0.9, 1.4, 2.0, 2.6],
    ...
  }
]
```

🟢 Change the `labels` if you add a new month (e.g., `'Jun'`)  
🟢 Update both `data` arrays with the new performance numbers

---

### 3️⃣ Performance Table

Located in the HTML body, under the table section:

```html
<tr><td>1 Month</td><td>+2.1%</td><td>+1.7%</td><td>+0.4%</td></tr>
```

🟢 Simply change the values between `<td>` tags for Fund, Benchmark, and Difference.

---

### 4️⃣ Footer Date

At the very bottom of the file:

```html
<footer>Data as of May 31, 2025. Past performance is not indicative of future results.</footer>
```

🟢 Update the reporting date here monthly.

---

## 💾 Saving Changes

Once you're done editing:

1. Scroll down to the bottom of the edit page
2. Write a short description (e.g., "Update June data")
3. Click **Commit changes**

✅ Your site will update automatically within seconds at:

```
https://lillyriemer.github.io/Caesari-AM/
```

---

## ✨ Need Help?

Feel free to open an issue or message the repo owner for help updating any section.
