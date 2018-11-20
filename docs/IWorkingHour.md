# Описание интерфейса IWORKINGHOUR
Интерфейс предназначен для работы с методами класса WorkingHour

## Реализация интерфейса
* +Add (WorkingHour:[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")): Int — функция, добавляющая расписание в базу данных. Параметр «[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")» — запись расписания, 
который необходимо добавить в БД;
* +Save (WorkingHour:[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")): Int — функция, добавляющая расписание в базу данных. Параметр «[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")): Bool — функция, редактирующая данные о записи расписания. Параметр «WorkingHour:[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")): Int — функция, добавляющая расписание в базу данных. Параметр «[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")» — 
запись расписания, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")  — функция, осуществляющая поиск записи расписания в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID): Bool – функция удаляет запись расписания.
* +GetAllWorkingHours(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[WorkingHour](https://github.com/gogganesko/Orho/blob/master/docs/WorkingHour.md "объект класса WorkingHour")> — функция, возвращающая список записей расписания по выбранным параметрам. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
