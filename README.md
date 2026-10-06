# Hi, I'm Muhammed 👋

I'm a backend-focused software engineer based in Nigeria, currently looking for a **graduate software engineering
role**.
I like building services that keep working when traffic grows. That means caching, background workers,
schema migrations, tests and CI, not only the endpoints.


## 🔨 Featured projects

### [URL Shortener with Analytics](https://github.com/moh-oppa/Url_Shortener)
**Python · FastAPI · PostgreSQL · Redis · Docker · GitHub Actions**

A production-style link shortener with click analytics, built for a fast redirect path.
- Redirects are served from a **Redis read-through cache**, with negative caching for unknown codes.
- Click tracking is moved off the request path. Clicks go into a **Redis Stream**, and a separate **cons
umer-group worker** batch-writes them to Postgres. Stuck messages are reclaimed with `XAUTOCLAIM`.
- Stats come from a **pre-aggregated daily rollup table** (built with upserts), so the stats endpoint do
esn't slow down as raw events pile up.
- **66 tests** cover the API, cache, worker and GeoIP. CI runs lint, tests against real Postgres and Red
is, a migration round-trip, and a Docker image smoke test.

### [BuddyAI: chat with your documents](https://github.com/moh-oppa/Buddy_ai)
**Python · FastAPI · PostgreSQL · LLM (Ollama API) · React**

Upload a PDF, DOCX or TXT file, then get a summary, ask questions about it, or extract
people, dates and figures as structured JSON. Endpoints are rate-limited per IP.

### [SQL data cleaning](https://github.com/moh-oppa/sqlexploration)
**SQL**

Scripts that clean real-world datasets (Superstore, BMW), plus practice with CTEs, temp tables,
window-style subqueries, stored procedures and string functions.

## 🧰 Tech I use

**Languages:** Python, SQL, JavaScript
**Backend:** FastAPI, SQLAlchemy (async), Pydantic, Alembic
**Data and infrastructure:** PostgreSQL, Redis (caching, Streams), Docker, Docker Compose
**Quality:** pytest, Ruff, GitHub Actions CI

## 📈 Also on here
- [leetcodeex](https://github.com/moh-oppa/leetcodeex): data structures and algorithms practice
- [mini_projects](https://github.com/moh-oppa/mini_projects): small Python programs from when I was lear
ning

## 📫 Contact
- Email: fasholakorede01@example.com
- Phone Number: +2348080990442
