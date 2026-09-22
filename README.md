<!-- Плеер будет создан с задержкой, после того как загрузятся все ресурсы на странице. Для этого используется событие `DOMContentLoaded`. Благодаря этой особенности можно вызывать функцию `createPlayer` раньше, чем загрузятся все необходимые библиотеки: jQuery и Playable.
 -->

# Видеоплеер

Учебный проект: верстка видеоплеера.

**Опубликованная версия:** [GitHub Pages](https://igorvinogradov1.github.io/lesson_django_01/)
**Репозиторий:** [GitHub](https://github.com/IgorVinogradov1/lesson_django_01)
**Курс:** [Девман — Верстаем онлайн-библиотеку](https://dvmn.org/modules/django-layout/lesson/player-layout/)

Построен на базе библиотеки [Playable](https://wix.github.io/playable/).

---

## Что это?

Видеоплеер с минимальным набором кнопок (play, volume, fullscreen):

<img width="600" height="448" alt="Скриншот плеера" src="https://gist.github.com/user-attachments/assets/4fcbaa6e-9752-4dc8-9528-c4d6dc2fe9d6" />

Этот код добавит на страницу плеер, который играет видео по [этой ссылке](https://dvmn.org/media/filer_public/78/db/78db3456-3fd3-4504-9ed9-d2d1fd843c0b/highest_peak.mp4).

Если хочется выбрать другое видео, с помощью аргумента `src` плееру можно указать какое видео проигрывать, ссылки обязаны заканчиваться расширением файла:

```html
<script type="text/javascript">
  createPlayer({
    elementId: 'player',
    src: 'https://dvmn.org/media/filer_public/d0/16/d016d9b8-4180-4bb9-ad83-0241f61627b8/samsung_demo_-_alive_in_color.mp4'
});
</script>
```

---

## Как использовать

### Скачать репозиторий

1. Перейдите на репозиторий: [GitHub](https://github.com/IgorVinogradov1/lesson_django_01)
2. Нажмите **`Code`** → **`Download ZIP`**.
3. Распакуйте.
4. Откройте `index1.html` в браузере.

---

### Посмотреть опубликованную версию

1. Перейдите на сайт: [GitHub Pages](https://igorvinogradov1.github.io/lesson_django_01/)
2. Покликайте кнопки, проверьте работу.

---

### Развернуть локально

1. Скачать репозиторий:
```
git clone https://github.com/IgorVinogradov1/lesson_django_01
cd lesson_django_01
```

2. Подключите livereload:
```
livereload .
```

3. Открыть в браузере: `http://127.0.0.1:35729/`