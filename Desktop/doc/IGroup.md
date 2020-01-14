# Описание интерфейса Group
Интерфейс предназначен для работы с методами класса Group

## Реализация интерфейса
* +AddGroup (Group:[Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")): Int — функция, добавляющая группу в базу данных. Параметр «[Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")» — группа, 
которую необходимо добавить в БД;
* +EditGroup (Group:[Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")): Bool — функция, редактирующая данные о группе. Параметр «[Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")» — 
группа, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")  — функция, осуществляющая поиск группы в базе данных по ID и возвращающая найденную, если такая есть. 
* +Del(ID): Bool – функция удаляет группу.
* +GetAllGroups(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Group](https://github.com/gogganesko/Orho/blob/master/docs/Group.md "объект класса Group")> — функция, возвращающая список групп. 
* +GetAllStudent(ID : int) List<Student> - функция возвращающая список учащихся в этой группе.
* +Getchedule(ID : int) List<Schedule> - функция возвращающая расписание заданной группы.
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
