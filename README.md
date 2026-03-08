[vercel.json](https://github.com/user-attachments/files/25824380/vercel.json)
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
