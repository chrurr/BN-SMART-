# BN SMART

Web-based phone repair shop management system built with Node.js, Express and PostgreSQL.

## Run locally

```bash
npm install
```

Create `.env` from `.env.example`, then set a PostgreSQL `DATABASE_URL` and a strong `JWT_SECRET`.

```bash
npm start
```

Open `http://localhost:3000`.

## Render

The repository includes `render.yaml` for a Render Blueprint. It creates:
- Node web service
- PostgreSQL database
- `DATABASE_URL` from the database connection string
- generated `JWT_SECRET`
- `/health` health check

On first startup the application creates/updates the database schema automatically.

Default first login created by the application when the database is empty:
- Username: `admin`
- Password: `Admin@12345`

**Change the password immediately after first login.**
