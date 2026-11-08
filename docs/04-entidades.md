# 04 — Identificação das Entidades

## 1. Introdução

As entidades representam os principais objetos do minimundo que precisam ter seus dados armazenados no banco de dados. No BookVerse, elas correspondem aos elementos envolvidos no gerenciamento do acervo, dos leitores, dos empréstimos e das atividades de leitura.

## 2. Entidades identificadas

### 2.1 Leitor

Representa as pessoas cadastradas que utilizam os serviços da biblioteca. Seus dados permitem identificar os usuários, controlar empréstimos e registrar históricos de leitura e avaliações.

### 2.2 Publicação

Representa as obras disponíveis no catálogo, incluindo livros, HQs, mangás e graphic novels. Armazena informações bibliográficas, como título, ISBN, ano, idioma e descrição.

### 2.3 Exemplar

Representa cada cópia física de uma publicação. É necessário para controlar individualmente a disponibilidade e a situação de cada unidade do acervo.

### 2.4 Autor

Representa as pessoas responsáveis pela criação dos textos ou histórias das publicações. Permite identificar e relacionar os autores às obras cadastradas.

### 2.5 Ilustrador

Representa os profissionais responsáveis pelas ilustrações das publicações. É especialmente relevante para HQs, mangás e graphic novels.

### 2.6 Editora

Representa as empresas responsáveis pela publicação das obras. Seus dados permitem organizar as informações bibliográficas e consultar publicações por editora.

### 2.7 Gênero

Representa a classificação temática das publicações, como fantasia, romance, terror, suspense e ficção científica.

### 2.8 Coleção

Representa conjuntos de publicações relacionadas, como séries de livros, coleções de HQs e sequências de mangás.

### 2.9 Empréstimo

Representa a operação de retirada de um exemplar por um leitor. Armazena as datas de retirada, previsão de devolução e retorno efetivo.

### 2.10 Bibliotecário

Representa o funcionário responsável pelas atividades operacionais, como cadastros, empréstimos e devoluções.

### 2.11 Acompanhamento de Leitura

Representa o registro do progresso de leitura de uma publicação por determinado leitor. Armazena o estado da leitura, as datas e a quantidade de páginas ou capítulos lidos.

### 2.12 Avaliação

Representa a opinião de um leitor sobre uma publicação, armazenando notas e resenhas.

### 2.13 Administrador

Representa o responsável pelo gerenciamento geral do sistema, incluindo usuários, permissões e configurações.

### 2.14 Gerente da Biblioteca

Representa o responsável por acompanhar os indicadores e consultar relatórios para apoiar decisões relacionadas ao funcionamento da biblioteca.

## 3. Observações sobre a organização das entidades

Algumas entidades possuem relacionamentos que precisam ser considerados na modelagem:

- Uma publicação pode possuir vários exemplares físicos.
- Uma publicação pode estar relacionada a vários autores, e um autor pode participar de várias publicações.
- Uma publicação pode possuir vários ilustradores, e um ilustrador pode trabalhar em várias publicações.
- Um leitor pode realizar vários empréstimos ao longo do tempo.
- Um empréstimo está associado a um leitor e a um exemplar.
- Um leitor pode acompanhar várias publicações.
- Uma publicação pode receber avaliações de diferentes leitores.

Para representar corretamente os relacionamentos de muitos para muitos, poderão ser utilizadas entidades associativas, como `Publicacao_Autor` e `Publicacao_Ilustrador`.

## 4. Considerações finais

A identificação das entidades estabelece a base para a construção do modelo conceitual e lógico do BookVerse. A partir delas, será possível definir atributos, chaves primárias, chaves estrangeiras e cardinalidades, garantindo uma estrutura organizada e coerente para o banco de dados.