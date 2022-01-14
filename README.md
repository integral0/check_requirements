### Описание 
При наличии файла requirements.yml, выдает теги прописанные в файле и последний в удаленном репозитории.
Запускать скрипт можно либо из корня ./admin-tools/, либо в инвентаре клиента ./admin-tools/client
### Установка 
```
cd ~
wget https://raw.githubusercontent.com/integral0/check_requirements/main/reqs-check
chmod a+x reqs-check
[[ -r /usr/local/bin/ && -w /usr/local/bin/ && -x /usr/local/bin/ ]] && mv reqs-check /usr/local/bin/ || { [[ ! -d ${HOME}/.local/bin ]] && mkdir -p ${HOME}/.local/bin; mv reqs-check ${HOME}/.local/bin/; }
```
### Использование
```
$ reqs-check -h
Check tags in file requirements.yml

Usage: reqs-check [OPTIONS]
OPTIONS:
-h | --help:        Show this help screen
-d | --diff-only:   Show only different tags
   | --clear-cache: Clear cache repo before check




```
