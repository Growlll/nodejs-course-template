# Caesar cipher CLI tool

### Запуск приложения

- Склонировать себе репозиторий ```git clone https://github.com/Growlll/nodejs-course-template.git```
   
- Установить все зависимости ```npm install```

- Перейти в папку приложения ```cd caesar-cipher-cli```

- Запустить приложения с указаными ниже параметрами

### Параметры запуска

1. -s, --shift: Обязательный параметр! Сдвиг в шифровании. Любое целое число
2. -i, --input: Путь/имя входного файла с данными для обработки. Если параметр не указан ввод данных будет идти из консоли. Если указан неверные данные, приложение завершиться с ошибкой
3. -o, --output: Путь/имя выходного файла с результатами работы приложения. Если параметр не указан вывод данных будет в консоль. Файл автоматически не создается, необходимо его создать. Если указаны неверные данные, приложение завершиться с ошибкой
4. -a, --action: Обязательный параметр! Направление работы приложения - шифрование/дешифрование. Доспустимые значения (encode | decode). Если shift меньше 0 и action = encode, результат будет как для action = decode для shift больше 0

#### Пример использования

```$ node index -a encode -s 7 -i "./input.txt" -o "./output.txt"```

```$ node index --action encode --shift 1 --input plain.txt --output encoded.txt```

```$ node index --action decode --shift 7 --input in.txt --output out.txt```
