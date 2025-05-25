# Scripts
Скрипты автоматизации для повседневности
**Remind**  
Скрипт работает с утилитой dunst, поэтому для работы скрипта он должен быть установлен
```sh
echo y | sudo pacman -Syu dunst
```

Можно добавить выполнение скрипта в конфиг оболочки
```sh
python3 /home/$USER/Scripts/remind
```
Способы передачи параметров:
- Можно передать в кавычках(в конфиге оболочки)
```sh
python3 /home/$USER/Scripts/remind "8:00" "9:00"
```
- Без кавычек(в конфиге оболочки)
```sh
python3 /home/$USER/Scripts/remind 8:00 9:00
```
- Можно передать в основную функцию в скрипт python3 */home/$USER/Scripts/remind*
```sh
Remind(min_time="8:00", max_time="9:00")
```
