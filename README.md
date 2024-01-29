## Фреймворк Spring (семинары)

### Урок 6. Проектирование и реализация API для серверного приложения.

Базовое задание:

Условие:

Важно! В проекте используем обязательно Spring Data и Lombok!

Разработайте небольшое веб-приложение на Spring Boot, которое будет представлять 

из себя сервис для учета личных заметок. Приложение должно поддерживать следующие функции:

Все методы контроллера возвращают ResponseEntity(как на семинаре)

1. Добавление заметки. (Подсказка @PostMapping )
   
2. Просмотр всех заметок.(Подсказка @GetMapping )
   
3. Получение заметки по id. (Подсказка @GetMapping("/{id}") )
   
4. Редактирование заметки.(Подсказка @PutMapping("/{id}") )
 
5. Удаление заметки.(Подсказка @DeleteMapping("/{id}") )
    
Структура заметки:
- ID (автоинкрементное)(тип - Long)
- Заголовок (не может быть пустым)(тип - String)
- Содержимое (не может быть пустым)(тип - String)
- Дата создания (автоматически устанавливается при создании заметки)(тип - LocalDateTime)

Подсказка:
Репозиторий насладует JpaRepository<Note, Long>. В репозитории добавляем метод Optional<Note> findById(Long id);

Подсказка:
В проект добавляем зависимости: spring data jpa, h2, lombok, spring web

Скрины работы приложения:

![1](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/1.png)

![2](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/2.png)

![3](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/3.png)

![4](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/4.png)

![5](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/5.png)

![6](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/6.png)

![7](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/7.png)

![8](https://github.com/PavelLogeiko/Spring_HW06/blob/main/images/8.png)
