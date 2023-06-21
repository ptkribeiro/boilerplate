# Snipe-it Docker Compose Setup

This repo has all the necessary configurations to run a snipe-it container.

In order to work, you will have to rename `config/dotenv` to **.env** and move in to the root folder.

---
## API Key

The first time you launch the container, you will run this two commands:

```
docker exec -it your-snipe-it-container-name sh
```

```
php artisan key:generate --show
```

Then copy the **base64** key and replace on your **.env** file and restart the container:

`{{INSERT_API_TOKEN}}`