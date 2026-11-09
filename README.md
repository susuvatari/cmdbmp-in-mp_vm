```
AUTO-ATTRIBS-CMDBMP/
├── .env.example                # Шаблон конфигурации и секретов
├── .gitignore                  # Исключения для git (секреты, venv, логи)
├── .gitlab-ci.yml              # Пайплайн автодеплоя через rsync + SSH
├── requirements.txt            # Зависимости Python
├── main.py                     # Главный скрипт-оркестратор (запуск по cron)
├── README.md                   # Документация проекта
├── api_mp_vm/
│   ├── __init__.py
│   ├── asset_processor.py      # Выгрузка хостов из MP и импорт CSV пакетно
│   ├── get_pdql_token.py       # Генерация токенов для выполнения PDQL-выборок
│   ├── group_manager.py        # Валидация и создание динамических групп по API
│   ├── mp_vm_variables.py      # Инфраструктурные переменные MaxPatrol
│   └── vm_authentication.py    # Модуль OAuth2-авторизации в MaxPatrol
└── cmdb_jira/
    ├── __init__.py
    └── jira_extractor.py       # Извлечение reference и select полей Jira Insight
```
