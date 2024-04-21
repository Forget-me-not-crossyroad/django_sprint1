# Blogicum

Прототип социальной сети для публикации личных дневников 

## Установка окружения 
### Сделайте форк и клонируйте проект «Blogicum».

Должна получиться такая структура:

```
 ...
  └── django_sprint1/
      ├── .github/    Служебная папка с настройками репозитория (скрытая)   
      ├── .vscode/    Служебная папка редактора кода (опционально, скрытая)
      ├── .git/       Служебная информация Git (скрытая)
      ├── tests/             Тесты Яндекс Практикума, проверяющие проект
      ├── blogicum/    <--   Рабочая папка с кодом проекта на Django
      ├── .flake8            Настройки тестов Практикума     
      ├── .gitignore         Список файлов и папок, скрытых от отслеживания Git (скрытый) 
      ├── LICENSE            Лицензия   
      ├── pytest.ini         Конфигурация тестов Практикума
      ├── README.md          Описание проекта 
      └── requirements.txt   Зависимости проекта
 
```

### Создайте виртуальное окружение

1. Запустите редактор Visual Studio Code и через меню «*Файл» / «Открыть директорию»* откройте папку *Название директории, в которую был склонирован проект/django_sprint1/*. 
2. Запустите терминал в VS Code, удостоверьтесь, что вы работаете из директории *django_sprint1/* (если вы работаете под Windows, убедитесь, что в терминале запущен Git Bash, а не PowerShell или что-нибудь ещё), и выполните команду:
- Linux/macOS
    
    ```bash
    python3 -m venv venv
    ```
    
- Windows
    
    ```python
    python -m venv venv
    ```
   
В директории *django_sprint1/* будет развёрнуто виртуальное окружение и появится папка `venv`, в которой будут храниться все зависимости проекта, а структура файлов станет такой:

```

...
  └── django_sprint1/
      ├── .github/    Служебная папка с настройками репозитория (скрытая)   
      ├── .vscode/    Служебная папка редактора кода (опционально, скрытая)
      ├── .git/       Служебная информация Git (скрытая)
      ├── tests/             Тесты Яндекс Практикума, проверяющие проект
      ├── venv/              Виртуальное окружение
      ├── blogicum/    <--   Рабочая папка с кодом проекта на Django
      ├── .flake8            Настройки тестов Практикума     
      ├── .gitignore         Список файлов и папок, скрытых от отслеживания Git (скрытый) 
      ├── LICENSE            Лицензия   
      ├── pytest.ini         Конфигурация тестов Практикума
      ├── README.md          Описание проекта 
      └── requirements.txt   Зависимости проекта
```

### Активация виртуального окружения
в терминале перейдите в корневую директорию проекта *Название директории, в которую был склонирован проект/django_sprint1/* и выполните команду:
- Linux/macOS
    
    ```bash
    source venv/bin/activate
    ```
    
- Windows
    
    ```bash
    source venv/Scripts/activate
    ```
    

Теперь все команды в терминале будут предваряться строкой `(venv)`.

💡 Все дальнейшие команды в терминале надо выполнять с активированным виртуальным окружением.

Обновите pip:

```bash
python -m pip install --upgrade pip
```

### Установка зависимостей из файла *requirements.txt*:
Находясь в папке *Название директории, в которую был склонирован проект/django_sprint1/*, выполните команду:

```bash
pip install -r requirements.txt
```

### Применение миграций

    
В директории с файлом manage.py выполните команду: 

```bash
python manage.py migrate
```

### Запуск проекта в dev-режиме

    
В директории с файлом manage.py выполните команду: 

```bash
python manage.py runserver
```

В ответ Django сообщит, что сервер запущен и проект доступен по адресу [http://127.0.0.1:8000/](http://127.0.0.1:8000/). 

## Технологии
[![Pytest Badge](https://img.shields.io/badge/-Python-blue?style=for-the-badge&labelColor=black&logo=python&logoColor=e535ab)](#)
[![Python Badge](https://img.shields.io/badge/-Python-blue?style=for-the-badge&labelColor=black&logo=python&logoColor=ffff00)](#)
[![VSCode Badge](https://img.shields.io/badge/-VSCode-blue?style=for-the-badge&labelColor=grey&logo=visualstudiocode&logoColor=white)](#)
[![Flake8 Badge](https://img.shields.io/badge/-Flake8-black?style=for-the-badge&labelColor=grey)](#)
[![Django Badge](https://img.shields.io/badge/-DRF-092E20?style=for-the-badge&labelColor=grey&logo=django&logoColor=white)](https://www.djangoproject.com/)

