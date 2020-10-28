# Recuperação de senha

**RF**

- O usuário deve poder recuperar sua senha informando seu e-mail;
- O  usuário deve receber um e-mail com instruções de reciuperação de senha;
- O usuário deve poder resetar sua senha;

**RNF**

- Utilizar Mailtrap para testar envios em ambiente de dev;
- Utilizar o Amazon SES para envios em produção;
- O envio de e-mails deve aconteecer em segundo plano;

**RN**

- O link enviado por e-mail para resetar senha, deve expirar em 2h;
- O usuário precisa confirmar a nova senha ao resetar a senha;

# Atualição do perfil

**RF**

- O usuário deve poder atualizar seu nome, email e senha;

**RN**

- o usuário não pode alterar seu e-mail para um e-mail já existente;
- Para atualizar sua senha, o usuário deve informar a senha antiga;
- Para atualizar sua senha, o usuário precisa confirmar a nova senha;

# Painel do prestador

**RF**

- O usuário deve poder listar seus agendamentos de um dia específico;
- O prestador deve receber uma notificação sempre que houver um novo agendamento;
- O prestador deve poder visualizar as notificações não lidas;

**RNF**

- Os agendamentos do prestador no dia devem ser armazenados em cache;
- As notificações do prestador devem ser armazenadas no MongoDB;
- As notificações do prestador devem ser enviadas em tempo real utilizando Socket.io;

**RN**

- A notificação deve ter um status de lida ou não-lida para que o prestador possa controlar;

# Agendamento de serviços

**RF**

- O usuário deve poder listar todos prestadores de serviços cadastrados;
- O usuário deve poder listar os dias de um mês com pelo menos um horário disponível de um prestador;
- O usuário deve poder listar horários disponíveis em um dia específico de um prestador;
- O usuário deve poder realizar um novo agendamento com um prestador;

**RNF**

- A listagem de prestadores deve ser armazenada em cache;

**RN**

- Os agendamentos devem estar disponíveis entre 8h às 18h (primeiro horário às 8h, último às 17h);
- O usuário não pode agendar em um horário que já passou;
- O usuário não pode agendar um horário consigo mesmo;
- O usuário não pode agendar em um horário já ocupado;
- Cada agendamento deve durar 1h exatamente;
