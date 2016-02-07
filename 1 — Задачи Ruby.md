 1. Что вернёт `A#foo` и `B#foo`?

    ```ruby
    module M
      def foo
        'M'
      end
    end

    class C
      def foo
        'C'
      end
    end

    class A < C
      include M
      def foo
        'A'
      end
    end

    class B < C
      def foo
        'B'
      end
      include M
    end
    ```

 2. Напишите метод, вычисляющий факториал:

    ```ruby
    def factorial(n)






    end
    ```
