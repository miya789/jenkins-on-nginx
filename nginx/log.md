古いものが残ったまま `docker-compose.yml` を書き換えた影響なのか，古いものが残ってしまったが，以下で削除できた
```bash
docker-compose down --rmi all
```