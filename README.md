# web-page-demo

Для запуска веб-приложения, необходимо сначала проинициализировать sqlite3 БД с помощью команды

```bash
python3 init_db.py
```

Для компиляции protobuf файлов в класс Python необходимо воспользоваться командой:

```bash
python -m grpc_tools.protoc -I=proto --python_out=. --pyi_out=. --grpc_python_out=. proto/alert.proto
```

Для запуска самого-веб приложения необходимо написать:

```bash
python3 app.py
```

Или запустить с помощью `docker`:
```bash
sudo docker-compose up -d
```

После чего приложение будет доступно по адресу `localhost:5000`