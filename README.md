# TouchSoftTest
Test task for the company TouchSoft

ArithmeticExpression
В сборниках занимательных математических задач встречается такой тип задач, когда надо из заданных чисел и арифметических знаков составить выражение, дающее какое-то заданное число. Пример такой задачи: "Составьте из чисел 4, 1, 8, 7 и арифметических знаков выражение, равное 24". Ответом может служить такое выражение: "(8-4) * (7-1)". К сожалению, некоторые авторы допускают ошибки и предлагают нерешаемую задачу, поэтому их начальник обратился к программистам.

Необходимо написать такую программу, которая определяет, можно ли построить из заданного набора выражение, равное числу N или нет. Так как это только прототип, то достаточно написать программу, которая работает только с наборами из 4-х чисел, а число N всегда равно 24.

Допустимые арифметические операторы: сложение, вычитание, умножение, деление, скобки.

На входе: массив из 4-х целых чисел от 1 до 9.
На выходе: true (если из заданного набора можно построить выражение, равное 24) или false (если из заданного набора такого выражения построить нельзя).

Пример 1.
На входе: [4, 1, 8, 7]
На выходе: true
Пояснение: (8-4) * (7-1) = 24

Пример 2.
На входе: [1, 2, 1, 2]
На выходе: false
Пояснение: из данного набора чисел невозможно составить выражение, равное 24.

Примечание: убедитесь, что в вашем решении деление корректно работает с дробями, т.е. например 4 / (1 - 2/3) = 12.

Представьте ваше решение в виде java-функции вида:
public boolean canBeEqualTo24(int[] nums) {
...
}



BarbellTest
Часть 1. Java.
В спортивном зале города N появилась штанга и набор блинов с различными массами. Для занятия спортом необходимо распределить блины по двум концам штанги таким образом, чтобы суммарный вес по оба конца штанги был одинаковый. Рассчитайте максимальный вес, который смогут поднимать спортсмены при заданном наборе блинов (с допущением, что гриф штанги невесомый).

Решение должно быть представлено в виде java-программы, у которой:
На входе: массив целых чисел, обозначающих веса блинов, входящих в набор.
На выходе: целое число, обозначающее максимальный вес, который можно поднять с заданным набором блинов.

Примеры:
1) На входе: [1,2,3,6]
На выходе: 12
Пояснение: можно нацепить блины {1,2,3} с одной стороны и блин {6} с другой, что в сумме даст 12.

2) На входе: [1,2,3,4,5,6]
На выходе: 20
Пояснение: можно нацепить блины {2,3,5} с одной стороны и блины {4,6} с другой, что в сумме даст 20. Оставшийся блин {1} не может быть нацеплен ни с одной из сторон без потери равновесия.

3) На входе: [1,2]
На выходе: 0
Пояснение: данный набор блинов невозможно нацепить без потери равновесия.

Ограничения:
1) Блин может весить от 0 до 20 фунтов.
2) В наборе может присутствовать от 1 до 1000 блинов.
3) Суммарный вес целого набора не может превышать 10000 фунтов.


Часть 2. JS.
Необходимо реализовать модель предыдущей задачи, в которой будет:
* схематичное изображение штанги (например, в виде линии)
* схематичное изображение блинов (например, в виде чисел, располагаемых на штанге)
* список блинов, не навешенных на штангу (например, в виде чисел, располагаемых под штангой)
* числовое поле для ввода массы блина
* кнопка для добавления блина с указанной массой, при нажатии на которую блин должен появиться в "списке блинов".
* При нажатии левой кнопкой мыши на блин из "списка блинов", он должен перенестить на левую сторону штанги.
* При нажатии правой кнопкой мыши на блин из "списка блинов", он должен перенестись на правую сторону штанги.
* При нажатии левой кнопки мыши на блин, находящийся на штанге, он должен перенестись обратно в "список блинов".
* Если суммарный вес по оба конца штанги стал одинаковый, то должна появиться надпись "Штанга готова".
* Если суммарный вес по оба конца штанги отличается, то надпись "Штанга готова" должна отсутствовать.