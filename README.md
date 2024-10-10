Agendador de tarefas

<< Atualmente estou trabalhando no desenvolvimento desta aplicação no microsserviço cadastro de usuários >>

A principal função dessa aplicação será enviar para o usuário um lembrete das tarefas que ele agendou.

METODOLOGIA ÁGIL KANBAN
Vamos dividir a aplicação em quatro microsserviços. Para cada microsserviço, faremos uma lista de tarefas. O objetivo é melhorar a organização do projeto e agilizar o desenvolvimento da aplicação.

MICROSSERVIÇOS QUE PRECISAM SER DESENVOLVIDOS
1) Cadastro de usuários
2) Agendador de tarefas
3) Notificação por email
4) BFF (Back-end For Front-end). Este padrão de arquitetura fará a intermediação entre os 3 primeiros microsserviços e o Front-end

CADASTRO DE USUÁRIOS - TAREFAS
Criar o banco de dados db_usuario no PostegreSQL (tarefa concluída)
Inicializar a aplicação usando o Spring Initializr (tarefa concluída)
Criar o repositório usuario no GitHub (tarefa concluída)
Configurar o CI/CD (tarefa concluída)
Configurar a segurança com Spring Security (tarefa concluída)
Criar método Post para cadastrar usuários (tarefa concluída)
Criar método Get para buscar usuários (tarefa concluída)
Criar método Delete para excluir usuários (tarefa concluída)
Criar método de login de usuário (tarefa concluída)
Criar método Put para alterar dados dos usuários 
Configurar Endpoint de verificação do token JWT pelo Agendador

AGENDADOR DE TAREFAS - TAREFAS
Criar o repositório agendador no GitHub
Criar método Post para cadastrar tarefas
Criar método Get para buscar tarefas
Criar método Put para alterar dados das tarefas
Criar método Patch para alterar somente o status das tarefas
Criar método Delete para excluir tarefas
Criar o banco de dados NoSQL db_agendador no MongoDB

NOTIFICAÇÃO POR EMAIL - TAREFAS
Criar método para enviar email

BFF - TAREFAS
Criar endpoints que apontam para o cadastro de usuários
Criar endpoints que apontam para o agendador de tarefas
Criar cron que chama a notificação por email
