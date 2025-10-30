# Job Portal - Fullstack (HTML/CSS/JS + Node/Express + MySQL)

## What's included
- `backend/` - Express server (server.js), package.json, db.sql
- `public/` - Static frontend (index.html, style.css, script.js)
- Sample data: server will insert a demo employer, demo seeker and a couple of jobs on first run.

## Quick start (local)
1. Ensure MySQL is installed and running.
2. Create database (optional) or let server create tables:
   - You can run `backend/db.sql` to create the `job_portal` database, or set `DB_NAME` env var.
3. From the `backend/` folder:
   ```bash
   npm install
   DB_HOST=localhost DB_USER=root DB_PASS=admin123 DB_NAME=job_portal JWT_SECRET=change_this node server.js
   ```
4. Open `http://localhost:3000` in browser.

## Demo accounts
- Admin: admin@jobportal.com / admin123
- Employer: employer@demo.com / password
- Seeker: seeker@demo.com / password

## Notes
- This is a minimal starter. Move secrets to env vars for production.
- For uploads in production, use S3 or similar.
- Add validation, rate limiting, and HTTPS for production.

