
# Web Performance Metrics Guide

## 1. First Contentful Paint (FCP)

First Contentful Paint (FCP) measures how long it takes for the browser to display the first piece of content after a page starts loading.

### Examples of content

- Text
- Images
- SVG elements
- Canvas elements
- Background images

### Formula

```text
FCP = Time when the first content becomes visible
```

### Recommended values

| Value | Rating |
|------|------|
| Less than 1.8 s | Good |
| 1.8–3 s | Needs improvement |
| More than 3 s | Poor |

### How to improve FCP

- Reduce render-blocking resources.
- Compress images.
- Minify CSS and JavaScript.
- Use caching.
- Use a content delivery network (CDN).

---

## 2. Largest Contentful Paint (LCP)

Largest Contentful Paint (LCP) measures the time required to display the largest visible element in the viewport.

### Examples

- Hero images
- Videos
- Large text blocks
- Large headings

### Formula

```text
LCP = Time when the largest visible element is rendered
```

### Recommended values

| Value | Rating |
|------|------|
| Less than 2.5 s | Good |
| 2.5–4 s | Needs improvement |
| More than 4 s | Poor |

### How to improve LCP

- Optimize images.
- Reduce server response times.
- Remove unnecessary JavaScript.
- Enable caching.

---

## 3. Total Blocking Time (TBT)

Total Blocking Time (TBT) measures the amount of time during which the browser's main thread is blocked and unable to respond to user interactions.

### Formula

```text
Blocking time = Task duration – 50 ms

TBT = Sum of all blocking times
```

### Example

| Task | Duration | Blocking time |
|------|-----------|----------------|
| Task 1 | 40 ms | 0 ms |
| Task 2 | 120 ms | 70 ms |
| Task 3 | 200 ms | 150 ms |

### Recommended values

| Value | Rating |
|------|------|
| 0–200 ms | Good |
| 200–600 ms | Needs improvement |
| More than 600 ms | Poor |

### How to improve TBT

- Split large tasks into smaller tasks.
- Reduce JavaScript bundle sizes.
- Defer unnecessary scripts.
- Use web workers.

---

## 4. Cumulative Layout Shift (CLS)

Cumulative Layout Shift (CLS) measures the visual stability of a webpage.

### Formula

```text
CLS = Impact fraction × Distance fraction
```

### Recommended values

| Value | Rating |
|------|------|
| 0–0.1 | Good |
| 0.1–0.25 | Needs improvement |
| More than 0.25 | Poor |

### Common causes

- Images without dimensions
- Advertisements
- Embedded content
- Dynamically inserted elements
- Slow-loading fonts

### How to improve CLS

```html
<img src="image.jpg" width="800" height="400" alt="Image">
```

---

## 5. Speed Index (SI)

Speed Index (SI) measures how quickly visible content is displayed while the page is loading.

### Recommended values

| Value | Rating |
|------|------|
| Less than 3.4 s | Good |
| 3.4–5.8 s | Needs improvement |
| More than 5.8 s | Poor |

### How to improve the Speed Index

- Optimize images.
- Minify CSS and JavaScript files.
- Use lazy loading.
- Reduce HTTP requests.

---

## 6. Interaction to Next Paint (INP)

Interaction to Next Paint (INP) measures how quickly a webpage responds to user interactions such as clicks, taps, and keyboard input.

INP evaluates the time between the user's interaction and the moment the browser updates the screen.

### Formula

```text
INP = Input delay + Processing time + Presentation delay
```

### Recommended values

| Value | Rating |
|------|------|
| Less than 200 ms | Good |
| 200–500 ms | Needs improvement |
| More than 500 ms | Poor |

### Common causes of poor INP

- Excessive JavaScript execution
- Long-running tasks
- Frequent DOM updates
- Heavy third-party libraries

### How to improve INP

- Reduce JavaScript execution time.
- Break large tasks into smaller tasks.
- Optimize event handlers.
- Use asynchronous processing where possible.

---

## Comparison Table

| Metric | Description |
|------|------|
| FCP | Measures when the first content appears. |
| LCP | Measures when the largest content element appears. |
| TBT | Measures how long the browser remains unresponsive. |
| CLS | Measures layout stability. |
| Speed Index | Measures how quickly the page becomes visually complete. |
| INP | Measures responsiveness to user interactions. |

---

## Core Web Vitals

Google currently focuses on the following Core Web Vitals:

- Largest Contentful Paint (LCP)
- Cumulative Layout Shift (CLS)
- Interaction to Next Paint (INP)

FCP, TBT, and Speed Index are also valuable metrics and are commonly included in Lighthouse reports.
