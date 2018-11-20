# Описание интерфейса ITYPEOFPROCEDURE
Интерфейс предназначен для работы с методами класса TypeOfProcedure

## Реализация интерфейса
* +Add (TypeOfProcedure:[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")): Int — функция, добавляющая тип процедуры в базу данных. Параметр «[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")» — тип процедуры, 
который необходимо добавить в БД;
* +AddWorkingHour(WorkingHourID: Int, TypeOfProcedureID: Int): Int – функция добавляет расписание типу процедуры в БД. Параметр WorkingHourID и TypeOfProcedureID – ID по которому будет осуществлен поиск в базе.
* +DelWorkingHour(WorkingHourID: Int, TypeOfProcedureID: Int): Int - удаление расписания типа процедуры.
* +Save (TypeOfProcedure:[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")): Bool — функция, редактирующая данные о типе процедуры. Параметр «[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")» — 
тип процедуры, который необходимо редактировать в БД;
* +FindByID(ID: Int): [TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")  — функция, осуществляющая поиск процедуры в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID): Bool – функция удаляет процедуру.
* +GetAllTypesOfProcedure(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[TypeOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/TypeOfProcedure.md "объект класса TypeOfProcedure")> — функция, возвращающая список типов процедур. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
