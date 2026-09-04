# Saxo Samples Company Application

A full-stack React, Tailwind CSS, Express, and SQLite application covering secure registration, email OTP verification, persistent authentication, sample request creation/viewing, factory delivery management, and follow-up controls.

## Run locally

```bash
cp .env.example .env
npm install
npm run dev
```

The web application runs on `http://localhost:5173` and proxies API requests to port 4000. Configure SMTP variables to send real OTP email. Without SMTP, development mode displays the OTP on the verification page. Admin, office, and factory allowlists are configured through the corresponding comma-separated environment variables.

Passwords use bcrypt hashes. Session JWTs expire after seven days. SQLite data is stored under `data/` and is intentionally excluded from version control.
