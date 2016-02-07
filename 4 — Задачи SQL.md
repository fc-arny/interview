```ruby
class Employee < ActiveRecord::Base
  belongs_to :company, inverse_of: :employees
end

class Company < ActiveRecord::Base
  has_many :employees, dependent: :destroy, inverse_of: :company
end
```

`employees`

| id |    name     | age | company_id |
| -: | ----------- | --: | ---------: |
|  1 | Андрей      |  26 |          1 |
|  2 | Юрий        |  25 |          1 |
|  3 | Кирилл      |     |          2 |
|  4 | Александр   |     |          3 |
|  5 | Инкогнито   |     |            |

`companies`

| id |     name      |
| -: | ------------- |
|  1 | AT Consulting |
|  2 | Прогресс      |
|  3 | Google        |


 1. Напишите запрос с выводом имён и возраста всех людей и названием их компании

    ```sql
    SELECT

    FROM



    ```


    |    name     | age | company       |
    | ----------- | --: | ------------- |
    | Андрей      |  26 | AT Consulting |
    | Юрий        |  25 | AT Consulting |
    | Кирилл      |     | Прогресс      |
    | Александр   |     | Google        |
    | Инкогнито   |     |               |

 2. Напишите запрос с выводом только трудоустроенных людей и названием их компании

    ```sql
    SELECT

    FROM


    ```

 3. Напишите запрос с выводом названий всех компаний, количеством сотрудников в них и их максимальным возрастом

    ```sql
    SELECT

    FROM


    ```

 4. То же, но выведите только те компании, в которых средний возраст более 30 лет

    ```sql
    SELECT

    FROM


    ```
