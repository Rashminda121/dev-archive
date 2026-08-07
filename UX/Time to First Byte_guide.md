# Time to First Byte (TTFB)

## Overview

**Time to First Byte (TTFB)** measures the amount of time required for a browser to receive the **first byte of data** from the server after sending an HTTP request.

In simple terms, TTFB answers the following question:

> How quickly does the server begin responding?

TTFB includes:

- DNS lookup time
- Connection establishment time
- TLS negotiation time
- Server processing time
- Network latency

---

## Formula

```text
TTFB = DNS lookup time
     + Connection time
     + TLS negotiation time
     + Server processing time
     + Response transfer time
```

---

## Example

| Stage | Time |
|------|------|
| DNS lookup | 20 ms |
| Connection | 30 ms |
| TLS handshake | 50 ms |
| Server processing | 120 ms |
| First-byte transfer | 30 ms |

```text
TTFB = 20 + 30 + 50 + 120 + 30

TTFB = 250 ms
```

---

## Recommended values

| Value | Rating |
|------|------|
| Less than 200 ms | Good |
| 200–500 ms | Needs improvement |
| More than 500 ms | Poor |

---

## Common causes of poor TTFB

- Slow web servers
- Inefficient database queries
- Long API execution times
- Large numbers of redirects
- High network latency
- Missing caching mechanisms

---

## How to improve TTFB

- Use a Content Delivery Network (CDN).
- Enable browser and server-side caching.
- Optimize database queries.
- Reduce server processing time.
- Compress assets.
- Upgrade server infrastructure.

---

# How to check TTFB

## Method 1: Chrome DevTools

1. Open the website in Google Chrome.
2. Press **F12** to open Developer Tools.
3. Select the **Network** tab.
4. Refresh the page.
5. Click the first request.
6. Open the **Timing** section.
7. Locate **Waiting (TTFB)**.

Example:

```text
Network
└── Request
    └── Timing
        └── Waiting (TTFB): 180 ms
```

---

## Method 2: Lighthouse

1. Open Chrome Developer Tools.
2. Select **Lighthouse**.
3. Click **Analyze page load**.
4. Review the performance report.

---

## Method 3: PageSpeed Insights

1. Open PageSpeed Insights.
2. Enter the website URL.
3. Run the analysis.
4. Review the TTFB value.

---

## Method 4: WebPageTest

1. Open WebPageTest.
2. Enter the website URL.
3. Select a testing location.
4. Start the test.
5. Review the timing report.

---

## Relationship with other metrics

| Metric | Purpose |
|------|------|
| TTFB | Measures server responsiveness. |
| FCP | Measures when the first content appears. |
| LCP | Measures when the largest element appears. |
| TBT | Measures how long the browser remains blocked. |
| CLS | Measures visual stability. |
| INP | Measures interaction responsiveness. |

A high TTFB value often negatively affects most of the other performance metrics.
