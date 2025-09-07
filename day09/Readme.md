# 🔹 Quick Revision Summary – Sizing Units & Elements

## 🏷️ HTML Basics

* `<!DOCTYPE html>` → Defines HTML5 document type.
* `<html lang="en">` → Root element, with language set to English.
* `<head>` → Metadata, styles, title.
* `<meta charset="UTF-8">` → Defines character encoding (supports all characters).
* `<meta name="viewport" content="width=device-width, initial-scale=1.0">` → Ensures responsive design on mobile devices.
* `<title>` → Title of the web page (shown in browser tab).
* `<style>` → Internal CSS.

### Body Elements

* `<div>` → Generic block container.
* `<p>` → Paragraph text.

---

## 🎨 CSS Basics in Your Code

### 🔹 Universal Selector

```css
* {
  margin: 0;
  padding: 0;
}
```

* Resets default margin/padding for all elements.

---

### 🔹 Root Font Size

```css
html {
  font-size: 12px;
}
```

* Sets root size → useful for `rem` calculations.
* Default browser font-size = **16px**.

---

### 🔹 Box Example

```css
.box {
  border: 2px solid black;
  background-color: aqua;
  box-sizing: border-box;
  width: 80vw;      /* 80% of viewport width */
  height: 10vh;     /* 10% of viewport height */
  min-height: 80vh; /* at least 80% of viewport height */
  margin: auto;     /* center horizontally */
}
```

* **`box-sizing: border-box;`** → Padding + border included inside width/height.
* **Nested `<div>` widths (`50%`)** → Percentages depend on **parent’s width**.

---

### 🔹 Container Example

```css
.container {
  width: 80vw;
  min-height: 80vh;
  margin: 23px auto;  /* vertical + horizontal margins */
  font-size: 18px;    /* fixed size in px */
}
.container p {
  font-size: 1em;  /* equal to parent’s font-size (18px) */
  font-size: 2em;  /* 2 × parent’s size = 36px */
  font-size: 2rem; /* 2 × root size (12px) = 24px */
}
```

👉 **Key point:**

* `em` → Relative to parent.
* `rem` → Relative to root (`html`).

---

### 🔹 My Container Example

```css
.mycont {
  color: yellow;
  background-color: red;
  border: 2px solid black;
  font-size: 22px;
  width: 80vw;
  margin: auto;
  /* width: 100vmin; height: 100vmax; */
}
```

* **`vmin`** → Relative to smaller side of viewport.
* **`vmax`** → Relative to larger side of viewport.

---

## 📏 CSS Units You Practiced

* **px** → Fixed pixels (absolute).
* **%** → Relative to parent element.
* **vw / vh** → Relative to viewport width / height.
* **vmin / vmax** → Relative to smaller / larger viewport side.
* **em** → Relative to parent element’s font size.
* **rem** → Relative to root element’s font size.

---

## 📝 Extra Notes

* `margin: auto;` works only on **block elements** (not inline like `<span>`).
* **Nested % widths** → Each % is based on its **direct parent’s size**, not the full viewport.
* `min-height` / `min-width` → Prevents shrinking below a threshold.
* Comments in CSS → `/* … */`

---

✅ **In short, you learned how different CSS units (`px, %, vw, vh, em, rem, vmin, vmax`) behave, how nesting affects sizes, and how to use margins, borders, and font scaling.**

---

Do you want me to make a **visual diagram (flow-style)** showing relationships between `em`, `rem`, `%`, and `vw/vh` so you can recall even faster?
