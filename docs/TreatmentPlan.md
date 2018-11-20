# Описание класса TreatmentPlan
Класс для работы с планами лечения пациентов

## Атрибуты

* Description:String
* Diagnosises:List<[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")>
* ID:Int
* Name:String
* Patient:[Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient")
* Procedures:List<[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")>
* Worker:[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")

## Описание атрибутов

* Description:String - описание.
* Diagnosises:List<[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")> - список диагнозов.
* ID:Int - идентификатор в БД.
* Name:String - название.
* Patient:[Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient") - пациент.
* Procedures:List<[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")> - список процедур.
* Worker:[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker") - врач.