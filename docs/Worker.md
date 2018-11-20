# Описание класса WORKER
Класс для работы с врачами клиники

## Атрибуты

ContactPhoneNumber:Int
ID:Int
Login:String
Name:String
Password:String
Position:Int
Specialization:String
WorkingHours:List<WorkingHour>

##Описание атрибутов
ContactPhoneNumber:Int - контактный номер телефона
ID:Int - идентификатор в БД
Login:String - логин для авторизации в системе
Name:String - ФИО
Password:String - пароль для авторизации в системе
Position:Int - позиция в таблице
Specialization:String - специализация
WorkingHours:List<WorkingHour> - список рабочего расписания