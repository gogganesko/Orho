# Описание интерфейса IKINDOFPROCEDURE
Интерфейс предназначен для работы с методами класса TypeOfProcedure

## Реализация интерфейса
* +Add (KindOfProcedure: [KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")): Int — функция, добавляющая тип процедуры в базу данных. Параметр «[KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")» — вид процедуры, 
который необходимо добавить в БД;
* +Save (KindOfProcedure: [KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")): Bool — функция, редактирующая данные о виде процедуры. Параметр «[KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")» — 
тип процедуры, который необходимо редактировать в БД;
* +FindByID(ID: Int): [KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")  — функция, осуществляющая поиск вида процедуры в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID): Bool – функция удаляет вид процедуры.
* +GetAllKindsOfProceduresOfProcedure(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[KindOfProcedure](https://github.com/gogganesko/Orho/blob/master/docs/KindOfProcedure.md "объект класса KindOfProcedure")> — функция, возвращающая список видов процедур. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
