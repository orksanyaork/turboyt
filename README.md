# Ремонт серверов Google не выходя из дома ~~не привлекая внимания санитаров~~
## Начальная настройка
1. В хромиум-браузере переходим по ссылке `chrome://flags/#enable-tls13-kyber` и выставляем значение **Disabled**
2. Откатываем п. 1 и п. 3 из предыдущей инструкции (спойлер `Устаревшее` ниже)
3. Скачиваем [последнюю версию GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI/releases)
4. Распаковываем в любое место на компьютере

## Автозагрузка при старте ОС (рекомендуется)
Из распакованной папки запускаем с правами администратора `service_install_russia_blacklist_dnsredir.cmd` и нажимаем любую клавишу. После этого проверяем, что в диспетчере задач есть процесс `goodbyedpi.exe` даже после перезагрузки ПК

## Ручной запуск
Из распакованной папки запускаем с правами администратора `1_russia_blacklist_dnsredir.cmd`. В открывшейся командной строке в конце должна быть фраза `Filter activated, GoodbyeDPI is now running!`
Если хотим сломать сервера Google, то закрываем окно командной строки

Протестированно на версии `goodbyedpi-0.2.3rc1` 01.08.2024

##
<details>
  <summary>Устаревшее</summary>
  
## Начальная настройка
1. В хромиум-браузере переходим по ссылке `chrome://flags/#enable-quic` и выставляем значение **Disabled**
2. Тоже самое делаем для `chrome://flags/#enable-tls13-kyber`
3. В настройках `chrome://settings/security` включаем `Использовать безопасный DNS-сервер` и в пункте `Выбрать поставщика услуг DNS` выбираем `OpenDNS` (возможно, этот пункт не обязателен)
4. Скачиваем [последнюю версию GoodbyeDPI](https://github.com/ValdikSS/GoodbyeDPI/releases)
5. Распаковываем в любое место на компьютере
6. Скачиваем файлы из этого репозитория в распакованную папку

## Автозагрузка при старте ОС (рекомендуется)
Из распакованной папки запускаем с правами администратора `!yt_service.cmd` и нажимаем любую клавишу. После этого проверяем, что в диспетчере задач есть процесс `goodbyedpi.exe` даже после перезагрузки ПК

## Ручной запуск
Из распакованной папки запускаем с правами администратора `!valdikss.cmd` или `!youtube.cmd`. В открывшейся командной строке в конце должна быть фраза `Filter activated, GoodbyeDPI is now running!`
Если хотим сломать сервера Google, то закрываем окно командной строки

Протестированно на версии `goodbyedpi-0.2.2` 27.07.2024
</details>
