# Linter
## Использование линтер-плагина для IDEA.
### Для опробования работы линтер-плагином взят исходный код программы, работающей с hashmap словарем и списком. 
### Cсылка на исходный код  ([https://github.com/SvetlanaBoichenko/lessons/edit/main/ListMap.java]). 
### Перед установкой линтера в окне результатов компиляции не наблюдалось  ни ошибок, ни предупреждений. 
### В процессе использования линтер выдал большоое количество замечаний. 
### Некоторые из замечаний типа "issue":

 - строка 25 - "entrySet()" should be iterated when both the key and value are needed
   ####    я не стала следовать рекомендации, так как применение этого правила привело бы к нарушению логики и результат оказался бы неверным.
 - строки 29, 45, 47 -  Standard outputs should not be used directly to log anything
   ####    также замечание не отработано, потому что мне не надо логгировать результат выполнения программы.
 - строка 2 - Unnecessary imports should be removed
   ####    неиспользуемую библиотеку Array удалила за ненадобностью.
 - строка 43 - Assignments should not be redundant
   ####    имеет смысл. Так как возвращаемое значение совпадает с параметром функции. Здесь ошибки не вызвало, но возможно может привести к ошибке в других случаях. Исправила. 

### Замечания типа "warning". 

 - строка 44 - Actual value of parameter 'ntimes' is always '11'
 ####    справедливое замечание. Ввела переменную вместо константы.   
 - Строка 8 и 38 - Explicit type argument Integer, Integer can be replaced with <>. The diamond operator ("<>") should be used
 ####    рекомендовано не использовать при создании словаря и списка типов используемых параметров. Исправила.
 #### Также предложено изменить названия функция и переменных. 

### В результате корректировки код программы стал выглядеть следующим образом:
([https://github.com/SvetlanaBoichenko/lessons/blob/main/ListMap.java]).
