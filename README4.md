? найдите число Пи

start
new pi number
set pi 0
new znak number
set znak 1  ? Для знака +-
new n number
set n 0     ? Счётчки шагов
new shagi number
set shagi 100000
new znamenatel number  

loop calc (shagi > n)
    set znamenatel 2 * n + 1
    set pi pi + (znak * 1000000 / znamenatel)  ? тип дроби
    set znak znak * -1  ? Меняем знак
    set n n + 1
end calc

? Умножаем на 4 и делим на лям, как и в цикле наоборот, а вообще это чтобы сохранить десятичные дроби в виде целых чисел
set pi 4 * pi
set pi pi / 1000000

log string "pi ~~ "
log number pi
finish
