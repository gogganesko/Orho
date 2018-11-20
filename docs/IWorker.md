# Описание интерфейса IWORKER
Интерфейс предназначен для работы с методами класса Worker

## Реализация интерфейса
* +Add (Worker: [Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")): Int — функция, добавляющая врача в базу данных. Параметр «Worker» — врач, 
которого необходимо добавить в БД;
* +Save (Worker: [Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")): Bool — функция, редактирующая данные о читателе. Параметр «Worker» — 
врач, которого необходимо редактировать в БД;
* +FindByID(ID: Int): [Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")  — функция, осуществляющая поиск врача в базе данных по ID и возвращающая найденный, если такой есть. 
+AddWorkerProcedure(ProcedureID: Int, WorkerID: Int): Int – функция добавляет врачу процедуру в БД. 
Параметр WorkerID и ProcedureID – ID по которому будет осуществлен поиск в базе.
* +AddWorkeVisit(VisitID: Int, WorkerID: Int): Int – функция добавляет врачу приём в БД. Параметр WorkerID и VisitID – ID по которому будет осуществлен поиск в базе.
* +AddWorkingHour(WorkingHourID: Int, WorkerID: Int): Int – функция добавляет врачу запись в расписании в БД. Параметр WorkerID и WorkingHourID – ID по которому будет осуществлен поиск в базе.
* +AddWorkerProcedure(ProcedureID: Int, WorkerID: Int): Int – функция добавляет врачу запись в расписании в БД. Параметр WorkerID и WorkingHourID – ID по которому будет осуществлен поиск в базе.
* +Delete(ID): Bool – функция удаляет врача.
* +DeleteWorkingHour (WorkingHourID: Int, WorkerID:Int):Bool – удаление записи расписания врача.
* +DelWorkerProcedure(ProcedureID: Int, WorkerID:Int):Bool – удаление процедуры врача
* +DeleteWorkerVisit (VisitID: Int, WorkerID:Int):Bool – удаление приёма врача
* +GetProcedures(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <Procedure> — функция, возвращающая список процедур врача с заданными параметрами. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
  
* +GetVisists(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List<[Visit](https://github.com/gogganesko/Orho/blob/master/docs/Visit.md "объект класса Visit")> — функция, возвращающая общее количество приёмов, удовлетворяющих заданным параметрам.
* +GetWorkers(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")> - функция, возвращающая общее количество врачей, удовлетворяющих заданным параметрам.