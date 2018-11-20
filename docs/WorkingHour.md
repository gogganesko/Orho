# Описание класса WorkingHour
Класс для работы с распианием клиники

## Атрибуты

* Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")
* Day:DateTime
* ID:Int
* Procedures:List<[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")>
* TimeEnd:DateTime
* TimeStart:DateTime

## Описание атрибутов

* Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet") - кабинет.
* Day:DateTime - день.
* ID:Int - идентификатор в БД.
* Procedures:List<[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")> - список типов процедур.
* TimeEnd:DateTime - дата окончания.
* TimeStart:DateTime - дата начала.