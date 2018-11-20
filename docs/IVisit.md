# Описание интерфейса IVISIT
Интерфейс предназначен для работы с методами класса Visit

## Реализация интерфейса
* +Add (Visit: [Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")): Int — функция, добавляющая приём в базу данных. Параметр «[Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")» — приём, 
который необходимо добавить в БД;
* +Save (Visit: [Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")): Bool — функция, редактирующая данные о приёме. Параметр «[Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")» — 
приём, который необходимо редактировать в БД;
* +FindByID(ID: Int): [Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")  — функция, осуществляющая поиск приёма в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddProcedure(VisitID: Int, ProcedureID: Int): Int – функция добавляет приёму процедуру в БД. Параметр ProcedureID и VisitID – ID по которому будет осуществлен поиск в базе.
* +Delete(ID): Bool – функция удаляет приём.
* +DelVisitProcedure(VisitID: Int, ProcedureID: Int): Bool – удаление у приёма процедуры.
* +GetAllVisits(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")> — функция, возвращающая список всех приёмов. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.