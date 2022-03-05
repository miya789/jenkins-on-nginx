## メモ
- `--prefix` があるとアクセス先のURLが違った
  - それはそう

## 参考
- nginxのDocker化
    - https://www.engilaboo.com/nginx-docker-https/
- 複数のserviceで共有
    - https://h-piiice16.hatenablog.com/entry/2019/11/30/103843

古いものが残ったまま `docker-compose.yml` を書き換えた影響なのか，古いものが残ってしまったが，以下で削除できた
```bash
docker-compose down --rmi all
```

- rogu
  - https://www.lancard.com/blog/2016/09/05/docker%E3%81%AEjenkins%E3%82%B3%E3%83%B3%E3%83%86%E3%83%8A%E3%81%A7%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%83%AD%E3%82%B0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6%E6%82%A9%E3%82%93%E3%81%A7%E3%81%84/

cli
```bash
java -jar cli-2.319.1.jar -s https://nginx/jenkins/ -noCertificateCheck -auth admin:11ba5ed5d2cfa4259485df78818c9ec59c
```