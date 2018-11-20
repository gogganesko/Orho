# Описание интерфейса IDIAGNOSIS
Интерфейс предназначен для работы с методами класса Diagnosis

## Реализация интерфейса
* +Add (Diagnosis:[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")): Int — функция, добавляющая диагноз в базу данных. Параметр «[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")» — диагноз, 
который необходимо добавить в БД;
* +Save (Diagnosis:[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")): Bool — функция, редактирующая данные о диагнозе. Параметр «Diagnosis:[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")» — 
диагноз, который необходимо редактировать в БД;
* +FindByID(ID: Int): [Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")  — функция, осуществляющая поиск вида процедуры в базе данных по ID и возвращающая найденный, если такой есть. 
* +Delete(ID): Bool – функция удаляет диагноз.
* +GetDiagnosises(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Diagnosis](https://github.com/gogganesko/Orho/blob/master/docs/Diagnosis.md "объект класса Diagnosis")> — функция, возвращающая список диагнозов. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
