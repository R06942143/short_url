# URL Shortener with FastAPI

[https://github.com/tiangolo/fastapi](https://github.com/tiangolo/fastapi)

```sh
$ git clone https://github.com/vancanhuit/url-shortener.git
$ cd url-shortener
$ docker-compose up -d --build
$ docker-compose exec api alembic upgrade head
```

Using [curl](https://curl.haxx.se):

```sh
$ curl -X POST -d '{"url": "https://google.com"}' -H "Content-Type: application/json" http://localhost:8000/api/shorten | jq .
{
  "short_link": "YiK5mlk"
}
```
