# Oracle JFo 9 Practice

---

Для запуска нужна [Oracle jdk-9](https://www.oracle.com/java/technologies/javase/javase9-archive-downloads.html)

---

Задание описано в файле JFo_9_Practice.pdf

---

В файлах dorm`i`Config.properties описаны параметры квадрата, которым будет изображено общежитие.

```
name=11 dorm // Название общежития
x=251 // Координаты
y=683 
colorBlue=1.0 // Цвет, задается как RGB
colorRed=1.0
colorGreen=0.0
population=136 // Размер квадрата
```

`Dorm` - класс с описанием общежития

`CenterPoint` - класс с методами для высчитывания центральных точек `All Dorms` и `Study Group`. Список общежитий для них задается в
класс `FindingCentralLocation` следующим образом:

```
 new CenterPoint("All Dorms", true, dorms);
 new CenterPoint("Study Group", false, dorms[0], dorms[2], dorms[3]);
```

`PopulationChanger` - класс с описанием скролл бара для изменения размера квадрата на карте

`FindingCentralLocation` - класс с основной логикой приложения (отрисовка полигонов, карты, фиксирование координат в .properties файлах)

Картинки с картами лежат по пути `src\FindingCentralLocation\Images\`.
Задать другую картинку можно в конфиге `stageConfigFile.properties` - `dormTitle`


