# Linux_OS20.04_V4_X64_By_Griggorii.iso_ubuntu_focal_fossa-linux-image-kernel-5.9.3
iso , RELEASE , X64 , ubuntu , wayland , fast run , fast perfomance wayland , idlepython 3.8.5 my build , python3.8.5 

Распространяется с mit лицензией ввиду того что содержит пропирти вещи такие как zfs , nvidia и другое ПО.

# ISO DOWNLOAD: https://yadi.sk/d/8hTcz7FdkDiB3Q

Proview desktop: https://youtu.be/9B-nTJyEZX0

Переключение языка виртуальной клавиатуры при входе в gdm3 win-super+space вообщем теперь можете пароль перебить на любой язык хоть на русский и менять вин + пробел раскладку для набора пароля даже на русском.

Установку делайте пока без efi раздела дело в том что туда за место специалистов забрались те кто не понимает как он устроен там должен быть grub который называется ubuntu по адресу /efi/EFI/ubuntu и в него сложены текстовый груб-grub.cfg и grubx64.efi , а кто то сделал что теперь папка называется не ubuntu со всем содержимым , а grub какая то воина дистрибутивов лишь бы загрузочную часть не назвать ubuntu.

Monitor убрать авторосположение иконок:https://www.youtube.com/watch?v=J7HbQ246W7s

Сессия wayland работает на ноутбуках nvidia optimus , на стационарных придётся удалять иксовую энвидия что бы nouveau драйвер подхватил wayland.
Если устроиство слабое смените тему на любую которая легче и все залетает даже на планшете.

NVD7 это GF117M на свободном xorg-nouveau драйвере при этом надо удалить все драйвера от bumblebee , prime так же относится к этому источнику https://github.com/Griggorii/libdrm-2.4.101-source версию как я всё время говорю можно делать выше но это будет оферой типа смотрите 2.5.150.000 по этому я предлагаю драиверо писателям остановиться на этом варианте и  точка -> возможно это ускорение флаг в груб типа HW-true или HW-1 и проверить вдруг это заработает.

Так же есть ядро где nvidia точно опробована из этого видео если она не заработает на ядре 5.9.3 которое я собрал , тут все почти пересобрано. https://github.com/Griggorii/linux-image-oem-5.6.0-1020-kernel-ubuntu-x86_64-deb-package это ядро я забраковал оно тяжелее чем 5.9.3 с моим настроенным конфигом.

В остальном же если кто заметит этот дистрибутив почти пересобран сам на себе в некоторых частях так что я хочу сразу предупредить слишком шибко умных патреонщиков которые любят получать донаты за чужие труды переделывая всё под другие патченные де или кому удалось выбить лицензию на продажу дистрибутивов , что этот дистрибутив уже отдельная ветка и при обновлении будут происходит эпики на данный момент я поработал над llvm-10 очень много уходит времени на пере модифицирование бинарников если не сложением определённых реп папок , то модифицирование сначала компилятора и им уже самого бинарника всё это золотое время и тратить его надо как показано качеством в этом дистрибутиве , а не наращивание армии бездельников ит понятно тем бы с их тдрипперми проводить и проводить эксперементы , но я понял у нех нету некого динамическо логического мышления иначе бы не я видео драивер так у паковал в один пак , а они при чём уже как года два назад , возможно даже из него можно будет вытащить скоро системд не потому что тот плохой , а потому что чем больше сервисов загружается тем меньшая скорость загрузки и мы заходим в тупик из которого не вышли ведь хромиум ос загружается на hdd за мгновение , при чем на hdd. На ssd всё загружается очень быстро.

Дистрибутив нацелен на кино производителей и саунд дизайнеров поскольку имеет самые качественные компоненты видеодрайвера что дает не реально хорошее качество изображения и звука , кому надо игры есть стим , литрус и много другого в репозиториях достаточно открыть synaptic и поставить. В /lib64 созданна ссылка на libcuda.so для давинчи редактора. 

Этот дистрибутив делается очень сложно так что больше его распространяйте и чем больше узнает что такое качество и тогда может другие страны отправят инвестиции и вообще зар платы за мой ручной труд и перестроение дистрибутива. На данный момент могу только сказать что если вы будете компилировать компилятор LLVM то делйте свап раздел с памятью на 50 Гигабайт и именно у этого дистрибутива очень хорошее связка с виртуальной и динамической памятью и он справится с компиляцией , другие дистрибутивы могут не поддерживать качественно swap память что и характерезирует наивысшее качество моего дистрибутива. Что бы поддерживать дистрибутив надо хотя бы миллионов 50 что бы нанимать людей рубящих в теме , например есть идея перекомпилировать всю убунту или какие то её части через не через gcc , а через javac и получить дистрибутив у которого все бинарники будут нативными и если даже изменится glib и ldd то такой дистрибутив продолжит работу , но не в этом идея конечно потом на другой глиб менять ничего не надо будет потому что с наличием денег этот дистрибутив поидет отдельно от каноникал и других фирм называться будет типа jubuntu или еще как то далее придумаем сообщаясь со всеми специалистами которых найму. Конечно кода мидлииарды строк и по этому ни какую распильную астра не имеет смысла строить. Так же есть электронный кошелек для биткоина туда могут кидать как просто благодарные люди и разработчики анонимно , так же могут кидать те кому стыдно что они работая в компаниях типа амазон , каноникал , гугл , яндекс и других компаний имеют дистрибутив созданные ихними сотрудниками получая миллионы нефти на порядки хуже либо с отсутствующими фичами типа быстрой настройки dconf единого профиля браузера с иконкой gaia на кошелек ниже:

Griggorii@gmail.com только настоящие технологии bitcoin support real technology new fix 1Fps612daCcb7vYN2bFDRoDuUnrjJESDmk

Nvidia autoconfig run support notebook optimus , nvidia all laptop desktop support nvidia autoconfig , not recommended generate xorg file nvidia auto onli

Данный дистрибутив использует пакет собранных мной дрйверов https://github.com/Griggorii/mesa-20.1.5_v3_ubuntu-19.04-20.04-20.10_X86_64_graphics в получения именно такого ядра так же поучаствовали своего рода инклюдами для новго ядра благодаря чему ядро собралось именно под эти видео драйвера и не будет конфликтовать если не делать резких движении с хорг конфигами , а точнее вообще их не делать так же перебилдены такие пакеты как glib посколько надо что бы он обернул драйвера для лучшей работо способности https://github.com/Griggorii/glibc-2.31_all.deb_package_version_gcc-10-full_ubuntu_20.04_focal_fossa перебилденный pulseaudio https://github.com/Griggorii/pulseaudio_13.99.1-1ubuntu3.5-ubuntu-focal-20.04 gdm3 https://github.com/Griggorii/gdm3_3.34.1-1ubuntu1-run-keyboard-test-deb-package busybox https://github.com/Griggorii/busybox-1.30.1-deb-package-ubuntu-20.04-ubuntu-20.10 частично добавленны некоторые библиотеки из так же перебилденного llvm-10 на более старой системе 16.04 где на борту был ещё только python3.5 https://github.com/Griggorii/llvm-10-tools где ранее на нём же была опробована сразу же сборка предоставляемых в тарболе драйверов mesa. Все клавиши переназначены допустим снимок экрана shift+f7 , shift+f6 настройки , посмотреть переназначения в терминале: gnome-control-center keyboard , был получен c сверх тяжелого перебилда новый python3.8.5 https://github.com/Griggorii/python3.8.5_ubuntu_20.04_new_rebuild_amd64.deb теперь он идет в поставке.




