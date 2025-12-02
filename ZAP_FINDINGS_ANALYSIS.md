# ZAP DAST Findings Analysis - Exercise 3

## ZAP Finding Details

| Code | Issue | Risk | Affected | Why It Matters |
| :-- | :-- | :-- | :-- | :-- |
| 10020 | Missing Anti-clickjacking Header | Medium | http://localhost:5000 | Prevents clickjacking attacks where attackers overlay invisible iframes |
| 10021 | X-Content-Type-Options Header Missing | Low | http://localhost:5000 | Prevents MIME-sniffing attacks where browsers incorrectly interpret file types |
| 10036 | Server Leaks Version Information | Low | http://localhost:5000, http://localhost:5000/robots.txt, http://localhost:5000/sitemap.xml | Exposes Werkzeug/2.0.1 and Python/3.9.25, helping attackers identify vulnerabilities |
| 10038 | Content Security Policy (CSP) Header Not Set | Medium | http://localhost:5000, http://localhost:5000/robots.txt, http://localhost:5000/sitemap.xml | Prevents XSS and data injection attacks by controlling resource loading |
| 10049 | Storable and Cacheable Content | Info | http://localhost:5000, http://localhost:5000/robots.txt, http://localhost:5000/sitemap.xml | Content may be cached for 1 year, potentially exposing sensitive data |
| 10063 | Permissions Policy Header Not Set | Low | http://localhost:5000, http://localhost:5000/robots.txt, http://localhost:5000/sitemap.xml | Controls browser feature access (camera, microphone, location) |
| 10109 | Modern Web Application | Info | http://localhost:5000 | Suggests using Ajax Spider for more effective scanning |
| 90004 | Insufficient Site Isolation Against Spectre | Low | http://localhost:5000 | Missing cross-origin headers that mitigate Spectre side-channel attacks |
| 90005 | Sec-Fetch-Dest Header is Missing | Info | http://localhost:5000, http://localhost:5000/robots.txt, http://localhost:5000/sitemap.xml | Browser metadata headers for enhanced security (informational only) |
