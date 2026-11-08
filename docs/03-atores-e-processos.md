# 03 — Atores e Processos do Sistema

## 1. Atores do sistema

Os atores representam os perfis que interagem com o BookVerse e executam atividades dentro da biblioteca. Cada perfil possui responsabilidades e permissões específicas.

### 1.1 Administrador do Sistema

É responsável pelo gerenciamento geral da plataforma. Suas principais atividades são:

- Gerenciar usuários e níveis de acesso.
- Configurar permissões.
- Gerenciar parâmetros gerais do sistema.
- Consultar informações gerais dos cadastros.

### 1.2 Bibliotecário

É responsável pelas atividades operacionais da biblioteca. Suas principais atividades são:

- Cadastrar e atualizar publicações.
- Gerenciar autores, ilustradores, editoras, gêneros e coleções.
- Cadastrar e atualizar exemplares físicos.
- Cadastrar leitores.
- Registrar empréstimos e devoluções.
- Consultar a disponibilidade das publicações.

### 1.3 Leitor

É o usuário que utiliza os serviços da biblioteca e acompanha suas próprias atividades de leitura. Suas principais atividades são:

- Consultar o catálogo de publicações.
- Verificar a disponibilidade dos exemplares.
- Consultar seu histórico de empréstimos.
- Registrar o progresso de leitura.
- Atualizar o estado de suas leituras.
- Registrar notas e resenhas.

### 1.4 Gerente da Biblioteca

É responsável por acompanhar os resultados e indicadores da biblioteca. Suas principais atividades são:

- Consultar relatórios de empréstimos.
- Identificar publicações mais procuradas.
- Analisar os gêneros mais populares.
- Acompanhar informações sobre os hábitos de leitura.
- Utilizar os relatórios para apoiar decisões sobre o acervo.

## 2. Processos principais do sistema

### 2.1 Cadastro e gerenciamento do acervo bibliográfico

O processo começa quando o bibliotecário recebe uma publicação para inclusão no catálogo. Ele registra informações como título, ISBN, tipo de publicação, gênero, ano, idioma, editora, autores e ilustradores.

O sistema valida os campos obrigatórios, verifica possíveis duplicidades e organiza os relacionamentos entre as informações bibliográficas.

Após o cadastro da publicação, são registrados seus exemplares físicos individualmente, cada um com um identificador próprio e uma situação de disponibilidade.

O processo permite manter o catálogo atualizado e controlar as cópias existentes na biblioteca.

### 2.2 Cadastro de leitores, empréstimos e devoluções

O processo começa com o cadastro do leitor, no qual são registrados dados como nome, CPF, endereço, telefone e e-mail.

O sistema valida as informações e gera um identificador para o leitor.

Quando um empréstimo é solicitado, o bibliotecário verifica o cadastro do leitor e a disponibilidade do exemplar. O sistema também verifica se o leitor está ativo e se respeita o limite de empréstimos permitido.

Após as validações, o empréstimo é registrado com a data de retirada e a data prevista para devolução. O exemplar passa a ter a situação de emprestado.

Na devolução, o bibliotecário registra o retorno do exemplar. O sistema compara a data efetiva com a data prevista, identifica possíveis atrasos e atualiza a disponibilidade do exemplar.

### 2.3 Acompanhamento de leitura e registro de avaliações

O processo começa quando o leitor seleciona uma publicação e registra sua intenção de leitura.

Ele pode classificar a atividade como planejada, em andamento, concluída ou abandonada. Durante a leitura, pode atualizar o progresso por páginas ou capítulos.

O sistema valida os registros e calcula o percentual de progresso quando existe uma quantidade total de páginas ou capítulos cadastrada.

Ao finalizar uma publicação, o leitor pode registrar uma avaliação de 1 a 5 estrelas e escrever uma resenha.

Esses registros formam um histórico individual e podem ser utilizados para gerar relatórios sobre preferências e hábitos de leitura.

## 3. Considerações finais

A identificação dos atores e processos permite compreender como as informações circulam dentro do BookVerse. Essa etapa é importante para definir as responsabilidades de cada perfil, as operações realizadas e os dados necessários para a futura modelagem do banco de dados.