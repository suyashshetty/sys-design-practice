## Non Functional Requiments
1. Driver search should be highly available
2. Driver booking should be highly consistent, no two users should be booked the same driver
3. Ride request match should have minimal latency (< 60 sec)
4. Handle high throughput during special events (soccer event, new years eve, taylor swift concert. etc)

### Out of scope
1. Monitoring - Logging, analysis and alerting
2. Deployment - CI/CD pipeline
3. GDPR - User data deletion
4. Resilience and handling system faliures 