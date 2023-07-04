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
<img src="https://camo.githubusercontent.com/fb8731f93b7bc9ac1d530eac09d2e739be7248fd119a7a8e81d11514eafe5a49/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d5079746573742d6535333561623f7374796c653d666f722d7468652d6261646765266c6162656c436f6c6f723d626c61636b266c6f676f3d507974657374266c6f676f436f6c6f723d653533356162" alt="Pytest Badge" data-canonical-src="https://img.shields.io/badge/-Pytest-e535ab?style=for-the-badge&amp;labelColor=black&amp;logo=Pytest&amp;logoColor=e535ab" style="max-width: 100%;"> <img src="https://camo.githubusercontent.com/6f821a8c6c5575e343061f1d2720d6c13db74798bc715d7f6f9f26ab9b361c7e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d507974686f6e2d6666666630303f7374796c653d666f722d7468652d6261646765266c6162656c436f6c6f723d626c61636b266c6f676f3d507974686f6e266c6f676f436f6c6f723d666666663030" alt="Python Badge" data-canonical-src="https://img.shields.io/badge/-Python-ffff00?style=for-the-badge&amp;labelColor=black&amp;logo=Python&amp;logoColor=ffff00" style="max-width: 100%;"> [![VSCode Badge](https://img.shields.io/badge/-VSCode-blue?style=for-the-badge&labelColor=grey&logo=visualstudiocode&logoColor=white)](#) [![Flake8 Badge](https://img.shields.io/badge/-Flake8-black?style=for-the-badge&labelColor=grey)](#) [![Django Badge](https://img.shields.io/badge/-Django-092E20?style=for-the-badge&labelColor=grey&logo=django&logoColor=white)](https://www.djangoproject.com/) [![Bootstrap Badge](https://img.shields.io/badge/-Bootstrap5-7952b3?style=for-the-badge&labelColor=grey&logo=bootstrap&logoColor=white)](https://getbootstrap.com/docs/5.1/getting-started/introduction/#starter-template)

