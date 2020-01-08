# TinyBlog тема для Zola
Простая тема блога для генератора статических сайтов [Zola](https://github.com/getzola/zola).

![Как выглядит тема](screenshot.png "Как выглядит тема")

## Как установить

**1. Добавляем git модуль к вашему проекту**

В корне проекта создаем файл `.gitmodules` со следующим содержанием:

```
[submodule "themes/tinyblog"]
	path = themes/tinyblog
	url = git@github.com:lebe-dev/tinyblog-zola-theme.git
```

**2. Создаем под каталог для темы**

Для Windows:

```shell script
mkdir themes\tinyblog
```

Для Linux:

```shell script
mkdir -p themes/tinyblog
```

**3. Подгружаем тему**

```shell script
git submodule update --init --recursive
```

**4. Указываем тему в качестве основной**

```
theme = "tinyblog"
```

## RoadMap

**Версия 1.1.0**
- Страница "Об авторе"
  
- Рефакторинг Sass  
Большая часть Sass-кода взято из оригинальной темы Ergo. В коде слабо используются возможности Sass и есть много
избыточных конструкций. Также из-за особенностей организации scss-файлов их не переопределить без копирования
всех файлов.

## Благодарности

За основу TinyBlog темы была взята тема [Ergo](https://github.com/insipx/Ergo).
Спасибо [Andrew Plaza](https://github.com/insipx).
