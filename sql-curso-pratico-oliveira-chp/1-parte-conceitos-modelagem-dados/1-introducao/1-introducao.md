# Introdução

- um sistema é feito para aceitar entrada de dados, realizar processamentos e gerar saídas das informações processadas e com o tempo verificou-se a necessidade de armazenar as informações geradas e aliado com a recuperação dessas informações passaram a passar um papel fundamental em processamento de informções.

- Em junho de 1970, Edgard Frank Codd (https://pt.wikipedia.org/wiki/Edgar_Frank_Codd) publicou um trabalho intitulado "A Relational Model of Data for Large shared Data Banks" (Um Modelo Relacional de Dados para Grandes Bancos de Dados Compartilhados), onde estabeleceu princípios sobre gerência de banco de dados, denominando-os com o termo relacional, sendo a base  utilizada na criação de uma linguagem-padrão para manipular informção em Banco de Dados Relacionais.  E essa linguagem é a SQL (Structure Query Language), inicialmente chamada de SEQUEL.

A linguagem foi concebida e desenvolvida pela IBM utilizando os conceitos de Codd e, em 1979, a Relational Software Inc., hoje Oracle Corporation, lançou a primeira versão comercial da linguagem.  Ao longo do tempo a linguagem vem sendo padronizada - pela ANSI e ISO.  O primeiro padrão (SQL-86) foi definido pela ANSI em 1986 e consistia basicamente na SQL da IBM, sendo esse padrão também adotado pela ISO, em 1987.  Em 1989, surge uma nova versão (SQL-89), com significativas modificações, sendo essa versão utilizada pelos bancos de dados atuais.  Em 1992, surge nova versão aprimorando a anterior, SQL-92, definindo as regras básicas para os bancos de dados relacionais.  Em 1999, surge a SQL-99, também conhecida como SQL-3, definindo um modelo de banco de dados objeto-relacional.

Divide-se o padrão SQL-92 em quatro níveis:  Entry (básico), Transational (em evolução), Intermediate (intermediário) e Full (completo).

# O que é SQL
É um conjunto de comandos de manipulação de banco de dados utilizado para criar e manter a estrutura desse banco de dados, além de incluir, excluir, modificar e pesquisar informações nas tabelas, não sendo uma linguagem de programação autônoma, podendo ser chamada de "sublinguagem".  Isto quer dizer que quando se escrevem aplicações  para banco de dados, é necessário utilizar uma linguagem de programação tradicional (C, Java, Pascal, COBOL, etc) e embutir comandos SQL para manipular dados.

SQL não é procedural, sendo possível especificar o que deve ser feito, e não como deve ser feito, assim, atingido um conjunto de linhas (set) por um comando e não cada uma das linhas. como é feito no ambiente procedural, não sendo necessário entender o funcionamento interno do banco de dados e como e onde estão armazenados fisicamente os dados.

É dividida nos seguintes componentes:
- DDL (Data Definition Language): permite a criação dos componentes de banco de dados, como tabelas, índices, etc.
-- CREATE TABLE;
-- ALTER TABLE;
-- DROP TABLE;
-- CREATE INDEX;
-- ALTER INDEX;
-- DROP INDES;

- DML (Data Manipulation Language):  permite a manipulação dos dados armazenados no banco de dados.
-- INSERT;
-- DELETE;
-- UPDATE;

- DQL (Data Query Language): permite extrair dados do banco de dados.
-- SELECT;

- DCL (Data Control Language): provê a segurança interna do banco de dados
-- CREATE USER;
-- ALTER USER;
-- GRANT;
-- REVOKE;
-- CREATE SCHEMA;

Com o advento da SQL-99, a linguagem passou a incorporar comandos procedurais (BEGIN, IF, funções, procedimentos) que, na prática, já existiam como extensões da linguagem.  Essas extensões são específicas de cada banco de dados, portanto a Oracle tem a sua própria linguagem procedural que estenda a SQL, que é a PL/SQL.  A Microsoft incorporou no SQL Server o Transact-SQL com o mesmo objetivo.

# NOTA DE IA

Dissertação sobre a Linguagem SQL e sua Evolução
A linguagem SQL (Structured Query Language) é um dos pilares fundamentais dos sistemas de gerenciamento de bancos de dados relacionais (SGBDR). Sua concepção e desenvolvimento estão intimamente ligados aos trabalhos teóricos de Edgar F. Codd, que em 1970 publicou um artigo seminal definindo o modelo relacional para armazenamento e recuperação de dados. A IBM, baseando-se nesses conceitos, desenvolveu a primeira implementação prática da linguagem, inicialmente chamada SEQUEL (Structured English Query Language), que mais tarde evoluiu para o SQL que conhecemos hoje.

O Surgimento do SQL Comercial e a Padronização
Em 1979, a Relational Software Inc. (que mais tarde se tornaria a Oracle Corporation) lançou a primeira versão comercial do SQL, marcando o início da adoção em larga escala da linguagem. A partir daí, outras empresas, como IBM, Microsoft (com o SQL Server) e a comunidade open-source (com sistemas como MySQL e PostgreSQL), passaram a implementar suas próprias versões do SQL, cada uma com particularidades, mas seguindo os mesmos princípios fundamentais.

Para garantir interoperabilidade entre os diferentes sistemas, foi necessário estabelecer padrões. A ANSI (American National Standards Institute) publicou o primeiro padrão oficial em 1986, conhecido como SQL-86, que basicamente refletia a implementação da IBM. Em 1987, a ISO (International Organization for Standardization) também adotou esse padrão, consolidando o SQL como uma linguagem universal para bancos de dados relacionais.

Evolução dos Padrões SQL
SQL-89 (ANSI/ISO):

Introduziu pequenas melhorias em relação ao SQL-86, principalmente em questões de integridade referencial.

Muitos bancos de dados atuais ainda utilizam conceitos dessa versão como base.

SQL-92 (Padrão Consolidado):

Foi um marco na padronização, definindo regras mais claras para operações em bancos de dados relacionais.

Dividiu-se em quatro níveis de conformidade:

Entry (Básico): Requisitos mínimos para um SGBD ser considerado compatível.

Transitional (Em Evolução): Um estágio intermediário entre Entry e Intermediate.

Intermediate (Intermediário): Inclui suporte a joins mais complexos, operações avançadas e maior integridade.

Full (Completo): Implementação total do padrão, raramente alcançada na prática devido à complexidade.

A maioria dos bancos de dados modernos segue pelo menos o nível Intermediate.

SQL-99 (SQL-3 – Modelo Objeto-Relacional):

Introduziu suporte a tipos de dados complexos, triggers, recursividade e programação procedural.

Trouxe conceitos de orientação a objetos, permitindo estruturas mais flexíveis.

Impacto e Legado
O SQL revolucionou a forma como os dados são armazenados e consultados, tornando-se uma linguagem ubíqua em sistemas corporativos. Apesar do surgimento de bancos de dados NoSQL para cenários específicos (como Big Data e sistemas distribuídos), o SQL permanece como a principal linguagem para bancos de dados relacionais, sendo essencial para áreas como análise de dados (BI), machine learning e desenvolvimento de software.

Conclusão
A evolução do SQL reflete a necessidade contínua de padronização e adaptação às novas demandas de armazenamento e processamento de dados. Desde sua criação na IBM até os padrões atuais (como SQL:2016 e SQL:2019), a linguagem continua a se desenvolver, incorporando funcionalidades como JSON, machine learning e processamento em tempo real. Portanto, o SQL não apenas resistiu ao teste do tempo, mas também se mantém como uma ferramenta indispensável no mundo da tecnologia da informação.

Qual o padrão mais utilizado atualmente e qual nível.
Atualmente, o padrão SQL mais amplamente adotado pelos sistemas de gerenciamento de banco de dados (SGBDs) é o SQL:2016 (também conhecido como ISO/IEC 9075:2016), com alguns já suportando parcialmente o SQL:2019. No entanto, a maioria dos bancos de dados comerciais e open-source ainda se baseia fortemente no SQL:92 e SQL:1999, pois esses padrões estabeleceram os fundamentos essenciais da linguagem (como JOINs, subconsultas, transações e stored procedures).

Nível de Conformidade Mais Comum (SQL-92)
Embora o SQL tenha evoluído para versões mais recentes (SQL:1999, SQL:2003, SQL:2008, SQL:2011, SQL:2016, SQL:2019), muitos SGBDs ainda não implementam completamente os padrões mais novos, optando por seguir um subconjunto do SQL-92 no nível Intermediate, que inclui:

Consultas complexas (subconsultas, múltiplos JOINs, GROUP BY, HAVING).

Controle de transações (COMMIT, ROLLBACK, SAVEPOINT).

Restrições de integridade (chaves primárias, estrangeiras, CHECK).

Funções agregadas (SUM, AVG, COUNT, MAX, MIN).

Por que o SQL-92 ainda é tão relevante?
Estabilidade e Maturidade: O SQL-92 definiu as operações fundamentais usadas até hoje.

Compatibilidade: Bancos de dados como Oracle, PostgreSQL, MySQL e SQL Server garantem compatibilidade retroativa.

Complexidade dos Padrões Recentes: SQL:2016 e SQL:2019 adicionam recursos avançados (como JSON, temporal tables e machine learning), mas muitos projetos não exigem esses recursos.

Adoção de Padrões Recentes
SQL:2016 trouxe suporte a JSON, polimorfismo e padrões de tempo (temporal tables).

PostgreSQL e MySQL já implementam parcialmente JSON.

Oracle e SQL Server têm suporte a temporal tables.

SQL:2019 introduziu grafos e mais operações analíticas, mas ainda está em adoção gradual.

Conclusão
O nível Intermediate do SQL-92 ainda é o mais utilizado na prática, pois cobre a maioria das necessidades de bancos de dados relacionais. Enquanto isso, os padrões mais recentes (SQL:2016/2019) são adotados parcialmente, conforme a demanda por funcionalidades avançadas cresce.

Se você está aprendendo SQL, focar no SQL-92 (nível Intermediate) e em extensões práticas do seu SGBD (como PL/SQL na Oracle ou T-SQL no SQL Server) é a melhor abordagem.

### **Análise: SQL-99 e as Extensões Procedurais em Bancos de Dados**

A introdução do padrão **SQL-99 (SQL-3)** representou um marco importante na evolução da linguagem SQL, pois **formalizou recursos procedurais** que, até então, eram implementados de forma proprietária pelos principais sistemas de banco de dados. Essa mudança refletiu a necessidade de tornar o SQL mais **poderoso e flexível**, permitindo a criação de lógica complexa diretamente no banco de dados.

#### **1. SQL-99 e a Incorporação de Comandos Procedurais**
Antes do SQL-99, a SQL era uma linguagem **declarativa**, focada principalmente em consultas e manipulação de dados. No entanto, muitos SGBDs já haviam desenvolvido **extensões procedurais** para permitir:
- **Controle de fluxo** (IF, ELSE, LOOP).
- **Blocos de código** (BEGIN...END).
- **Funções e procedimentos armazenados** (STORED PROCEDURES, FUNCTIONS).

O **SQL-99 padronizou esses conceitos**, incluindo:
- **SQL/PSM (Persistent Stored Modules)** → Define estruturas para programação procedural.
- **Triggers** → Permite ações automáticas baseadas em eventos.
- **Recursividade** (WITH RECURSIVE).

#### **2. Extensões Proprietárias Antes do SQL-99**
Antes dessa padronização, cada banco de dados já tinha sua própria linguagem procedural:
- **Oracle → PL/SQL** (Procedural Language/SQL):
  - Surgiu antes do SQL-99, inspirado em Pascal e Ada.
  - Suporta estruturas complexas, exceções e cursores.
- **Microsoft SQL Server → T-SQL (Transact-SQL):**
  - Extensão da SQL com elementos procedurais, como variáveis e fluxo condicional.
- **PostgreSQL → PL/pgSQL:**
  - Similar ao PL/SQL, mas com algumas diferenças de sintaxe.

#### **3. Impacto da SQL-99 nas Extensões Procedurais**
Apesar da padronização, **as implementações continuaram sendo específicas de cada SGBD** porque:
- **Legado**: Muitos sistemas já usavam extensões proprietárias antes do SQL-99.
- **Otimizações**: Cada banco adapta a linguagem para seu motor de execução.
- **Recursos extras**: PL/SQL, T-SQL e PL/pgSQL adicionam funcionalidades além do padrão.

#### **4. Conclusão**
O **SQL-99 trouxe uma base comum para programação procedural**, mas **não eliminou as variações proprietárias**. Hoje, temos:
- **Padrão SQL/PSM** → Teoricamente universal, mas pouco adotado na prática.
- **Extensões proprietárias** (PL/SQL, T-SQL, PL/pgSQL) → Dominam o mercado por oferecerem melhor integração com seus respectivos bancos.

**Para desenvolvedores:**
- Se você trabalha com **Oracle**, precisa aprender **PL/SQL**.
- Se usa **SQL Server**, deve dominar **T-SQL**.
- Bancos como **PostgreSQL** seguem o **PL/pgSQL**, mas também suportam outras linguagens (Python, JavaScript via PL/V8).

Apesar das diferenças, o **core SQL permanece consistente**, e entender a lógica procedural (seja via padrão SQL-99 ou extensões) é essencial para desenvolvimento avançado em bancos de dados.
