# Jupyter

*Читайте об этом на других языках: [English](README.md), [Español](README.es-ES.md), [Português](README.pt-BR.md)*

Метапакет Jupyter для установки и документации.

## Запуск документации локально
Сперва перейдите в каталог `/docs` и создайте среду `conda`:

```bash
conda env create -f environment.yml  
```  

Активируйте среду:

```bash
source activate jupyter_docs  
```

Создайте документацию:

```bash
make clean  
make html
```

Документация будет создана в `build/html`. Её можно посмотреть открыв `build/html/index.html` или запустив HTTP-сервер и перейдя по адресу `0.0.0.0:8000` в Вашем веб-браузере.

```bash
python3 -m http.server
```
