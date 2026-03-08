[package.json](https://github.com/user-attachments/files/25824376/package.json)
{
  "name": "og-api",
  "version": "1.0.0",
  "description": "OG Metadata extraction API with redirect following"
}
[vercel.json](https://github.com/user-attachments/files/25824378/vercel.json)
{
  "version": 2,
  "functions": {
    "api/og.js": {
      "runtime": "nodejs20.x"
    }
  },
  "headers": [
    {
      "source": "/api/(.*)",
      "headers": [
        { "key": "Access-Control-Allow-Origin", "value": "*" },
        { "key": "Access-Control-Allow-Methods", "value": "GET, OPTIONS" }
      ]
    }
  ]
}
