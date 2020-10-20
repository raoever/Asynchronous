<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chamada Assíncrona</title>
</head>
<body>
    <h1>Usando método fetch para requisição assíncrona em JavaScript</h1>
    <div id="titulo"></div>
    <div id="dados"></div>
</body>
<script>
    async function request(){
        const response = await fetch ('https://jsonplaceholder.typicode.com/photos');
        const object = await response.json();
        document.querySelector("dados").innerHTML = JSON.stringify(object);
    }
    request();
    document.querySelector("titulo").innerHTML = "<h2>Dados obtidos do servidor!</h2>"
</script>
</html>
