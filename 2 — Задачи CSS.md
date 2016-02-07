## Basic

 1. Написать HTML, подходящий под селектор `#my p.announce, .foo.bar li a:hover+span`

    ```html




    ```

 2. Специфичность селекторов

    Даны CSS-правила:

    ```css
    div         { color: red';    }
    div.foo     { color: green;   }
    .foo        { color: cyan;    }
    .foo#bar    { color: magenta; }
    #bar        { color: purple;  }
    div#bar.foo { color: blue;    }
    ```

    Какого цвета будет текст в каждом из данных тэгов, почему?

    ```html
    <div>Раз</div>
    <p class="foo">Два</p>
    <div class="foo">Три</div>
    <div class="foo" id="bar">Четыре</div>
    <p class="foo" id="bar">Пять</p>
    ```
