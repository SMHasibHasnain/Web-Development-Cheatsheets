# 🎓 CSS Selectors Master Reference
This repository provides a **comprehensive, categorized, and example-rich reference of all CSS selectors**, ideal for software engineering students, researchers, and frontend developers.

---

## 📘 Table of Contents

- [Basic Selectors](#basic-selectors)
- [Combinator Selectors](#combinator-selectors)
- [Attribute Selectors](#attribute-selectors)
- [Pseudo-Class Selectors](#pseudo-class-selectors)
    - [Structural Pseudo-Classes](#structural-pseudo-classes)
    - [Type-Specific Pseudo-Classes](#type-specific-pseudo-classes)
    - [UI/State-Based Pseudo-Classes](#uistate-based-pseudo-classes)
- [Pseudo-Element Selectors](#pseudo-element-selectors)
- [Logical & Negation Selectors](#logical--negation-selectors)
- [Advanced Selector Combinations](#advanced-selector-combinations)
- [Quick Summary Table](#quick-summary-table)
- [Further Reading](#further-reading)

---

## 🧱 Basic Selectors

| Selector | Example | Description |
|----------|---------|-------------|
| `*` | `* { margin: 0; }` | Universal selector (everything) |
| `element` | `p { color: red; }` | Type selector |
| `.class` | `.intro { font-size: 18px; }` | Class selector |
| `#id` | `#main { padding: 20px; }` | ID selector |
| `A, B` | `h1, p { font-family: serif; }` | Group selector |

🧠 **Tip:** `*` = all, `.` = many, `#` = one.

---

## 🧩 Combinator Selectors

| Selector | Example | Meaning |
|----------|---------|---------|
| `A B` | `div p {}` | Descendant |
| `A > B` | `ul > li {}` | Direct child |
| `A + B` | `h1 + p {}` | Immediate sibling |
| `A ~ B` | `h1 ~ p {}` | All following siblings |

🧠 **Hierarchy Logic:** Space = nested, `>` = child, `+` = next, `~` = all next siblings.

---

## 🧬 Attribute Selectors

| Selector | Example | Description |
|----------|---------|-------------|
| `[attr]` | `[type]` | Has attribute |
| `[attr=value]` | `[type="text"]` | Exact match |
| `[attr~=value]` | `[title~="tip"]` | Contains word |
| `[attr|=value]` | `[lang|="en"]` | Lang or lang-* |
| `[attr^=value]` | `[href^="https"]` | Starts with |
| `[attr$=value]` | `[href$=".pdf"]` | Ends with |
| `[attr*=value]` | `[class*="nav"]` | Contains substring |

🧠 **Memory Trick:**
- `^=` → starts with
- `$=` → ends with
- `*=` → contains
- `~=` → word contains

---

## 🎭 Pseudo-Class Selectors

### 🔢 Structural Pseudo-Classes

| Selector | Example | Description |
|----------|---------|-------------|
| `:first-child` | `li:first-child` | First child |
| `:last-child` | `li:last-child` | Last child |
| `:nth-child(n)` | `li:nth-child(2)` | nth child |
| `:nth-last-child(n)` | `li:nth-last-child(2)` | nth-from-end |
| `:only-child` | `p:only-child` | Sole child |

### 🔤 Type-Specific Pseudo-Classes

| Selector | Example | Description |
|----------|---------|-------------|
| `:first-of-type` | `p:first-of-type` | First of its type |
| `:last-of-type` | `p:last-of-type` | Last of its type |
| `:nth-of-type(n)` | `p:nth-of-type(2)` | nth of type |
| `:only-of-type` | `p:only-of-type` | Sole of type |

### 🧑‍💻 UI/State-Based Pseudo-Classes

| Selector | Example | Description |
|----------|---------|-------------|
| `:hover` | `a:hover` | On hover |
| `:focus` | `input:focus` | On focus |
| `:active` | `button:active` | When clicked |
| `:visited` | `a:visited` | Visited link |
| `:checked` | `input:checked` | Checked |
| `:disabled` | `input:disabled` | Disabled input |
| `:enabled` | `input:enabled` | Enabled input |

---

## 🧪 Pseudo-Element Selectors

| Selector | Example | Description |
|----------|---------|-------------|
| `::before` | `p::before { content: "✔ "; }` | Content before |
| `::after` | `p::after { content: " ✖"; }` | Content after |
| `::first-line` | `p::first-line` | First line styling |
| `::first-letter` | `p::first-letter` | First letter styling |
| `::selection` | `p::selection` | Highlight styling |

🧠 **Colon Guide:**  
Old syntax: `:before`, modern: `::before`.

---

## ⚙️ Logical & Negation Selectors

| Selector | Example | Description |
|----------|---------|-------------|
| `:not()` | `div:not(.active)` | Exclude selector |
| `:is()` | `:is(h1, h2)` | Match any group |
| `:where()` | `:where(h1, h2)` | No specificity |
| `:has()` | `div:has(img)` | Parent with child (⚠️ limited support) |

---

## 🛰️ Advanced Selector Combinations

| Pattern | Example | Description |
|--------|---------|-------------|
| `.btn.primary:hover` | Combines class and state |
| `section > ul > li:nth-child(odd)` | Structured targeting |
| `a[href^="https"]:not(.external)` | Filter by attribute and class |
| `ul li:last-of-type::after` | Target and enhance last item |
| `:is(header, footer) a` | Target scoped links |

---

## 🧾 Quick Summary Table

| Category | Example | Notes |
|----------|---------|-------|
| Basic | `div`, `.box`, `#id` | Element, Class, ID |
| Combinator | `div > p`, `h1 + p` | Hierarchical |
| Attribute | `[href^="http"]` | Filter by attributes |
| Pseudo-Class | `li:first-child` | State/position |
| Pseudo-Element | `::before` | Fake element styling |
| Logical | `:not()`, `:is()` | Conditional logic |

---

## 📚 Further Reading

- [MDN CSS Selectors Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- *CSS: The Definitive Guide* – Eric A. Meyer
- [CSS-Tricks Selector Almanac](https://css-tricks.com/almanac/selectors/)

---

## ✅ License

This reference is published under the MIT License. Free to use for education and research purposes.

---

### ✍️ Maintainer

**Hasib Hasnain** – [hasibhasnain.com](https://hasibhasnain.com)  
