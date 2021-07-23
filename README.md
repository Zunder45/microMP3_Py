# MicroSortingFileMP3_Py

## О пограмме
___MicroSortingFileMP3___ была разаботана для автоматизированного сортирования (по имени исполнителя) аудио файлов формата mp3. 

Есть две версии UI: 
- [Консольная](#cl);

![console](img/console.png)

- [Графическая](#gr).

![gui](img/gui.png)



***
## Установа 

1. Устанавливаем [python](https://www.python.org/).

2.  Устанвливаем pip.

- Ubuntu:

```sh
sudo apt install pip
```

- Arch:

```sh
pacman -S python-pip
```



3.  Устанавливаем нужные для работоспосоробности библеотеки.

```sh
pip install pysimplegui
pip install colorama
pip install eyed3
pip install argparse
``` 

4. Ставим tkinter
- Ubuntu:

```sh
sudo apt-get install python3-tk
```

- Arch:

```sh
sudo pacman -S tk
```


5. Скачиваним с  репозитория github файлы программы.

``` sh
git clone https://github.com/Zunder45/MicroSortingFileMP3_Py.git 
```

Переходим в директорию программы

```sh
cd MicroSortingFileMP3_Py 
```

## Запуск

Запуск происходит через файл Main.py (графика и консоль) или Console version/Main.py (без зависимостей к tkinter и pysimplegui).


<p id="cl">Запуск консольной версии:</p>

```sh
python3 Main.py 
```

<p id="gr">Запуск графической версии:</p>

```sh
python3 Main.py -g   
```

***
## Аргументы

Сортировка файлов происходи в рабочем каталоге (там откуда запущена программа) или с помощью аргумента **-p** можно указать точное местоположение каталога.

```sh
python3 Main.py -p *Путь*
```

Аргумент **-f** (доступный только в *Console version*) принимает в себя путь, того кталога от куда будут браться файлы для перемещения в каталог программы или указаный аргументом **-p**.

```sh
python3 Main.py -f *Путь к файлам* -p *Путь куда будут перемещены и сортированы файлы*
```

Если добавть **-p** к **-g**, то путь указанный в консоле будет указан в поле ввода пути к каталогу.

```sh
python3 Main.py -gp *Путь*
```

## Остальные аргументы

|Аргумент|Описание|
|:--------:|--------|
|**-u** (доступный только в *Console version*) | Брать файлы без имени исполнителя (они будут перемещены в каталог       "Неизвестный исполнитель")|
|**-s** (доступный только в *Console version*) | Пропускает запрос о продолжении|



