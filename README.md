## Push_swap 

Цель проекта - отсортировать массив чисел, используя 2 стека: A и B.

Правила: 
Программа состоит из 2 стеков, названных A и B. 
* A содержит случайное число положительных или отрицательных чисел без дубликатов.
* B пусто

Цель состоит в том, чтобы отсортировать числа в порядке возрастания в стеке A.
Для этого в вашем распоряжении следующие операции:

sa: swap a - поменять местами первые 2 элемента на вершине стека A. (Ничего не делать, если есть только один элемент или их нет).

sb: swap b - поменять местами первые 2 элемента наверху стека B. (Ничего не делать, если есть только один элемент или их нет).

ss: sa и sb одновременно.

pa: push a - возьмите первый элемент вверху B и поместите его вверху A. Ничего не делать, если B пусто.

pb: push b - возьмите первый элемент вверху A и поместите его вверху B. Ничего не делать, если A пусто.

ra: rotate a - сдвинуть вверх все элементы стека A на 1. Первый элемент становится последним.

rb: rotate b - сдвинуть вверх все элементы стека B на 1. Первый элемент становится последним.

rr: ra и rb одновременно.

rra: reverse rotate a - сдвинуть вниз все элементы стека A на 1. Последний элемент становится первым.

rrb: reverse rotate b - сдвинуть вниз все элементы стека B на 1. Последний элемент становится первым.

rrr: rra и rrb одновременно. 

Программa с именем push_swap, которая получает в качестве аргумента стек, формированный как список целых чисел, а на выходе выводит операции, разделенные '\n', необходимые для сортировки списка подаваемых чисел.
В случае ошибки отображает "Error", за которой следует '\n' для стандартной ошибки. К ошибкам относятся, например: некоторые аргументы не являются целыми числами, некоторые аргументы больше целого числа и/или есть дубликаты.

Бонусная часть:

Программа с именем checker, которая будет получать в качестве аргумента стек, форматированный как список целых чисел. Если аргумент не задан, проверка останавливается и ничего не отображает.
Checker будет ждать и читать инструкции на стандартном вводе, за каждой инструкцией будет следовать ’\n’. Как только все инструкции будут прочитаны, программа проверки выполнит их в стеке, полученном в качестве аргумента.
Если после выполнения этих инструкций стек A фактически отсортирован, а B пуст, тогда программа проверки отображает на стандартном выходе «OK», за которым следует a ’\n’. Во всех остальных случаях программа проверки тображает "KO", за которым следует '\n’ в стандартном выводе.
В случае ошибки отображает "Error", за которой следует '\n' для стандартной ошибки. К ошибкам относятся, например: некоторые аргументы не являются целыми числами, некоторые аргументы больше целого числа, есть дубликаты, инструкция не существует и/или имеет неправильный формат.

## Usage

> bash && make && make bonus

> ARG="4 67 3 87 23"; ./push_swap $ARG | ./checker $ARG

> ARG="4 67 3 87 23"; ./push_swap $ARG | wc -l

<img src="./docs/Screen Shot 2021-10-01 at 1.43.21 PM.png">

Полный subject на английском языке можно найти <a href="./docs/en.subject.pdf">тут</a>.

