# Knowledge Base

TDB

## Running

Just run:

```bash
$ docker-compose up
```


## Commands

Running gulp to have livereload on templates and frontend files:

```bash
$ docker exec -it knowledgebase_web_1 gulp
```

To run any command on the app container you can do:

```bash
$ docker exec -it knowledgebase_web_1 python manage.py createsuperuser
$ docker exec -it knowledgebase_web_1 python manage.py shell_plus
$ docker exec -it knowledgebase_web_1 python manage.py test --failfast
$ docker exec -it knowledgebase_web_1 bash
```

## Upgrade packages

To upgrade packages version run:

```bash
$ docker exec -it knowledgebase_web_1 piprot --latest --verbatim
```
