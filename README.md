# felvidek-ru
Переводчик игры Felvidek.
Обрабатывает текстовые файлы движка RPG Maker из www/data.
Заточен под конкретную игру, при желании можно адаптировать к любой другой игре на этом движке.

# Использование

Скачать перевод из гуглдока в кэш:
```bash
./update_from_doc.py > translate_cache.json 
```

Перевести игру:
```bash
./translate.py --game-dir src_game --line-limit 300
```

Распечатать перевод из кэша для загрузки в гуглдок:
```bash
./print_translate_cache.py > doc.txt
```

Залить документы в облако
```bash
./upload_doc.py --file doc.txt
```
