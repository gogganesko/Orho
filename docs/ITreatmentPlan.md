# Описание интерфейса ITREATMENTPLAN
Интерфейс предназначен для работы с методами класса TreatmentPlan

## Реализация интерфейса
* +Add (TreatmentPlan:[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")): Int — функция, добавляющая плана лечения в базу данных. Параметр «[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")» — план лечения, 
который необходимо добавить в БД;
* +Save (TreatmentPlan:[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")): Bool — функция, редактирующая данные о плане лечения. Параметр «[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan"))» — 
план лечения, который необходимо редактировать в БД;
* +FindByID(ID: Int):[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")  — функция, осуществляющая поиск плана лечения в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddDiagnosis(DiagnosisID: Int, TreatmentPlanID: Int): Int – функция добавляет плану лечения диагноз в БД. Параметр DiagnosisID и TreatmentPlanID – ID по которому будет осуществлен поиск в базе.
* +Delete(ID): Bool – функция удаляет план лечения.
* +GetAllTreatmentPlans(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")> — функция, возвращающая список всех планов лечения. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.