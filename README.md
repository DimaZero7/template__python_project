# project_name

short project description

## Оглавление
1) [Установка](README.md#установка)
2) [Запуск на GPU](README.md#запуск-на-gpu)

## Установка
[Ссылка на документациюъ](./docs/ru/index.md#установка)



## Запуск на GPU

Чтобы запустить нейросеть на GPU, необходимо выполнить следующие шаги:

1) Создать контейнер в Docker, используя следующую команду:
```bash
docker run -it --gpus all -v absolute_path/src:/app/ --name container_name tensorflow/tensorflow:latest-gpu
```

2) Войти в контейнер:
```bash
docker exec -it container_name bash
```

3) Перейти в директорию `app`:
```bash
cd app
```

4) Установить все необходимые пакеты с помощью `pip`:
```bash
pip install package_name
```

5) Запустить обучение или выполнение нейронной сети. Она будет выполнена на GPU.
