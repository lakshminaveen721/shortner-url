# URL Shortener Microservice

## Features

- POST a URL to `/api/shorturl` → `{ original_url, short_url }`
- GET `/api/shorturl/:short_url` → Redirects to original URL
- Invalid URL → `{ error: "invalid url" }`

## Run Locally

```bash
npm install
npm start
```

## Example

POST `http://localhost:3000/api/shorturl`  
Body: `url=https://freecodecamp.org`  
→ Response: `{ original_url: "...", short_url: 1 }`

GET `http://localhost:3000/api/shorturl/1`  
→ Redirects to `https://freecodecamp.org`
