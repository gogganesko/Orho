# Описание интерфейса IPATIENT
Интерфейс предназначен для работы с методами класса Patient

## Реализация интерфейса
* +Add (Patient: [Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient")): Int — функция, добавляющая врача в базу данных. Параметр «Patient» — пациент, 
которого необходимо добавить в БД;
* +Save (Patient: [Patient](https://github.com/gogganesko/Orho/blob/master/docs/Patient.md "объект класса Patient")): Bool — функция, редактирующая данные о читателе. Параметр «Patient» — 
пациент, которого необходимо редактировать в БД;
* +FindByID(ID: Int): Int  — функция, осуществляющая поиск пациента в базе данных по ID и возвращающая найденный, если такой есть. 
* +AddPatientDiagnosis(DiagnosisID: Int, PatientID: Int): Int – функция добавляет пациенту диагноз в БД. 
Параметр PatientID и DiagnosisID – ID по которому будет осуществлен поиск в базе.
* +AddPatientVisit(VisitID: Int, PatientID: Int): Int – функция добавляет пациенту приём в БД. Параметр PatientID и VisitID – ID по которому будет осуществлен поиск в базе.
* +Delete(ID): Bool – функция удаляет пациента.
* +DelPatientDiagnosis (DiagnosisID: Int, PatientID:Int):Bool – удаление записи диагноза пациента.
* +DelPatientVisits(VisitID: Int, PatientID:Int):Bool – удаление приёма пациента.
* +GetAllDiagnosises(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <Diagnosis> — функция, возвращающая список диагнозов пациента с заданными параметрами. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
  
* +GetVisists(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List<Visit> — функция, возвращающая общее количество приёмов, удовлетворяющих заданным параметрам.
* +GetAllPatients(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <Worker> - функция, возвращающая общее количество пациентов, удовлетворяющих заданным параметрам.