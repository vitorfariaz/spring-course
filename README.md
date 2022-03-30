# spring-course
O objetivo desse repositório é ser um guia para quem quer aprender sobre Spring

## Introdução
Aqui vou passar alguns cursos gratuito com a teoria + prática sobre spring e vou passar alguns exercícios. <br />
A ideia é: faça os cursos como **apoio** para o desenvolvimento dos exercícios práticos solicitados aqui. Faça o curso enquanto resolve os exercícios e não assitir todo o curso e só depois colocar em prática. <br />
Os exercícios começam bem simples e vão dificultando conforme você vai aprendendo novos conceitos. <br />

Alguns exercícios vou escreve-los de forma que não fique tão explícito o que você tem que fazer para resolver o problema e sim o resultado esperado. <br />
Exemplo de exercício: <br />
Crie uma API que retorna uma exceção quando chamar o recurso base da API `localhost:porta/` <br />

Nesse caso você terá que inicializar um projeto Spring, podendo usar o [Spring initializr](https://start.spring.io/), baixar as dependencias do Web e subir na sua máquina local o projeto e ver se quando chama o recurso `localhost:8080/` está retornando uma exceção do servidor que foi levantado junto com o Spring. Porém a forma como você vai fazer tudo isso é transparente, entende? <br />



O Spring disponibiliza vários "recursos" para nós
 - Client Http(WebClient / RestTemplate)
 - Mensageria (Cloud Stream / Kafka)
 - Conexão com banco de dados (Jpa repositories / MongoDB )
 - Criação de API's (Controller)
 - Entre outros

A ideia dos exercícios é passar um pouco por cada um desses conceitos principais. Então o exercício é o seguinte, nós iremos criar uma API responsável por todo o "backend" de uma loja de pizzas. Ela vai gerenciar desde os pedidos de pizzas feito por um site até o acompanhamento de status(Pedido recebido, cozinhando, em rota de entrega, entregue) etc... Ao final de todo o projeto, nós teremos a conclusão dessa API. Porém vamos começar com exercícios bem simples e ir incrementando aos poucos essa API, não precise se preocupar achando que será algo muito complexo, a ideia é começar bem simples.

[Curso Spring](https://www.youtube.com/watch?v=LXRU-Z36GEU)


## Exercícios

1. Criar um projeto spring e subir localmente e chamar localhost/ pra ver se subiu mesmo
2. Criar uma classe @Service e colocar system.out.println() no construtor para ver que o spring cria a classe
3. Criar o recurso GET /orders, que retorne "hello world"
4. Criar o recurso POST /orders, que recebe um objeto abaixo e retorna "Hello, 5 CHEESES"
```
{"flavour" : "5 CHEESES"}
```
5. Salvar no banco de dados o valor enviado para POST /orders
6. No recurso POST /orders, alterar o atributo flavour para flavours e receber uma lista de string. (Essa modificação deve refletir no banco de dados também)
7. Criar o recurso GET /orders que retorne todas as **orders** salvas no banco de dados
8. Ajustar o POST /orders para retornar um atributo chamado `location` no response header com o valor do id gerado no momento de salvar uma **order** no banco.
9. Ajustar o POST /orders, quando for salvar a **order** no banco, adicionar o atributo `status` com o valor `REQUESTED`
10. Criar o recurso GET /orders/id que retornará a order específica por id
11. Criar o recurso PATCH /orders/id que recebe o objeto abaixo e atualiza o status da order no banco
```
{"status":"COOKING"}
Possíveis status: REQUESTED / COOKING / DELIVERING / DELIVERED
```

