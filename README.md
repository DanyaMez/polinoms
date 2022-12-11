# ЛР 4. Арифметические операции с полиномами

__Цель работы:__ 
Разработать программу, выполняющую арифметические операции с полиномами трех переменных (x, y и z): сложение, вычитание, умножение на константу, умножение двух полиномов.
Считается, что полином составлен из мономов от трех переменных с ограничением на степень каждой переменой от 0 до 9 (Опцианально можно расширить данное ограничение). Коэффициенты полинома - вещественные числа. 
Работоспособность программы необходимо проверить с помощью Google Test-ов. Кроме того, необходимо разработать пользовательское консольное приложение. 

__Особенности реализации:__

1. В качестве структуры хранения полинома использовать список мономов с ненулевыми коэффициентами (односвязный или двухсвязный). Односвязный список удобнее реализовать с фиктивной головой. Элементы списка хранить упорядоченными.
1. Степень полинома хранить в "свернутом" виде, т. е. степень должна быть представлена как трехзначное число, где число сотен – это степень при переменной “x”, число десятков - степень при переменной “y”, число единиц - степень при переменной “z”.
1. Сложение полиномов осуществлять алгоритмом слияния упорядоченных массивов.
1. Вычитание полиномов допускается выполнять через сложение с умножением на константу (C = A - B = A + (-1)*B)
1. При умножении и сложение (вычитание) необходимо следить, чтобы в итоговом полиноме были приведены подобные слагаемые и не хранилось мономов с нулевым коэффициентом.
1. Если при умножении полиномов полученные степени переменных больше 9, выводить сообщение об ошибке.
1. Считывание полинома у пользователя допускается в любом удобном для вас виде. Необходимо предоставить пользователю правила ввода данных
1. Следует учесть, что пользователь может вводить полином, не упорядочив в нем мономы.