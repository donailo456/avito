# Avito

Задание от Avito

  Вас встречает главный экран, на котором показаны 30 позиций товаров, которые приходят из интернета. При нажатии на любой товар, появляется карточка позиции, в которой предствлена дополнительная информация

  - В проекте не были использованы посторонние библиотеки
  - Реализованы два экрана состояния - загрузки и ошибки
  - Отображение контента из JSON файла
  - Данные взяты из предоставленных URL-ссылок
  - Приложение написано на языке Swift.
  - Пользовательский интерфейс приложения реализован кодом без использования SwiftUI.
  - Для отображения списка используется UICollectionView с отображением в 2 столбца.
  - £Для запроса данных используется URLSession.

# Для запуска
  Для запуска проекта можно скачать исходный zip-файл или применить в Xcode Swift Package Manager

# Важно 

  Для показа состояние экрана при загрузке, в коде имеется задержка основного потока
  
```sh
DispatchQueue.main.asyncAfter(deadline: .now() + .milliseconds(500)) {
    ...
}
```

  Для показа состояния экрана ошибки, был использован AlertViewController, который сработает при ошибке
