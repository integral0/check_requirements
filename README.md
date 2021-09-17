Запуск скрипта в каталогах с инвентарями клиентов ./admin-tools/client. При наилчии файла requirements.yml, выдает теги прописанные в конфиге и на удаленном сервере.


```
cd ~
wget https://raw.githubusercontent.com/integral0/check_requirements/main/check_requirements
chmod a+x check_requirements
[[ -r /usr/local/bin/ && -w /usr/local/bin/ && -x /usr/local/bin/ ]] && mv check_requirements /usr/local/bin/ || { [[ ! -d ${HOME}/.local/bin ]] && mkdir -p ${HOME}/.local/bin; mv check_requirements ${HOME}/.local/bin/; }

