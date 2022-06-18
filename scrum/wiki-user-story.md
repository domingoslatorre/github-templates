# Como escrever as histórias de usuário

Uma história de usuário é uma breve descrição de algo um determinado perfil de usuário fará na sua aplicação com foco no valor que ele obtém do processo. Devem ser escritas com o ponto de vista do usuário e com a linguagem que ele utiliza.

Em geral uma história segue o seguinte template:

> Como um **perfil (quem)** eu quero **algo (o quê)** para **me beneficiar (por quê)**

## Exemplos:
> Como um **cliente** eu quero **pagar com pix** para **não ter que fornecer meus dados de cartão de crédito**

> Como um **aluno** eu quero **me cadastrar no sistema** para **ter acesso aos arquivos de acompanhamento de estágio**


## Vantagens das histórias de usuário
- Funcionalidades da aplicação sobre o ponto de vista dos usuários
- Definem funcionalidade discretas
- Reduz o tempo de planejamento inicial
- Convite para uma conversa com os usuários e dono do projeto (product owner)

## Critérios de aceitação
São os critérios que devem ser atendidos para uma história de usuário ser considerada completa. Eles são usados para confirmar se tudo está funcionando como esperado e também definem um limite para a história. Quando utilizado com SCRUM, o Product Owner do projeto define os critérios de aceitação.

Imagine a seguinte história:

> Como um **aluno** eu quero **me cadastrar no sistema** para **ter acesso aos arquivos de acompanhamento de estágio**

O time de desenvolvimento poderia perguntar ao product owner:

- Quais informações precisaremos coletar neste cadastro?
- Existe algum padrão de validação neste número de matricula?
- O aluno precisa confirmar o cadastro de alguma forma? Via link no e-mail? sms?
- Caso ele já estiver cadastrado, podemos seguir com o comportamento padrão?
- O aluno terá acesso apenas aos arquivos dele?
- Existe algum problema de utilizar o login via sistema acadêmico?

Com base nesta discussão entre com P.O. e time de desenvolvimento, poderiam ser definidos os seguintes critérios de aceitação:

- Um aluno não poderá enviar o dados de cadastro sem preencher os campos obrigatório (nome, email, matricula)
- A matricula deverá ser validado com o padrão "xyz"
- Um link de confirmação deverá ser enviado via e-mail ao aluno
- O link de confirmação deverá expirar em 24 horas
- O registro de aluno não confirmado deverá ser liberado após expiração do link 
- O orientador de estágio deverá ser avisado via e-mail que seu aluno se cadastrou no sistema
- Deve ser possível o aluno se registrar usando uma conta Google `esse item poderia ser negociado e virar uma nova história com seus próprios critérios de aceitação`

### Definição de pronto
Definição de pronto são itens que devem ser atendidos por todas as histórias de usuário, exemplo: 
- Documentação do projeto foi atualizada e revisada;
- Pull request foi revisado por pelo menos 1 membro do time.

Já os critérios de aceitação devem ser atendidos por uma história específica.

Veja mais sobre na wiki [Definição de Pronto]().

## Template de issue
```md
> Antes de escrever a user story verificar a wiki [Como escrever as histórias de usuário](). Apagar este bloco antes de salvar a issue

Como um **perfil (quem)** eu quero **algo (o quê)** para **me beneficiar (por quê)**

## Tamanho estimado

pequeno/medio/grande

## Critérios de Aceitação

- [ ] ...
- [ ] ...
- [ ] ...

## Tarefas

Etapas específicas que precisam ser realizadas

## Definição de Pronto

Link para a documentação de Definição de Pronto do projeto

## Referências
- links a materiais, documentação
- links para histórias relacionadas

```

## Referências
- [Introduction to user stories](https://www.boost.co.nz/blog/2010/09/user-stories)