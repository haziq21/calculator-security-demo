# Scanner Comparison

## Only CodeQL (SAST) Found
- Flask debug mode enabled
- Code patterns and logic errors
- Data flow vulnerabilities
- Insecure configuration in app.py

## Only ZAP (DAST) Found
- Missing security headers
- Server version information leakage
- Runtime configuration issues
- Permissions Policy not set
- Cross-Origin isolation headers missing
- Cacheable content without proper cache controls

## Only Dependency-Check (SCA) Found
- No vulnerabilities detected in this scan

## All Three Tools
- None - they focus on different layers
