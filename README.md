# Database
Estudo sobre Banco de Dados

Banco de dados
Sistemas:
MySQL
SQL Server
Microsoft Access
Quando se lida com banco de dados, temos que ter em mente os problemas
em potencial.
Considerações
Tamanho
Por que isso seria um problema?
-Planilhas tem limites, ele foi projetado para volume.

Atualizações
O que acontece se dois usuários diferentes tentar alterar o mesmo
telefone da mesma pessoa, ao mesmo temo?
- Se você trabalha com sistemas baseados em arquivos, isso é
muito problemático

Precisão
Tipos de dados – informações consistentes
- Tudo isso é para garantir que os dados sejam coerentes, com o
tipo de informação que você deseja armazenar.

Segurança
Sigilo de informações – Acesso parcial – Controle de permissão – Histórico de
Alterações
Redundância
Duplicação de dados
Ter isso de certa forma é bom por conta de backups, ou copias de
segurança, mas os dados em si não são tão bons, pois, você pode gerar
conflito ou incertezas sobre o valor correto.

Importância
Tipo de informação – relevância – Dependência.

Banco de Dados
Gerenciar grandes volumes de dados

Transformar dados em informações uteis
Manter dados atualizados por vários usuários
Garantir precisão e consistência dos dados.

Banco de Dados
Informações estruturadas
Múltiplas tabelas
Relacionamentos de tabelas – baseado em regras que você define.
Esse conjunto é chamado de:
Esquema do banco

Também conseguimos criar regras para cada campo por ex:
tipo de dados
proteção de dados
exibição parcial

SGDB:
Oracle
SQL Server
MySQL
DB2
PostgreSQL
MongoDB
Esses sistemas são basicamente Softwares que permite que você crie um ou mais banco de
dados. Com uma interface gráfica um pouco mais amigável do que os comandos de textos que
ainda existem por aí.

Os tipos e sistemas mais comuns:
Relacional RDBMS esse é o mais comum, que organiza os dados em tabelas
Hierárquico
Rede
Orientado a Objetos
NoSQL

Banco de dados relacionais:

- Em um banco de dados relacional agrupamos informações em uma tabela, essa
tabela é composta de linhas e cada linha representa um item ou um registro, cada
coluna representa um atributo do registro.
Exemplo: Um restaurante.
- Em um banco de dados de um restaurante temos uma tabela para armazenar as
informações dos clientes, nessa tabela cada cliente é uma entidade e cada entidade
ocupa uma linha nessa tabela, cada linha representa um cliente diferente, mas todos
compartilham a condição de ser um cliente. Cada cliente individual é uma instância de
uma entidade chamada “cliente”, e como clientes eles compartilham certos atributos e
propriedades que os descrevem. Exemplo: (nome, número, e-mail etc.).
Além da tabela de clientes, também tem a tabela com os itens do cardápio, nesse
caso, o item do cardápio é a entidade. Cada instância do cardápio é uma instância ou
registro, e cada item no cardápio tem atributos específicos. Exemplo: (nome,
descrição, preço do item). Esses itens e os clientes são mantidos em tabelas separadas
em um banco de dados, porque são entidades diferentes, e contêm informações
diferentes. Exemplo: “Os itens do cardápio não têm números de telefone, e as pessoas
não têm preço.”
Temos uma terceira tabela para os itens favoritos dos clientes. Um nome é composto
das tabelas que ela une, seguido de uma descrição se necessário. Nessa terceira tabela
está relacionando a tabela clientes com a tabela itens do cardápio. O item favorito é a
entidade ou registro, que é composto do nome do cliente e um item de cardápio, ou
seja, essa tabela relaciona um item de uma tabela com um ou mais itens de outra.
Tipos de relacionamentos:
- Existem 3 tipos de relacionamentos utilizados em um banco de dados.
. Um-para-muitos
. Muitos-para-muitos
. Um-para-um
- Um-para-muitos - É de longe o relacionamento mais comum. Ele associa um registro
em uma tabela com vários registros em outra tabela, um-para-muitos. Exemplo do
restaurante: “Um cliente pode ter mais de um prato favorito, ou seja, existe uma
relação de um cliente para vários itens favoritos”.
- Muitos-para-muitos - Ocorre quando vários registros em uma tabela são associados a
vários registros em outra tabela. Ex: “Um relacionamento muitos-para-muitos existe
entre clientes e produtos: clientes podem comprar vários produtos e produtos podem
ser comprados por muitos clientes”.
- Um-para-um - Ao contrário de um relacionamento um-para-muitos, um
relacionamento um-para-um associa apenas um registro em uma tabela ou apenas um
registro em outra tabela, de forma que o registro de destino não possa ser associado a
outro registro ao mesmo tempo.
- Nos relacionamentos há um conceito fundamental, tanto para pensar sobre seus
dados, quanto para recuperá-los mais tarde.

Modelagem de banco de dados:
- Modelagem de banco de dados é o processo de levantamento, análise, categorização
e exploração de todos os dados e tipos de informações que irão sustentar uma
aplicação. Esta é uma etapa primordial no trabalho do desenvolvimento de sistemas,
porque todo software é criado com determinados objetivos, para atender às
necessidades dos usuários dentro deste cenário.
Se um sistema for desenvolvido sem que haja uma modelagem de banco de dados
bem executada no início do projeto, as chances de ele apresentar falhas ou até mesmo
de não suprir os objetivos para os quais foi criado são grandes.

➔ Otimizações e Gerenciamento:
- Índices: Índices são identificações que ajudam a tornar a consulta a um dado do
banco muito mais rápida.
- Procedimentos armazenados: É um conjunto de transações armazenadas no servidor
do banco de dados. Ele contém uma série de comandos que você precisa referenciar e
usar ao interagir com banco de dados. Usando um procedimento armazenado, você
evita de fazer consultas longas e detalhadas toda vez que precisar de um relatório.
Os procedimentos armazenados também são usados para fornecer maneiras seguras
ou aprovadas de lidar com dados confidenciais.
Em vez de permitir o acesso aos dados diretamente do SQL inserido manualmente,
que pode conter erros, um administrador de banco de dados geralmente fornece um
conjunto de procedimentos armazenados, projetados para obter determinadas
informações de usuário. Na qual é uma boa ideia permitir acesso a dados confidenciais
somente através de procedimentos armazenados, e não diretamente via SQL.
