<!DOCTYPE html>
<html>
    <head>
        <meta charset='utf-8'>
    </head>

    <body>
        <button id="btn">ClickMe</button>

        <script>
            const button = document.querySelector('#btn');
            const body = document.querySelector('body');
            const colors = ['red', 'blue', 'green', 'yellow', 'black'];

            body.style.backgroundColor = 'violet';

            button.addEventListener('click', changeBackground);
            setInterval(changeBackground, 3000)
            function changeBackground() {
                let index;

                index = Math.floor(Math.random() * colors.length);

                body.style.backgroundColor = colors[index];

            }
        </script>
    </body>
</html>

