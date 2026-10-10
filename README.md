# ComboStrap Environment for issues 134

Environment for [issues 134](https://github.com/combostrap/combo/issues/134)

How to start
```bash
git clone https://github.com/ComboStrap/site-starter-issues-134
cd site-starter-issues-134
docker run \
  --name site-starter-issues-134 \
  --rm \
  -p 8081:80 \
  --user 1000:1000 \
  -e DOKU_DOCKER_ENV=dev \
  -e DOKU_DOCKER_ACL_POLICY='public' \
  -e DOKU_DOCKER_ADMIN_NAME='admin' \
  -e DOKU_DOCKER_ADMIN_PASSWORD='welcome' \
  -v $PWD:/var/www/html \
  ghcr.io/combostrap/dokuwiki:php8.3-latest
```
The default ComboStrap site should be available at: http://localhost:8081 



