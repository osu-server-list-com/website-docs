<!---
ROUTE=crawler
TITLE=Crawler
SORT=3
-->

The osu!Server List Crawler is an automated system that periodically collects statistics from registered osu! private servers and performs real-time voting verification.

* * *

##### What Does the Crawler Do?

The crawler performs several essential tasks to keep server information up-to-date:

- **Statistics Collection**: Gathers player counts, server status, and other vital metrics
- **Vote Verification**: Validates voting actions in real-time to ensure users exist on the target server
- **Server Health Monitoring**: Checks server availability and response times
- **Data Synchronization**: Updates server listings with the latest information

* * *

##### User Agent

All requests from our crawler use the following user-agent string:

```
osu!ListBot/3.0 (+https://osu-server-list.com/docs/crawler)
```

You can use this identifier to whitelist our crawler in your server's access logs or security configurations.

* * *

##### Crawler Behavior

- **Frequency**: Servers are crawled every 15 minutes
- **Timeout**: Requests timeout after 5 seconds

* * *

##### Troubleshooting

###### My server isn't showing updated statistics

- Verify the crawler can access your API endpoints
- Check your server logs for requests from `osu!ListBot/3.0`
- Ensure your API returns valid JSON responses
- Contact support if the issue persists

###### The crawler is being blocked

- Whitelist the user-agent `osu!ListBot/3.0`
- Check your firewall settings
- Review rate limiting rules

* * *

###### Privacy & Security

- The crawler only accesses publicly available API endpoints
- No authentication credentials are stored or transmitted
- All data is transmitted securely when HTTPS is available