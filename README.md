# Teste de DEV Backend

Este projeto é a base para os testes básicos de desenvolvedores para ingresso no grupo de trabalho de backend do PAIMLAB

# Instruções Básicas

- Leia o arquivo de texto *PADROES DE DESENVOLVIMENTO DE PROJETO.doc* (Versão 1.0) e tenha ele como padrão para a entrega
-- É importante salientar que este documento é versionado conforme novas práticas são adotadas pela equipe, portanto a versão a qual estava ativa no momento da criação do repositório será considerada a versão válida.
- Crie um projeto no GIT de sua preferência com o conteúdo deste GIT
- Crie uma branch para cada implementação de feature, segindo o conceito de *git flow*
- Faça o commit de cada implementação de forma separada.
    - Isto é MUITO importante: o tempo que você demorou para implementar cada feature será avaliado considerando o horário de criação da branch e do deploy desta no GIT. Não "faça todo o deploy de uma vez" ou a tarefa esta será desconsiderada durante a avaliação. Caso você precise "parar a tarefa" em algum ponto faça o commit e, após ele, crie novas branchs de implementação dentro da branch de feature para dar continuidade na linha do tempo e siga o flow para implementação das mesmas.
- Para o deploy do banco de dados utilize a pasta chamada SQL, salvando nela os arquivos de deploy do banco de dados utilizando no nome a data e hora de criação do arquivo para se ter como referência para a ordem de implementação.
    - Considere que tabelas relacionais que dependem de chaves estrangeiras devem ser importadas em uma ordem correta.
    - Se você conhecer o conceito de Migrations e Seeds pode utilizá-lo dentro da estrutura padrão do CodeIgniter
- O uso das seguintes ferramentas é obrigatório:
    - Bootstrap
    - jQuery
    - Requisições em Ajax
    - jQuery DataTables
    - jQuery Select2

#Estrutura do Projeto

Leia com atenção o escopo abaixo e aplique-o:

- Crie uma estrutura simples de banco de dados com as seguintes tabelas:
    - Usuários (id, nome, cpf)
    - Unidades (id, nome, telefone)
    - Setores (id, nome)
    - Usuários das Unidades (relacional entre usuários e unidades)
    - Usuários das Setores (relacional entre usuários e setores)
- Crie um CRUD para Unidades
- Crie um CRUD para Usuários, onde:
    - O Usuário **deve** estar relacionado à uma Unidade
    - O Usuário **pode** estar relacionado à mais de um Setor
    - Na listagem de Usuários devem aparecer o Nome, as Unidades e Setores de cada Usuário cadastrado em colunas específicas

# Detalhes importantes:

- Existe no arquivo index.php@Linha 97 existe uma função customizada para debug. Use e abuse, se quiser copie para você.
- **JAMAIS** publique o resultado de seu teste neste repositório do GITLAB, utilize um criado por você
- Quando terminada a tarefa envie o acesso ao GIT para o e-mail desenvolvimento@paim.com.br
    - Este acesso deve ser um GIT público. Serão analisados os commits e tempo de execução entre os mesmos.