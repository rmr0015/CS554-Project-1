# Project 1 Starter – EC2 REST Converter

This is a minimal Node.js/Express service that converts pounds (lbs) to kilograms (kg).

## Run locally

```bash
npm install
node server.js
```

Then test:

```bash
curl "http://localhost:8080/convert?lbs=150"
curl "http://localhost:8080/convert?lbs=0"
curl "http://localhost:8080/convert?lbs=0.1"
curl "http://localhost:8080/convert"
curl "http://localhost:8080/convert?lbs=-5"
curl "http://localhost:8080/convert?lbs=NaN"
```

## Deploy on EC2

1. Launch EC2 (Amazon Linux 2 or Ubuntu).
2. Install Node.js + npm.
3. Clone or copy this repo to EC2 instance.
4. Run `npm install && node server.js`.
5. Adjust Security Group to allow inbound TCP/8080 (or use NGINX reverse proxy for port 80).
