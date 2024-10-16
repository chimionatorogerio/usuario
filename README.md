<< Atualmente estou trabalhando no desenvolvimento desta aplicação no microsserviço  Agendador de tarefas >>

A principal função dessa aplicação será enviar para o usuário um lembrete das tarefas que ele agendou.

METODOLOGIA ÁGIL KANBAN
Vamos dividir a aplicação em quatro microsserviços. Para cada microsserviço, faremos uma lista de tarefas. O objetivo é melhorar a organização do projeto e agilizar o desenvolvimento da aplicação.

MICROSSERVIÇOS QUE PRECISAM SER DESENVOLVIDOS
1) Cadastro de usuários (concluído)
2) Agendador de tarefas
3) Notificação por email
4) BFF (Back-end For Front-end). Este padrão de arquitetura fará a intermediação entre os 3 primeiros microsserviços e o Front-end

CADASTRO DE USUÁRIOS - TAREFAS
Criar o banco de dados db_usuario no PostegreSQL (concluída)
Inicializar a aplicação usando o Spring Initializr (concluída)
Criar o repositório usuario no GitHub (concluída)
Configurar o CI/CD (concluída)
Configurar a segurança com Spring Security (concluída)
Criar método:
- Post para cadastrar usuários (concluída)
- Get para buscar usuários (concluída)
- Delete para excluir usuários (concluída)
- de login de usuário (concluída)
Criar métodos Put para alterar:
- Nome, email e senha (concluída)
- Endereços (concluída)
- Telefones (concluída)
Criar métodos Post para que usuários já cadastrados possam incluir um:
- Endereço (concluída)
- Telefone (concluída)

AGENDADOR DE TAREFAS - TAREFAS
Configurar Endpoint de verificação do token JWT pelo Agendador
Criar o repositório agendador no GitHub
Criar método:
- Post para cadastrar tarefas
- Get para buscar tarefas
- Put para alterar dados das tarefas
- Patch para alterar somente o status das tarefas
- Delete para excluir tarefas
Criar o banco de dados NoSQL db_agendador no MongoDB

NOTIFICAÇÃO POR EMAIL - TAREFAS
Criar método para enviar email

BFF - TAREFAS
Criar endpoints que apontam para o: 
- Cadastro de usuários
- Agendador de tarefas
Criar cron que chama a notificação por email
