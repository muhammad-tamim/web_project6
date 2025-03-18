## What I newly learned while building this project:
1. **Using Google Fonts with CSS Variables**
    * Before, I would import Google Fonts and apply them using a class like this:
    ```
      /* style.css */
      @import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap');

      .quicksand {
        font-family: "Quicksand", sans-serif;
        font-optical-sizing: auto;
        font-weight: normal;
        font-style: normal;
      }
    ```
    ```
      <!--index.html-->
      <body class="quicksand"></body>
    ```
    * In this project, I learned how to centralize font settings using CSS variables.
    ```
    /* style.css */
    @import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap');

    :root{
      --font-primary: "Quicksand", sans-serif;
    }

    body{
      font-family: var(--font-primary);
      font-optical-sizing: auto;
      font-weight: normal;
      font-style: normal;
    }
```