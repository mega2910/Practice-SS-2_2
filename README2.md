?вывести реальную таблицу умножения от 1х1 до 9х9, выводите только значения

start
new i number
set i 1

loop counter_i (10 > i)        ? внешний цикл
    new j number
    set j 1
    loop counter_j (10 > j)    ? внтуренний цикл
        new result number
        set result i * j
        log number result
        set j j + 1
    end counter_j
    set i i + 1
end counter_i

finish
