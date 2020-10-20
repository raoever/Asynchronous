#Asynchronous

1 - qual problema percebeu ao realizar tais alterações?
O título é inserido muito antes da chegada dos dados e caso haja um problema no rebebimento dos dados o título vai carregar de qualquer maneira.

2 - explique porque o problema ocorreu e o qual a relação com chamadas assíncronas;
Porque o comando de innerHTML foi colocado fora da função assíncrona e não checa se a resposta foi bem ou mal sucedida.

3 - altere o código para resolver o problema.
innerHTML colocado dentro da função assíncrona e também foi adicionado um try/catch para mostrar uma mensagem de erro caso os dados não sejam carregados corretamente.
