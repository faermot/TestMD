# TestMD 
<img src="https://github.com/user-attachments/assets/f57852aa-b866-4a98-b1f2-5788c74bcd49" width="135" />

## Самостоятельная работа

<ins>**1.**</ins> C# - очередной язык из бесконечного цикла эволюции языков программирования. Это объектно ориентированный яп, разработанный Microsoft. Изначально задумывался как язык для написания программ под Windows, но сейчас это очень универсальный язык. (Используется для написания программ, игр, драйверов, и т.д.)

<ins>**2.**</ins> Особенности C#:
    - Строго типизированный
    - Объектно-ориентированный
    - Полиморфный
    
<ins>**3.**</ins> .NET Framework - оболочка, определяющая среду для разработки и выполнения сильно распределённых приложений, основанный на использовании компонентных обектов. Связь среды .NET Framework с C# обусловлена наличием общего языка CLR (Common Language Runtime), который позволяет программам, написанным на разных языках, взаимодействовать друг с другом. C# является одним из основных языков, для которого разработан .NET Framework, и использует его библиотеки для создания приложений.

<ins>**4.**</ins> CLR (Common Language Runtime) - это часть .NET Framework, которая делает программы переносимыми. Поддерживает многоязыковое программирование и обеспечивает безопасность.

<ins>**5.**</ins> Струкура программы на C# представляет собой:

        1. Пространство имен (namespace)
        
        2. Классы (class)
        
        3. Метод Main — точка входа в программу
        
        4. Директивы using для подключения библиотек
        
        5. Поля, методы, свойства для реализации логики

<ins>**6.**</ins> Различия с C++:
    - C++ компилируется в машинный код, C# же компилируется в промежуточный язык и выполняется с помощью CLR. Это делает C# чуть менее производительным, но более безопасным.
    - В C++ программист должен вручную управлять памятью, тогда как в C# эта задача делегируется сборщику мусора, что снижает риск ошибок, связанных с утечками памяти.
    Различия с Java (хотя Java и C# похожие яп):
    - C# тесно связан с .NET, а Java — с JVM. Обе платформы обеспечивают межплатформенную совместимость, но C# больше интегрирован с экосистемой Windows.
    - Синтаксис у C# и Java похож, но C# предлагает более широкий набор функций, таких как свойства, события и делегаты.
    
<ins>**7.**</ins> Пространства имен позволяют организовать код программы в логические блоки, поволяют объединить и отделить от остального кода некоторую функциональность, которая связана некоторой общей идеей или которая выполняет определенную задачу.

<ins>**8.**</ins> Сборка представляет собой скомпилированный код и метаданные, которые нужны для выполнения программы. Она может быть как библиотекой, которую можно использовать повторно в других проектах, так и полноценным приложением.

<ins>**9.**</ins> Управляемый код — это код, который выполняется под контролем .NET CLR. Он включает программы, написанные на C# и других .NET языках (CLR управляет такими аспектами выполнения управляемого кода, как управление памятью, обработка исключений, безопасность и т.д.). Неуправляемый код — это код, который выполняется вне среды CLR. Это обычно низкоуровневый код, написанный на языках, таких как C или C++, и напрямую компилируется в машинный код, специфичный для целевой платформы. Программы, написанные на неуправляемом коде, не имеют преимуществ, предоставляемых CLR (программисту нужно вручную управлять памятью и безопасностью)

<ins>**10.**</ins> JIT компилятор переводит код, написанный на MSIL в испольняемый. JIT (Just in time) - эта аббревиатура означает, что выполнение кода происходит в точно нужный момент. В результате компиляции, помимо MSIL кода образуются метаданные - они описывают данные, используемые программой, и позволяют коду обмениватся с другим кодом.

<ins>**11.**</ins> Типы данных в C# имеют особое значение, т.к. C# строго типизированный яп. Это означает, что все операции проверяются на соответсвие типов. C# содержит 2 категории встроенных типов данных - типы значений и ссылочный тип. Основное ядро языка составляет базовые 13 типов. 

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

<ins>**15.**</ins> Строка в C# - набор символов, которые содержатся в двойных ковычках. Тип данных string является ссылочным типом. Со строками можно выполнять различные операции. Методы (для обработки строк):
    1. Свойство Lenght - возвращает текущую длинну строки
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


    
    
