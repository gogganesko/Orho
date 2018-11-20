# Описание интерфейса IPROCEDURE
Интерфейс предназначен для работы с методами класса Procedure

## Реализация интерфейса
* +Add (Procedure: [Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")): Int — функция, добавляющая процедуру в базу данных. Параметр «[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")» — процедура, 
которую необходимо добавить в БД;
* +Save (Procedure: [Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")): Bool — функция, редактирующая данные о процедуре. Параметр «[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")» — 
процедура, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")  — функция, осуществляющая поиск процедуры в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddFile(Path : String): Int – функция добавляет файл в процедуру. 
* +AddProcedureCabinet(CabinetID: Int, ProcedureID: Int): Int – функция добавляет процедуре кабинет в БД. Параметр ProcedureID и CabinetID – ID по которому будет осуществлен поиск в базе.
* +AddProcedurePay(PayID: Int, ProcedureID: Int): Int – функция добавляет процедуре платёж в БД. Параметр ProcedureID и PayID – ID по которому будет осуществлен поиск в базе.
* +AddProcedureWorker(WorkerID: Int, ProcedureID: Int): Int – функция добавляет процедуре работника в БД. Параметр ProcedureID и WorkerID – ID по которому будет осуществлен поиск в базе.
* +Delete(ID): Bool – функция удаляет процедуру.
* +DelProcedureCabinet(CabinetID: Int, ProcedureID: Int): Bool – удаление кабинета процедуры.
* +DelProcedurePay(PayID: Int, ProcedureID: Int): Bool – удаление платежа процедуры.
* +DelProcedureWorker(WorkerID: Int, ProcedureID: Int): Boole – удаление работника процедуры.
* +GetAllPays(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Pay](https://github.com/gogganesko/Orho/blob/master/docs/Pay.md "объект класса Pay")> — функция, возвращающая список платежей процедуры с заданными параметрами. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
  
* +GetCabinets(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List<[Cabinet](https://github.com/gogganesko/Orho/blob/master/docs/Cabinet.md "объект класса Cabinet")> — функция, возвращающая общее количество кабинетов, удовлетворяющих заданным параметрам.
* +GetProcedures(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List<[Procedure](https://github.com/gogganesko/Orho/blob/master/docs/Procedure.md "объект класса Procedure")> — функция, возвращающая общее количество процедур, удовлетворяющих заданным параметрам.
* +GetWorkers(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List<[Worker](https://github.com/gogganesko/Orho/blob/master/docs/Worker.md "объект класса Worker")> — функция, возвращающая общее количество работников, удовлетворяющих заданным параметрам.
