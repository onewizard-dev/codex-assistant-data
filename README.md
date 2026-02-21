# Codex Assistant Data

Хранилище данных для приложения Codex Assistant.

## Структура

/  
├── laws/                  # Законы для серверов (new-york-1.json, los-angeles-7.json, ...)  
├── rules/                 # Правила (general.json, events.json, organizations.json)  
├── repo_structure.json    # Список всех доступных файлов  
└── banner.json            # Конфигурация баннера  

## Форматы данных

### Законы (/laws/*.json)  
{  
  "updatedAt": 1734444000000,  
  "data": {  
    "UK": {  
      "url": "https://forum.majestic-rp.ru/...",  
      "articles": [  
        {  
          "code": "6.9",  
          "title": "Название статьи",  
          "text": "Текст статьи",  
          "penalty": "Наказание"  
        }  
      ]  
    }  
  }  
}  

### Правила (/rules/*.json)  
{  
  "updatedAt": 1734444000000,  
  "data": {  
    "main-rules": {  
      "articles": [  
        {  
          "code": "1.1",  
          "title": "Название",  
          "note": "Примечание",  
          "explanation": "Пояснение",  
          "exception": "Исключения",  
          "penalty": "Наказание"  
        }  
      ]  
    }  
  }  
}  

### repo_structure.json  
{  
  "laws": { "files": ["new-york-1.json", "los-angeles-7.json"] },  
  "rules": { "files": ["general.json", "events.json", "organizations.json"] },  
  "lastUpdate": 1734444000000  
}  

### banner.json  
{  
  "enabled": true,  
  "imageUrl": "https://...",  
  "linkUrl": "https://..."  
}