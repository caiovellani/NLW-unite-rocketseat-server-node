# pass.in 

O pass.in é uma aplicação de **gestão de participantes em eventos presenciais**.

A ferramenta permite que o organizador cadastre um evento e abra uma página pública de inscrição.

Os participantes inscritos podem emitir uma credencial para check-in no dia do evento.

O sistema fará um scan de credencial do participante para permitir a entrada no evento. 

## Requisitos

### Requisitos funcionais

- [ ] O organizador deve poder cadastrar um novo evento;
- [ ] O organizador deve poder visualizar dados de um evento;
- [ ] O organizador deve poder visualizar a lista de participantes;
- [ ] O participante deve poder se inscrever em um evento;
- [ ] O participante deve poder visualizar seu crachá de inscrição;
- [ ] O participante deve poder realizar check-in no evento;

### Regras de negócio 

- [ ] O participante só pode se inscrever em um evento uma única vez;
- [ ] O participante só pode se inscrever em eventos com vagas disponíveis;
- [ ] O participante só pode realizar check-in em um evento uma única vez;

### Requisitos não-funcionais

- [ ] O check-in no evento será realizado através de um QRCode;

## Anotações 

Métodos HTTP: GET, POST, PUT, DELETE, PATCH, HEAD, OPTIONS, ...
GET => Retornar algo
POST => Criar algo
PUT => Atualizar algo
DELETE => Deletar algo
PATCH => Atualizar algo parcialmente
HEAD => Obter metadados
OPTIONS => Obter opções

Corpo da requisição (Request Body)
Parâmetros de busca (Search Params / QueryParams) `http://localhost:3333/users?search=Caio`
Parâmetros de rota (Route Params) -> Identificação de recursos `http://localhost:3333/users/1`
Cabeçalhos (Headers) -> Contexto da requisição 

Conectar ao banco de dados, 3 formas
Driver nativo / Query Builders / ORMs

Object Relational Mapping (Hibernate / Doctrine / ActiveRecord)

JSON -> JavaScript Object Notation

STATUS CODE 
20x -> Sucesso 
30x -> Redirecionamento
40x -> Erro do cliente (Erro em alguma informação enviada por QUEM está fazendo a chamada para a API)
50x -> Erro do servidor (Um erro que está acontecendo INDEPENDENTE do que está sendo enviado para o servidor)

slug -> titulo do evento na url `http://localhost:3333/events/nlw-unite` -> nlw-unite

'###' -> Separa as rotas. (api.http)
