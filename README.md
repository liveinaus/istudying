# iStudying

NAPLAN-style Numeracy and Reading practice for Australian primary school kids, made for iPad (Safari or
added to the Home Screen).

- Each kid signs in by tapping their picture and typing a 4-digit PIN
- A parent makes practice sessions, tests and exams at each kid's level, with a time limit
- Wrong answers come back in later tests until they're right
- Step-by-step explanations, with optional AI help
- Print any test, with a separate answer sheet

## Run it

```sh
mkdir istudying && cd istudying
curl -O https://raw.githubusercontent.com/liveinaus/istudying/main/docker-compose.yml
echo "JWT_SECRET=$(openssl rand -hex 32)" > .env
docker compose up -d
```

Open `http://<server>:56622` and create the parent account. Data is kept in `./data`.

Images: `liveinaus/istudying:latest` (stable), `:beta`, `:dev`.
