# Trabalhando com API`s

- Aprendemos sobre API´s, porque esse recursos nos ajuda a trocar informações entre sistemas seja do mesmo servidor até sistemas de onde não temos acesso. 
    - Ex: Logar com uma conta do google em um site ou jogo que não envolve o google.
    - Pagamento de Terceiros: Quando você acessa um site com seus dados e aparece que o pagamento será feito por um banco. Esse sistema do site pegar suas informações e se conectar com outro sistema é feito por uma API.
- API´s servem para estruturar qualquer aplicação web para os dias de hoje, tendo como principal característica a troca de informações entre apps, sites e afins de forma padronizada.

## Conceito de API

> Application Programming Interface, ou seja, é uma aplicação voltada ao intermédio de sistemas, possibilitando diversas conexões, por meio de uma série de padrões e protocolos. Além disso, ela é criada por uma empresa, geralmente, quando a organização tem a intenção de que outros softwares usufruam de seus serviços. 

- Analogia do Restaurante
    - Chamamos o garçon e fazemos o pedido, porque nós não podemos ir diretamente até a cozinha e fazer isso.
    - Então, ele vem a mesa, anota o pedido e leva até a cozinha.
    - A cozinha tem a responsabilidade de preparar o pedido.
    - Quando a comida estiver pronta o chefe vai avisar o garçon que trás o pedido a nossa mesa.
- Explicação da Analogia 
    - Clientes: Usuários
    - Mesa: Front-End, aplicação que conversa com o usuário.
    - Garçon: API, recebe o pedido do front, manda pro back e após recber os dados entrega para o front. (não tem influência de como os dados serão tratados)
    - Cozinha: Back-End, aplicação que conversa com o servidor/sistema externo. Vai preparar os dados.

## JSON

É um formato de arquivo leve para organizar seus dados, no qual, independente da linguagem, os seres humanos conseguem ler e as máquinas conseguem gerar.

```json
{
    "nome":"Samara Silvia",
    "idade": 19,
    "cidade": "Recife",
    "filmes_favoritos" : [
        "A Cabana",
        "Os vingadores",
        "A 5 passos de você"
    ],
    "hobbies":{
        "semana": "leitura",
        "fim_de_semana": {
            "sabado": "cinema",
            "domingo": "park",
            "outros": [
                "caminhada",
                "netflix",
                "natação"
            ]
        }
    }
}
```

- Ele sempre começa com { } e é composto por chaves e valores, ambos marcados com "".
- Armazena qualquer tipo de dado: String; Number; Object; Array...


## Métodos HTTP

Os 5 principais métodos ou verbos HTTP são:

- `Get:` A API fornece informações. Precisa devolver dados;
    - Ex: https://api.github.com/users/samarasilvia81 - Sempre que passamos informações
- `Post:` A API recebe informações que devem ou não serem registradas;
    - Quando criamos um repositório, preenchemos as informações e enviamos do front do git para o back do git.
- `Put:` A API recebe informações para update de um ou mais registros;
    - Ao acessar https://api.github.com/users com todos os usuários do git e colocamos na porta put + dados, o git vai atualizar esses dados.
- `Patch:` A API recebe informações para update de um registro;
    - Ao acessar https://api.github.com/users com todos os usuários do git e colocamos na porta put + dado, o git vai atualizar esse dado (apenas um único registro).
- `Delete:` A API recebe identificadores de registros que devem ser apagados;
    - Ao acessar https://api.github.com/users com todos os usuários do git e colocamos na porta delete + identificador, ele automaticamente irá deletar este dado.


## Insominia

É um programa para fazer as requisições como post, put...








## Referências

- https://json.org/json-pt.html
- https://www.w3schools.com/whatis/whatis_json.asp