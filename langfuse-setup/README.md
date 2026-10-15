# Langfuse setup

Runs Langfuse v4 locally for the Langfuse lab.

- `docker-compose.yml` is the official Langfuse v4 compose file.
- `.env` holds lab-only secrets for the containers. It creates no users or projects.

```bash
docker compose up -d
```

Open http://localhost:3000, sign up, then create an organization, a project and API keys.
The full steps are in the Langfuse lab guide, online at https://kodelumi.com/w/AVWkaKxQo3zaT28p.
Start with `getting-started-with-langfuse.md`, then `lab-00-overview.md` and the step files.
