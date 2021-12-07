# Task. Многопоточность
Разработать многопоточное приложение, использующее разделяемые 
ресурсы. В приложении должна быть реализована функциональность, 
определенная индивидуальным заданием.
## Требования
+ Любая сущность, желающая получить доступ к разделяемому ресурсу, должна быть 
потоком.
+ Программа должна использовать возможности синхронизации, поставляемые 
библиотеками java.util.concurrent, java.util.concurrent.atomic и 
java.util.concurrent.locks. 
+ Не использовать synchronized, volatile, а также BlockingQueue и другие ограниченно 
потокобезопасные коллекции.
+ Классы и другие сущности приложения должны быть грамотно структурированы по пакетам 
и иметь отражающую их функциональность название.
+ Использовать шаблон State для описания состояний объекта, если только этих состояний 
больше двух. 
+ Для создания потоков разрешается использовать по возможности Callable
+ Запускать потоки с помощью ExecutorService. 
+ Вместо Thread.sleep использовать только возможности перечисления TimeUnit. 
+  Данные инициализации объектов считывать из файла. Данные в файле корректны.
+ В приложении должен присутствовать потокобезопасный Singleton. При его создании 
запрещено использовать enum. 
+ Для записи логов использовать Log4J2. 
+Для вывода работы потоков использовать метод main.
## Индивидуальные задания
**Маршрут.** Автобусный маршрут состоит из последовательности различных остановок. 
На одной остановке может останавливаться несколько автобусов одновременно, но не 
более заданного числа. Если автобусы стоят на остановке пассажиры могут пересесть 
из одного автобуса в другой или остаться на остановке. Автобусы могут ездить каждый 
по своему маршруту.
