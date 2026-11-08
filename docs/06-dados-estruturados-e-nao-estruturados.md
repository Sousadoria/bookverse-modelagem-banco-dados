# 06 — Dados Estruturados e Não Estruturados

## 1. Introdução

O BookVerse precisará armazenar diferentes tipos de dados para gerenciar as publicações, os leitores e as atividades da biblioteca.

Os dados estruturados possuem formato padronizado e previsível, sendo organizados em campos e tabelas. Já os dados não estruturados não seguem um padrão rígido de conteúdo, podendo incluir textos livres e arquivos de imagem.

## 2. Exemplos de dados estruturados

| Exemplo de dado | Classificação | Justificativa |
|---|---|---|
| Nome, CPF, e-mail e telefone de um leitor. | Estruturado | São informações organizadas em campos específicos na tabela de leitores, permitindo consultas e validações. |
| ISBN, título, ano de publicação e idioma de uma obra. | Estruturado | São dados bibliográficos com campos definidos, que podem ser armazenados em colunas de uma tabela de publicações. |
| Data de retirada e data prevista para devolução. | Estruturado | São valores armazenados em campos do tipo data, permitindo comparações e consultas. |
| Nota atribuída por um leitor. | Estruturado | É um valor numérico limitado a uma escala predefinida de 1 a 5 estrelas. |
| Quantidade de páginas lidas. | Estruturado | É um valor numérico que pode ser armazenado em um campo específico e utilizado no cálculo do progresso de leitura. |

## 3. Exemplos de dados não estruturados

| Exemplo de dado | Classificação | Justificativa |
|---|---|---|
| Texto de uma resenha escrita por um leitor. | Não estruturado | É um conteúdo textual livre, no qual o leitor expressa sua opinião sem seguir um formato fixo. |
| Descrição ou sinopse de uma publicação. | Não estruturado | É um texto descritivo que pode variar em tamanho, linguagem e organização. |
| Capa de um livro, mangá ou HQ. | Não estruturado | É um arquivo de imagem composto por elementos visuais, que não podem ser organizados diretamente em campos convencionais de uma tabela. |
| Fotografia de uma publicação danificada. | Não estruturado | É um arquivo de imagem utilizado para documentar visualmente o estado físico de um exemplar. |
| Comentário de um leitor sobre sua experiência de leitura. | Não estruturado | É um texto livre, com conteúdo e extensão variáveis, sem um modelo rígido de preenchimento. |

## 4. Organização técnica dos dados

Os dados estruturados serão armazenados principalmente em tabelas relacionais, com campos definidos e tipos de dados apropriados, como texto, números, datas e identificadores.

Os dados não estruturados, como resenhas e sinopses, poderão ser armazenados em campos de texto apropriados no banco de dados. Já arquivos de imagem poderão ser mantidos em um repositório de arquivos, enquanto o banco de dados armazenará suas referências, como nomes ou caminhos dos arquivos.

Essa organização permitirá relacionar os conteúdos às respectivas publicações, leitores ou exemplares sem comprometer a estrutura principal do banco de dados.

## 5. Considerações finais

A identificação dos dados estruturados e não estruturados ajuda a definir como as informações deverão ser armazenadas e consultadas. A combinação desses formatos permitirá que o BookVerse mantenha registros administrativos organizados e também preserve conteúdos textuais e visuais relacionados às publicações e às experiências dos leitores.