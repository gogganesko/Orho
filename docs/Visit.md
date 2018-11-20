# Описание класса Visit
Класс для работы с приёмами клиники

## Атрибуты

* Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")
* DateEnd:DateTime
* DateStart:DateTime
* Description:String
* ID:Int
* Patient: [Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient")
* Result:String
* Workers:List<[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")>

## Описание атрибутов

* Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet") - кабинет.
* DateEnd:DateTime - дата окончания приёма.
* DateStart:DateTime - дата начала приёма.
* Description:String - описание.
* ID:Int - идентификатор в БД.
* Patient: [Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient") - пациент.
* Result:String - результат приёма.
* Workers:List<[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")> - список врачей приёма.