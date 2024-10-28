# TestMD 
<img src="https://github.com/user-attachments/assets/f57852aa-b866-4a98-b1f2-5788c74bcd49" width="135" />

## Самостоятельная работа

<ins>**1.**</ins> C# - очередной язык из бесконечного цикла эволюции языков программирования. Это объектно ориентированный яп, разработанный Microsoft. Изначально задумывался как язык для написания программ под Windows, но сейчас это очень универсальный язык. (Используется для написания программ, игр, драйверов, и т.д.)

<ins>**2.**</ins> Особенности C#:
    - Строго типизированный
    - Объектно-ориентированный
    - Полиморфный
    
<ins>**3.**</ins> .NET Framework - оболочка, определяющая среду для разработки и выполнения сильно распределённых приложений, основанный на использовании компонентных объектов. Связь среды .NET Framework с C# обусловлена наличием общего языка CLR (Common Language Runtime), который позволяет программам, написанным на разных языках, взаимодействовать друг с другом. C# является одним из основных языков, для которого разработан .NET Framework, и использует его библиотеки для создания приложений.

<ins>**4.**</ins> CLR (Common Language Runtime) - это часть .NET Framework, которая делает программы переносимыми. Поддерживает многоязыковое программирование и обеспечивает безопасность.

<ins>**5.**</ins> Структура  программы на C# представляет собой:

        1. Пространство имен (namespace)
        
        2. Классы (class)
        
        3. Метод Main — точка входа в программу
        
        4. Директивы using для подключения библиотек
        
        5. Поля, методы, свойства для реализации логики

<ins>**6.**</ins> 
1. Различия с C++:
    - C++ компилируется в машинный код, C# же компилируется в промежуточный язык и выполняется с помощью CLR. Это делает C# чуть менее производительным, но более безопасным.
    - В C++ программист должен вручную управлять памятью, тогда как в C# эта задача делегируется сборщику мусора, что снижает риск ошибок, связанных с утечками памяти.
    
2. Различия с Java (хотя Java и C# похожие яп):
    - C# тесно связан с .NET, а Java — с JVM. Обе платформы обеспечивают межплатформенную совместимость, но C# больше интегрирован с экосистемой Windows.
    - Синтаксис у C# и Java похож, но C# предлагает более широкий набор функций, таких как свойства, события и делегаты.
    
<ins>**7.**</ins> Пространства имен позволяют организовать код программы в логические блоки, позволяют  объединить и отделить от остального кода некоторую функциональность, которая связана некоторой общей идеей или которая выполняет определенную задачу.

<ins>**8.**</ins> Сборка представляет собой скомпилированный код и метаданные, которые нужны для выполнения программы. Она может быть как библиотекой, которую можно использовать повторно в других проектах, так и полноценным приложением.

<ins>**9.**</ins> Управляемый код — это код, который выполняется под контролем .NET CLR. Он включает программы, написанные на C# и других .NET языках (CLR управляет такими аспектами выполнения управляемого кода, как управление памятью, обработка исключений, безопасность и т.д.). Неуправляемый код — это код, который выполняется вне среды CLR. Это обычно низкоуровневый код, написанный на языках, таких как C или C++, и напрямую компилируется в машинный код, специфичный для целевой платформы. Программы, написанные на неуправляемом коде, не имеют преимуществ, предоставляемых CLR (Программисту  нужно вручную управлять памятью и безопасностью)

<ins>**10.**</ins> JIT компилятор переводит код, написанный на MSIL в исполняемый. JIT (Just in time) - эта аббревиатура означает, что выполнение кода происходит в точно нужный момент. В результате компиляции, помимо MSIL кода образуются метаданные - они описывают данные, используемые программой, и позволяют коду обмениваться  с другим кодом.

<ins>**11.**</ins> Типы данных в C# имеют особое значение, т.к. C# строго типизированный яп. Это означает, что все операции проверяются на соответствие  типов. C# содержит 2 категории встроенных типов данных - типы значений и ссылочный тип. Основное ядро языка составляет базовые 13 типов. 

<ins>**12.**</ins> Значимые типы — включают числа, логические значения, символы, структуры и перечисления, хранящиеся в стеке.
Ссылочные типы  — включают строки, классы, интерфейсы, делегаты и массивы, хранящиеся в куче.

<ins>**13.**</ins> Nullable — это тип, который позволяет переменной хранить значение null помимо её обычных допустимых значений. (В C# nullable типы создаются с использованием оператора ?)

<ins>**14.**</ins> Целочисленные типы:
В C# определено 9 основных целочисленных типов:

    | |Тип|Размер|Диапазон|
    |-|------|--------|----------------------------------------------------------|
    |1|Char  |8 бит   |                                                          |
    |2|Byte  |8 бит   |0 - 255                                                   |
    |3|SByte |8 бит   |-128 - 127                                                |
    |4|Short |16 бит  |-32 768 - 32 767                                          |
    |5|UShort|16 бит  |0 - 65 535                                                |
    |6|Int   |32 бита |−2 147 483 648 - 2 147 483 647                            |
    |7|UInt  |32 бита |0 - 4 294 967 295                                         |
    |8|Long  |64 бита |−9 223 372 036 854 775 808 - 9 223 372 036 854 775 807    |
    |9|ULong |64 бита |0 - 18 446 744 073 709 551 615                            |

<ins>**15.**</ins> Строка в C# - набор символов, которые содержатся в двойных кавычках. Тип данных string является ссылочным типом. Со строками можно выполнять различные операции. Методы (для обработки строк):
    1. Свойство Lenght - возвращает текущую длину строки
    2. Copy - возвращает копию строки
    3. CompareTo - данный метод возвращает отрицательное значение, если вызывающая строка меньше текущей
    4. IndexOf - выполняет поиск подстроки в строке
    5. LastIndexOf - выполняет поиск подстроки в строке и возвращает индекс последнего вхождения искомой подстроки
    6. ToLower - возвращает строчную версию вызываемой строки
    7. ToUpper - возвращает прописную версию вызывающей строки

<ins>**16.**</ins> Для преобразования строки в число и наоборот можно использовать класс Convert:
```C#
string numberString = "123";
int number = Convert.ToInt32(numberString);
// обратно в строку
int anotherNumber = 456;
string anotherNumberString = Convert.ToString(anotherNumber);
```

<ins>**17.**</ins> Перечисления  (enum) в C# - это специальный тип данных, который позволяет задавать набор именованных констант. Перечисления делают код более читаемым и удобным для работы с фиксированным набором значений.  

<ins>**18.**</ins> Особенности **var**:
1. Неявная типизация 
    > При использовании var не указывается явный тип переменной. Компилятор определяет тип переменной во время компиляции на основе значения, которое ей присваивается. 
2. Обязательное присваивание при объявлении
    > Переменная, объявленная с использованием var, должна быть инициализирована в момент объявления.
3. Статическая типизация
    > Тип переменной определяется на этапе компиляции, и его нельзя изменить в процессе выполнения программы.

<ins>**19.**</ins> Условный оператор __if__ реализует выполнение определенных команд при условии, что используемое логическое выражение истинно, соответственно результатом может быть True/False. В зависимости от условий выполнения выполняется только 1 из серии команд, входящих в ветвление.

<ins>**20.**</ins> Оператор __switch__ - используется как совместно, так и для замены оператора if. Оператор switch принимает выражение или переменную(селектор) и далее значение этой переменной сравнивается со значением каждого кейса. Когда оператор switch находит идентичное значение, то выполняется соответствующий кейс, вместе с блоком кода. После выполнения кода, операция будет прервана оператором brake, который обязательно должен быть в конце каждого кейса. Если ни одно значение кейса не выполняется, то выполняется оператор default - он схож с оператором else.

<ins>**21.**</ins> Для проверки нескольких условий можно использовать if else. Для проверки нескольких условий в 1 условном операторе, можно использовать логические операторы.

<ins>**22.**</ins> Тернарный  (третичный) оператор - обязательно должен возвращать значение, иначе будет ошибка.

<ins>**23.**</ins> :Логические операторы: 
    
        1. & - И
        
        2. | - ИЛИ
        
        3. ^ - Исключающее ИЛИ
        
        4. && - сокращённое И
        
        5. || - сокращённое ИЛИ
     
        6. ! - НЕ

<ins>**24.**</ins> Ниже перечислены логические операторы в порядке убывания приоритета:

        1. ! - НЕ
        
        2. ! - НЕ
        
        3. ^ - Исключающее ИЛИ
        
        4. | - ИЛИ
        
        5. && - сокращённое И
     
        6. || - сокращённое ИЛИ

<ins>**25.**</ins> В C# логические операторы позволяют комбинировать несколько условий и таким образом создавать сложные логические выражения. 

<ins>**26.**</ins> В C# имеются следующие виды циклов:
1. for
2. foreach
3. while
4. do...while

<ins>**27.**</ins> Цикл for - цикл, используемый для выполнения одной конструкции. Цикл for будет выполнятся до тех пор, пока вычисление элемента условия даёт истинный результат. Как только условие станет ложным, выполнение программы продолжится с конструкцией, которая идёт за циклом for. Управляющая переменная цикла for может изменятся как с положительным так и с отрицательным прирощением. При этом величина этого приращения может быть любой. Важным условием при проверке выражения и его тестировании идёт в начале цикла for, и если эта проверка возвращает False, то тело цикла не выполнится ни разу. Цикл for подходит лучше всего,  когда известно количество итераций, когда необходимо последовательно увеличивать/уменьшать индекс в цикле.

<ins>**28.**</ins> Цикл while сразу проверяет истинность некоторого условия, и если условие истинно, то код цикла выполняется. Данный цикл предпочтительнее, когда неизвестно количество итераций, если необходимо проверять условие перед каждой итерацией, если цикл должен продолжаться до тех пор, пока выполняется какое-то условие, и это условие может измениться в ходе выполнения.

<ins>**29.**</ins> В отличии от циклов for и While, в которых условие проверяется при входе в цикл, do...While проверяет условие при выходе из цикла. Это означает, что цикл do...While выполнится хотя бы 1 раз. 

<ins>**30.**</ins> Оператор break используется для немедленного выхода из цикла, прерывая его выполнение. Оператор continue используется для пропуска текущей итерации цикла и перехода к следующей итерации. Если условие continue выполняется, оставшаяся часть кода в текущей итерации не будет выполнена, и выполнение перейдет к следующему циклу.

<ins>**31.**</ins> Массив (Array) - коллекция переменных одинакового типа, обращение к которым происходит с использованием общего для всех имени. В C# массивы могут быть одномерными и многомерными. Массивы представляют собой удобное средство связанных переменных. Для объявления одномерного массива  используется следующая запись:
```C#
тип[] имяМассива = new Тип[размер];
```




















