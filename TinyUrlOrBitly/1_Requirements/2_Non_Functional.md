## Non Functional Requiments
1. No two long urls should have same shortUrl. Short urls generation should be consistent
2. Redirection should be highly available to be able to access the original url.
3. Low latency for redirection (< 200 ms to redirect to original url)
4. Must support 100M DAU and 1B short urls

### Out of scope
1. Monitoring - Logging, analysis and alerting
2. Deployment - CI/CD pipeline
3. GDPR - User data deletion