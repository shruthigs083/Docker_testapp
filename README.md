# Docker_testapp

## Start MongoDB

Set a strong password before starting the services. In PowerShell:

```powershell
$env:MONGO_ROOT_PASSWORD = "choose-a-strong-password"
docker compose -f mongodb.yaml up -d
```

MongoDB is exposed on port `27018`, and Mongo Express is available on port `8082`.

## Build the app image

```powershell
docker build -t docker-testapp .
```