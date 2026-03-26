# Code Citations

## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
```


## License: unknown
https://github.com/nisharga/Deployment/blob/ffcdc2cd2130486aa9d63c3f6e176805ee55c83d/README.md

```
Here's everything you need:

## Required Environment Variables (27 total)

| Variable | How to Get It |
|---|---|
| `NODE_ENV` | Set to `production` |
| `PORT` | Vercel sets this automatically, use `5000` as default |
| `DATABASE_URL` | PostgreSQL connection string — use [Neon](https://neon.tech), [Supabase](https://supabase.com), or [Railway](https://railway.app) for a hosted Postgres DB |
| **Auth** | |
| `BETTER_AUTH_SECRET` | Generate: `openssl rand -base64 32` |
| `BETTER_AUTH_URL` | Your deployed Vercel URL, e.g. `https://your-app.vercel.app` |
| `ACCESS_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `REFRESH_TOKEN_SECRET` | Generate: `openssl rand -base64 32` |
| `ACCESS_TOKEN_EXPIRES_IN` | e.g. `1d` |
| `REFRESH_TOKEN_EXPIRES_IN` | e.g. `7d` |
| `BETTER_AUTH_SESSION_TOKEN_EXPIRES_IN` | e.g. `604800` (7 days in seconds) |
| `BETTER_AUTH_SESSION_TOKEN_UPDATE_AGE` | e.g. `86400` (1 day in seconds) |
| **Email (Gmail SMTP)** | |
| `EMAIL_SENDER_SMTP_USER` | Your Gmail address |
| `EMAIL_SENDER_SMTP_PASS` | Gmail App Password — [generate here](https://myaccount.google.com/apppasswords) (requires 2FA) |
| `EMAIL_SENDER_SMTP_HOST` | `smtp.gmail.com` |
| `EMAIL_SENDER_SMTP_PORT` | `465` |
| `EMAIL_SENDER_SMTP_FROM` | Your sender email address |
| **Google OAuth** | |
| `GOOGLE_CLIENT_ID` | From [Google Cloud Console](https://console.cloud.google.com/apis/credentials) → Create OAuth 2.0 Client ID |
| `GOOGLE_CLIENT_SECRET` | Same place as above |
| `GOOGLE_CALLBACK_URL` | `https://your-app.vercel.app/api/auth/callback/google` |
| **Frontend** | |
| `FRONTEND_URL` | Your deployed frontend URL |
| **Cloudinary** | |
| `CLOUDINARY_CLOUD_NAME` | From [Cloudinary Dashboard](https://cloudinary.com/console) |
| `CLOUDINARY_API_KEY` | Same dashboard |
| `CLOUDINARY_API_SECRET` | Same dashboard |
| **Stripe** | |
| `STRIPE_SECRET_KEY` | From [Stripe Dashboard](https://dashboard.stripe.com/apikeys) |
| `STRIPE_WEBHOOK_SECRET` | Stripe Dashboard → Webhooks → Add endpoint → get the signing secret |
| **Seed** | |
| `SUPER_ADMIN_EMAIL` | Your admin email |
| `SUPER_ADMIN_PASSWORD` | Your admin password |

---

## Deploying to Vercel

**Important:** Vercel is designed for serverless/frontend apps. This is an Express + Prisma backend, so you need a few adjustments:

### 1. Create `vercel.json`

```json
{
  "version": 2,
  "builds": [
    {
      "src": "src/server.ts",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "src/server.ts"
    }
  ]
}
```

### 2
```

