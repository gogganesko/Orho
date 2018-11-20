# Описание класса Procedure
Класс для работы с процедурами клиники

## Атрибуты

* DateFact:DateTime
* DateStart:DateTime
* DateEnd:DateTime
* Description:String
* EventDate:DateTime
* ID:Int
* IsMine:Bool
* KindOfProcedure:[KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")
* Name:String
* TypeOfProcedure:[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")

## Описание атрибутов

* DateFact:DateTime - фактическая дата процедуры.
* DateStart:DateTime - дата начала процедуры.
* DateEnd:DateTime - дата окончания процедуры.
* Description:String - описание.
* EventDate:DateTime - дата события.
* ID:Int - идентификатор в БД.
* IsMine:Bool - флаг принадлежности процедуры к клинике.
* KindOfProcedure:[KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure") - вид процедуры.
* Name:String - название процедуры.
* TypeOfProcedure:[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure") - тип процедуры.