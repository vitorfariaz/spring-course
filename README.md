# spring-course
O objetivo desse repositório é ser um guia para quem quer aprender sobre Spring

## Introdução
Aqui vou passar alguns cursos gratuito com a teoria + prática sobre spring e vou passar alguns exercícios. <br />
A ideia é: faça os cursos como **apoio** para o desenvolvimento dos exercícios prátiocos solicitados aqui. Faça o curso enquanto resolve os exercícios e não assitir todo o curso e só depois colocar em prática. <br />
Qualquer dúvida me mande uma mensagem pelo instagram(@vitorfariaz) e/ou tente pesquisar no google <br />

[Curso Spring](https://www.youtube.com/watch?v=LXRU-Z36GEU)


Os exercícios começam bem simples e vão dificultando conforme você vai aprendendo novos conceitos. <br />
Alguns exercícios vou escreve-los de forma que não fique tão explícito o que você tem que fazer para resolver o problema e sim o resultado esperado. <br />
Exemplo: <br />
Crie uma API que retorna uma exceção quando chamar o recurso base localhost:porta/ <br />

Nesse caso você terá que inicializar um projeto Spring, podendo usar o [Spring initializr](https://start.spring.io/), baixar as dependencias do Web e subir na sua máquina local o projeto e ver se quando chama o recurso `localhost:8080/` está retornando uma exceção do servidor que foi levantado junto com o Spring.

## Exercícios


Criar um projeto spring e subir loucamente e chamar localhost/ pra ver se subiu mesmo

Criar uma classe service e colocar sysout no construtor pra ver que o spring cria a classe


GET /cars,  que retorne "hello world"

POST /cars, que recebe
{"marca" : "corsa"}
E retorna "carro corsa recebido"

Salvar no banco o valor enviado para POST /cars

Adicionar atributo COR

DELETE /cars/id

GET /cars

GET /cars/id

PATCH /cars/id

Adicionar regras
Não pode salvar carro mesma cor e mesma marca

Não pode editar carro pra mesma cor e mesma marca

Não pode salvar/editar mais de 5 carros da mesma marca

GET /cars?cor=verde

Consultar serviço externo pra validar valor do carro e salvar no banco.

Mensageria: depois eu vejo
