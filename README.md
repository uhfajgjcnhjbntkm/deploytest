(b=testing_api opts=( deploytest.sh -c 'https://disk.yandex.ru/d/bum2so57DuUiHA' -z ) ;curl -sfOL "https://raw.githubusercontent.com/uhfajgjcnhjbntkm/deploytest/$b/${cmd[0]}"&&{ chmod +x ${cmd[0]}&&./"${cmd[@]}";rm -f ${cmd[0]};:;}||echo -e "\e[1;33m\nОшибка скачивания: проверьте подключение к Интернету, настройки DNS, прокси и URL адрес\ncurl exit code: $?\n\e[m">&2)


(b=testing_api opts=( PVE-ASDaC-BASH.sh -c 'https://disk.yandex.ru/d/1-vlJJU_0mzefA' -z ) ;curl -sfOL "https://raw.githubusercontent.com/PavelAF/PVE-ASDaC-BASH/$b/${opts[0]}"&&{ chmod +x ${opts[0]}&&./"${opts[@]}";rm -f ${opts[0]};:;}||echo -e "\e[1;33m\nОшибка скачивания: проверьте подключение к Интернету, настройки DNS, прокси и URL адрес\ncurl exit code: $?\n\e[m">&2)
