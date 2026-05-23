# Arcane Docker Management UI

## Official Links

- [Website](https://getarcane.app/)
- [GitHub](https://github.com/getarcaneapp/arcane)
- [Documentation](https://getarcane.app/docs)

## Configure `.env`

Two different secrets are needed, one is the `ENCRYPTION_KEY` and the other is the `JWT_SECRET`. Both of these secrets can be generated using any one of the following commands:

- On Linux/MacOS:
```bash
openssl rand -hex 32 
```

- Using Python:
```bash
python -c "import secrets; print(secrets.token_urlsafe(32))"
```

Rename `.env.example` to `.env` and paste the generated secrets

## Post Deploy

- After Deploy, Arcane UI is available on `http://localhost:3552` or `http://<server-ip>:3552`

- Initial admin credentials are logged in the docker logs which can be accessed via `docker compose logs` (username: `arcane`, password: `arcane-adin`)

- Create an admin user from the settings page and delete the default admin user for increased security

