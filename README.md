# Request Header Parser Microservice

# `/api/whoami` API Documentation

This API endpoint provides information about the client making the request.

## Endpoint

`GET /api/whoami`

## Response

The response is a JSON object containing the following keys:

- `ipaddress`: The IP address of the client.
- `language`: The preferred language of the client, derived from the `Accept-Language` header.
- `software`: Information about the client's software, including operating system and browser, derived from the `User-Agent` header.

### Example Response

```json
{
  "ipaddress": "93.184.216.34",
  "language": "en-US,en;q=0.5",
  "software": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
}
