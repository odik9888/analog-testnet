# View gets queried by SDK

## Зависимости

Для работы потребуется установить [Docker](https://docs.docker.com/engine/install/)

## Подготовка окружения

Копируем env файл и настраиваем окружение

```
cp .env-example .env
```

- **WALLET_SUBSTRATE_ADDRESS** адрес Substrate кошелька

- **WALLET_SEED** seed фраза данного кошелька

- **QUERY_HASH_ID** хеш вашего профинансированного представления. Найти можно в [профиле](https://watch.testnet.analog.one/#/profile) во вкладке **Funded Views**

- **QUERY_HASH_FIELD** поле которые хотим вывести. Найти можно в **Definition** представления

![plot](./img/view.png)

## Запуск

Запускаем всего один скрипт

```
✗ ./run.sh                           
20-alpine: Pulling from library/node
4abcf2066143: Pull complete 
d1e2f2d8a178: Pull complete 
3badf7a80ed4: Pull complete 
a0bb3a80cd3b: Pull complete 
Digest: sha256:fac6f741d51194c175c517f66bc3125588313327ad7e0ecd673e161e4fa807f3
Status: Downloaded newer image for node:20-alpine
docker.io/library/node:20-alpine

added 36 packages, and audited 37 packages in 4s

4 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
npm notice 
npm notice New minor version of npm available! 10.5.2 -> 10.7.0
npm notice Changelog: https://github.com/npm/cli/releases/tag/v10.7.0
npm notice Run npm install -g npm@10.7.0 to update!
npm notice 
The SESSION_KEY has been updated successfully.
The .apikeys file has been created successfully.
[]
[]
[]
[]
[]
```