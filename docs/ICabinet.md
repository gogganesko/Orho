# Описание интерфейса ICABINET
Интерфейс предназначен для работы с методами класса Cabinet

## Реализация интерфейса
* +Add (Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")): Int — функция, добавляющая плана лечения в базу данных. Параметр «[TreatmentPlan](https://github.com/gogganesko/Orho/blob/master/docs/TreatmentPlan.md "объект класса TreatmentPlan")» — кабинет, 
который необходимо добавить в БД;
* +AddCabinetVisit(VisitID: Int, CabinetID: Int): Int – функция добавляет кабинету приём в БД. Параметр CabinetID и VisitID – ID по которому будет осуществлен поиск в базе.
* +DelCabinetVisit(VisitID: Int, CabinetID: Int): Int - удаление кабинета у приёма.
* +Save (Cabinet:[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")): Bool — функция, редактирующая данные о кабинете. Параметр «[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")» — 
кабинет, который необходимо редактировать в БД;
* +FindByID(ID: Int): [Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")  — функция, осуществляющая поиск кабинета в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID): Bool – функция удаляет кабинет.
* +GetCabinets(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")> — функция, возвращающая список кабинетов. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
* +GetVisits(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")> — функция, возвращающая список приёмов кабинета.