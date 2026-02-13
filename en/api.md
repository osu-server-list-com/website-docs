<!---
ROUTE=api
TITLE=API
SORT=4
-->

The osu!Server List API provides programmatic access to server listings, live statistics, and voting endpoints used by the frontend and third-party integrations.

* * *

##### Base URL

All endpoints are available under the following base URL:

You can explore the full API surface and interactive documentation at our Swagger UI:

[https://api.osu-server-list.com/swagger](https://api.osu-server-list.com/swagger)

* * *

##### What the API provides

- Server listings and details (name, URL, description, tags)
- Live server statistics (player counts, status, ping)

##### Troubleshooting

- If an endpoint returns a 500 with a message like `500 Error parsing results ...`, the crawler or target server may be returning malformed JSON.
- Check the Swagger UI to confirm the expected response schema.

* * *

##### Contact

If you need access, documentation updates, or help integrating, visit our discord [https://discord.gg/gHp3PgmVAh](https://discord.gg/gHp3PgmVAh)