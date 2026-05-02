# **1 - O que é um banco de dados: diferença de bancos relacionais e não relacionais**

- O que são Banco de Dados:
    
    Um sistema projetado para organizar, armazenar e gerenciar dados de maneira eficiente, facilitando o acesso, a gestão e a atualização dessas informações.
    
- O que são banco de dados relacionais?
    - Estrutura bem definida e tabelas com relações entre si.
    - Ideal para dados estruturados e relacionamentos complexos.
    - Exemplos de banco: mySQL, PostgreSQL, Oracle
- O que são banco de dados não relacionais?
    - Estrutura mais flexível e podem lidar com dados não estruturados.
    - Ideal para grandes volumes de dados não estruturados e alta escalabilidade.
    - Exemplos de banco: MongoDB, Cassandra, Redis
- Como os bancos relacionais organizam os dados de maneira eficiente?
    - Através de estruturas tabulares, onde os dados são organizados em tabelas com linhas e colunas.
    - Cada tabela representa uma entidade (tipo de informação) e cada linha representa uma instância (registro) dessa entidade.
    - As colunas representam os atributos (características) de cada entidade.

---

# **2 - Entidades e Relacionamentos**

- **O que são relacionamentos entre tabelas?**
    - A forma como as tabelas se conectam e "conversam" em um banco de dados.
- Tipos de relacionamentos:
    
![img/Captura de Tela 2026-04-30 às 22.13.32.png]()
    
- **1 para 1 (1:1):** Cada uma das duas entidades envolvidas referenciam obrigatoriamente apenas uma unidade da outra.
    - Ex: Cada pessoa tem apenas uma carteira de identidade.
- **1 para muitos (1:N) ou Muitos para 1 (N:1):** Uma das entidades envolvidas pode referenciar várias unidades da outra, porém, do outro lado cada uma das várias unidades referenciadas só pode estar ligada uma unidade da outra entidade
    - Ex: Um álbum pode ter várias músicas, mas cada música pertence a apenas um álbum (1:N) ou Várias músicas podem pertencer a um único álbum (N:1).
- **Muitos para muitos (N:N):** Neste tipo de relacionamento cada entidade, de ambos os lados, podem referenciar múltiplas unidades da outra
    - Ex: Um cliente pode comprar vários álbuns, e um álbum pode ser comprado por vários clientes.
    
![img/Captura de Tela 2026-04-30 às 22.11.33.png]()
    
- O que são diagramas de entidade e relacionamento?
    - É uma representação gráfica das relações entre as tabelas, facilita muito a compreender o que tem no banco e como essas entidades estão se relacionando.
        - Representado por retângulos (tabelas) e linhas que as conectam (relacionamentos).
        - Símbolos especiais indicam o tipo de relacionamento (1:1, 1:N, N:1, N:N).
- Chave primária e estrangeira
    - As chaves indicam quais os campos que representam e conectam as tabelas.
        - **Chave primária:** O "RG" da tabela, um identificador único para cada linha.
        - **Chave estrangeira:** Campo que identifica qual o registro de uma tabela terceira está sendo associado naquela tabela. É o que permite que você conecte as informações de diferentes tabelas em um banco de dados relacional. Isso facilita a busca e organização dos dados.

---

# **3 - Conhecendo SQL (parte 1 e 2)**

- O que é SQL?
    - SQL (Structured Query Language) é a linguagem padrão para gerenciar e manipular dados em bancos de dados relacionais.
    - Imagine o SQL como um tradutor mágico que permite conversar com o banco de dados, extraindo e organizando informações.
- Tipos de Comandos SQL (DDL, DML, DCL)
    - **DDL (Data Definition Language):** Linguagem de Definição - Cria, modifica e exclui tabelas no banco de dados.
        - Ex: CREATE TABLE, ALTER TABLE, DROP TABLE
    - **DML (Data Manipulation Language):** Linguagem de Manipulação - Insere, atualiza, consulta e remove dados das tabelas.
        - Ex: SELECT, INSERT, UPDATE, DELETE
    - **DCL (Data Control Language):** Linguagem de Controle - Controla permissões de acesso e segurança no banco de dados.
        - Ex: GRANT, REVOKE
- O que são queries?
    - Comando de instrução do SQL
    - Uma pergunta que fazemos ao banco de dados para obter informações especificas ou realizar operações dentro do banco.