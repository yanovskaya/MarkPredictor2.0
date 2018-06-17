[![Platform](https://img.shields.io/badge/platform-iOS-green.svg)]()
[![Swift 4.1](https://img.shields.io/badge/Swift-4.1-orange.svg)](https://swift.org)
# Mark Predictor 2.0
Ранее был опубликован проект **[Mark Predictor](https://github.com/yanovskaya/MarkPredictor)**, в котором обучение модели происходило на языке Python с помощью фреймворка Keras.

Однако на **[703 сессии WWDC](https://developer.apple.com/videos/play/wwdc2018/703/)** был представлен фреймворк **[CreateML](https://developer.apple.com/documentation/create_ml)**, позволяющий обучить модель прямо в playground. Именно с помощью CreateML и происходило обучение модели для **Mark Predictor 2.0**.

## 🔧 Что нужно, чтобы установить проект
В терминале в корне проекта введите следующую команду:
`pod install`. 
<br />

Для работы с playground должен быть установлен **Xcode 10**.

## ⚖ Keras vs CreateML
Сравним модели в **[Mark Predictor](https://github.com/yanovskaya/MarkPredictor)** и **MarkPredictor 2.0**.

|                          |      Keras      |            CreateML           |
|:------------------------:|:---------------:|:-----------------------------:|
|          **Размер**          |      214 KB     |              3 KB             |
|            **Тип**           | Neural networks |       Pipeline Regressor      |
| **Скорость создания модели** |     Быстрый     | Медленный  (из-за playground) |
|         **Точность**         |   Менее точный  |          Более точный         |
