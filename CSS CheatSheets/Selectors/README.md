# 🎓 CSS Selectors Master Reference

This repository provides a **comprehensive, categorized, and example-rich reference of all CSS selectors**, ideal for software engineering students, researchers, and frontend developers.

---

## 📚 Table of Contents

- [🧱 Basic Selectors](#-basic-selectors)
- [Combinator Selectors](#combinator-selectors)
- [🧬 Attribute Selectors](#-attribute-selectors)
- [🎭 Pseudo-Class Selectors](#-pseudo-class-selectors)
  - [🔢 Structural Pseudo-Classes](#-structural-pseudo-classes)
  - [🔤 Type-Specific Pseudo-Classes](#-type-specific-pseudo-classes)
  - [👩‍💻 UI/State-Based Pseudo-Classes](#-uistate-based-pseudo-classes)
  - [✅ Form and Input Validation Pseudo-Classes](#-form-and-input-validation-pseudo-classes)
  - [🌍 Language, Direction, and Link Pseudo-Classes](#-language-direction-and-link-pseudo-classes)
- [🧾 Pseudo-Element Selectors](#-pseudo-element-selectors)
- [⚙️ Logical & Negation Selectors](#️-logical--negation-selectors)
- [🚀 Advanced Selector Combinations](#-advanced-selector-combinations)
- [🧭 Usage Frequency Key](#-usage-frequency-key)
- [📖 Further Reading](#-further-reading)
- [✅ License](#-license)
- [✍️ Maintainer](#️-maintainer)

---

## 🧱 Basic Selectors

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `*` | `* { margin: 0; }` | Universal selector | 🔸 Medium |
| `element` | `p { color: red; }` | Type selector | 🔹 High |
| `.class` | `.intro { font-size: 18px; }` | Class selector | 🔷 Very High |
| `#id` | `#main { padding: 20px; }` | ID selector | 🔹 High |
| `A, B` | `h1, p { font-family: serif; }` | Group selector | 🔸 Medium |

---

## Combinator Selectors

| Selector | Example | Meaning | Usage |
|----------|---------|---------|--------|
| `A B` | `div p {}` | Descendant | 🔷 Very High |
| `A > B` | `ul > li {}` | Direct child | 🔹 High |
| `A + B` | `h1 + p {}` | Immediate sibling | 🔸 Medium |
| `A ~ B` | `h1 ~ p {}` | All following siblings | 🔸 Medium |

---

## 🧬 Attribute Selectors

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `[attr]` | `[type]` | Has attribute | 🔸 Medium |
| `[attr=value]` | `[type="text"]` | Exact match | 🔸 Medium |
| `[attr~=value]` | `[title~="tip"]` | Contains word | 🔸 Medium |
| `[attr|=value]` | `[lang|="en"]` | Lang or lang-* | 🔹 Low |
| `[attr^=value]` | `[href^="https"]` | Starts with | 🔸 Medium |
| `[attr$=value]` | `[href$=".pdf"]` | Ends with | 🔸 Medium |
| `[attr*=value]` | `[class*="nav"]` | Contains substring | 🔸 Medium |

---

## 🎭 Pseudo-Class Selectors

### 🔢 Structural Pseudo-Classes

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:first-child` | `li:first-child` | First child | 🔹 High |
| `:last-child` | `li:last-child` | Last child | 🔹 High |
| `:nth-child(n)` | `li:nth-child(2)` | nth child | 🔸 Medium |
| `:nth-last-child(n)` | `li:nth-last-child(2)` | nth-from-end | 🔸 Medium |
| `:only-child` | `p:only-child` | Sole child | 🔹 Low |

### 🔤 Type-Specific Pseudo-Classes

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:first-of-type` | `p:first-of-type` | First of its type | 🔹 Medium |
| `:last-of-type` | `p:last-of-type` | Last of its type | 🔹 Medium |
| `:nth-of-type(n)` | `p:nth-of-type(2)` | nth of type | 🔹 Medium |
| `:only-of-type` | `p:only-of-type` | Sole of type | 🔹 Low |

### 👩‍💻 UI/State-Based Pseudo-Classes

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:hover` | `a:hover` | On hover | 🔷 Very High |
| `:focus` | `input:focus` | On focus | 🔷 Very High |
| `:active` | `button:active` | When clicked | 🔷 Very High |
| `:visited` | `a:visited` | Visited link | 🔸 Medium |
| `:checked` | `input:checked` | Checked | 🔹 Medium |
| `:disabled` | `input:disabled` | Disabled input | 🔹 Medium |
| `:enabled` | `input:enabled` | Enabled input | 🔹 Medium |
| `:indeterminate` | `input:indeterminate` | Mixed checkbox state | 🔹 Low |
| `:default` | `input:default` | Default input | 🔹 Low |

### ✅ Form and Input Validation Pseudo-Classes

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:valid` | `input:valid` | Valid input | 🔹 Medium |
| `:invalid` | `input:invalid` | Invalid input | 🔹 Medium |
| `:required` | `input:required` | Required field | 🔹 Medium |
| `:optional` | `input:optional` | Optional field | 🔹 Medium |
| `:in-range` | `input:in-range` | In range value | 🔹 Low |
| `:out-of-range` | `input:out-of-range` | Out of range value | 🔹 Low |
| `:read-only` | `input:read-only` | Not editable | 🔹 Low |
| `:read-write` | `textarea:read-write` | Editable | 🔹 Low |

### 🌍 Language, Direction, and Link Pseudo-Classes

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:lang()` | `p:lang(en)` | Language match | 🔹 Low |
| `:dir()` | `div:dir(rtl)` | Direction match | 🔹 Low |
| `:link` | `a:link` | Unvisited link | 🔹 Medium |
| `:target` | `#section:target` | URL anchor target | 🔹 Low |
| `:empty` | `div:empty` | No content | 🔹 Medium |
| `:root` | `:root` | Document root | 🔷 Very High |

---

## 🧾 Pseudo-Element Selectors

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `::before` | `p::before` | Content before | 🔷 Very High |
| `::after` | `p::after` | Content after | 🔷 Very High |
| `::first-line` | `p::first-line` | First line | 🔹 Low |
| `::first-letter` | `p::first-letter` | First letter | 🔹 Low |
| `::selection` | `p::selection` | Highlight styling | 🔹 Medium |
| `::placeholder` | `input::placeholder` | Input placeholder | 🔷 High |
| `::marker` | `li::marker` | List bullet marker | 🔹 Medium |
| `::cue` | `::cue` | Subtitle text | 🔹 Low |

---

## ⚙️ Logical & Negation Selectors

| Selector | Example | Description | Usage |
|----------|---------|-------------|--------|
| `:not()` | `div:not(.active)` | Exclude selector | 🔷 Very High |
| `:is()` | `:is(h1, h2)` | Match any group | 🔹 Medium |
| `:where()` | `:where(h1, h2)` | 0 specificity selector | 🔹 Medium |
| `:has()` | `div:has(img)` | Parent with child (⚠️ limited support) | 🔹 Medium |

---

## 🚀 Advanced Selector Combinations

| Pattern | Example | Description |
|--------|---------|-------------|
| `.btn.primary:hover` | Combine class and state |
| `section > ul > li:nth-child(odd)` | Nested + structural |
| `a[href^="https"]:not(.external)` | Attribute + logic |
| `ul li:last-of-type::after` | Structural + pseudo-element |
| `:is(header, footer) a` | Logical group targeting |

---

## 🧭 Usage Frequency Key

- 🔷 **Very High** – Used in nearly every project
- 🔹 **High** – Frequently encountered in real-world CSS
- 🔸 **Medium** – Occasional use in dynamic/UI-based scenarios
- 🔻 **Low** – Niche, special cases, or accessibility-heavy

---

## 📖 Further Reading

- [MDN CSS Selectors Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- *CSS: The Definitive Guide* – Eric A. Meyer
- [CSS-Tricks Selector Almanac](https://css-tricks.com/almanac/selectors/)

---

## ✅ License

This reference is published under the MIT License. Free to use for education and research purposes.

---

### ✍️ Maintainer

**Hasib Hasnain**  
[hasibhasnain.com](https://hasibhasnain.com)
