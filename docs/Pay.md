# Описание класса Pay
Класс для работы с платежами клиники

## Атрибуты

* Date:DateTime
* ID:Int
* Patient:[Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient")
* Price:Float
* Procedure:[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")
* Worker:[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")

## Описание атрибутов

* Date:DateTime - дата платежа.
* ID:Int - идентификатор в БД.
* Patient:[Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient") - пациент.
* Price:Float - сумма.
* Procedure:[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure") - процедура.
* Worker:[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker") - врач.