Запуск скрипта в каталогах с инвентарями клиентов, либо из корня ./admin-tools/ либо в одном клиенте, ./admin-tools/client. При наличии файла requirements.yml, выдает теги прописанные в конфиге и на удаленном сервере.

```
cd ~
wget https://raw.githubusercontent.com/integral0/check_requirements/main/reqs-check
chmod a+x check_requirements
[[ -r /usr/local/bin/ && -w /usr/local/bin/ && -x /usr/local/bin/ ]] && mv reqs-check /usr/local/bin/ || { [[ ! -d ${HOME}/.local/bin ]] && mkdir -p ${HOME}/.local/bin; mv reqs-check ${HOME}/.local/bin/; }
