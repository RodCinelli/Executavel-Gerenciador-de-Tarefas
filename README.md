# Gerenciador de Tarefas por Rodrigo Cinelli

## Descrição Geral

O Gerenciador de Tarefas é uma aplicação desenvolvida em Python, que utiliza a interface gráfica Tkinter. Este programa facilita a organização e o acompanhamento de tarefas, permitindo que o usuário adicione, visualize, edite, exclua e gerencie suas tarefas de forma eficiente. Além disso, ajuda a aumentar a produtividade e a evitar o esquecimento de compromissos importantes, enviando lembretes por e-mail aos usuários.

## Funcionalidades

- **Adicionar Novas Tarefas**: Preencha os campos e clique em "Adicionar" para salvar a tarefa.
- **Visualizar Tarefas Existentes**: Veja as tarefas na interface do programa. Tarefas com status “importante”, “pendente” ou “concluída” são coloridas automaticamente:
- **Importante**: Tarefas contendo a palavra “importante” após “-” ou “/” aparecerão em vermelho.
- **Pendente**: Tarefas contendo a palavra “pendente” após “-” ou “/” aparecerão em laranja.
- **Concluída**: Tarefas contendo as palavras “concluído” ou “concluída” após “-” ou “/” aparecerão em verde.
- **Pesquisar Tarefas**: Encontre tarefas específicas rapidamente digitando o ID da tarefa ou uma palavra-chave no campo correspondente.
- **Editar Tarefas**: Edite os detalhes das tarefas existentes e altere seu status para importante, pendente ou concluída, conforme desejar. As tarefas editadas serão coloridas automaticamente conforme a palavra-chave.
- **Excluir Tarefas**: Exclua tarefas indesejadas da lista. As tarefas são exibidas com a coloração correspondente antes da exclusão.
- **Botão 'Reset'**: Limpe todas as tarefas de uma vez e resete os IDs para zero.
- **Mensagens de Aviso e Sucesso**: Informações sobre ações do sistema para manter o usuário informado.
- **Envio de E-mails**: Envia ao usuário e-mails relacionados às tarefas que estão próximas ao prazo final.

## Inserindo Datas e Horas

- **Praticidade na Entrada de Dados**:  Ao inserir uma data, como “29/04/2024”, o usuário não precisa incluir as barras (“/”). Basta digitar os números consecutivamente (29042024) que o sistema automaticamente formatará para “29/04/2024”. O mesmo se aplica à inserção de horas. Por exemplo, para registrar 5h da tarde, o usuário pode simplesmente digitar “1700”, e o sistema completará automaticamente para “17:00 PM”, indicando claramente que se trata do horário da tarde. Esta funcionalidade de auto-completação facilita a entrada de informações e minimiza erros de formatação, tornando a interface mais intuitiva e eficiente.

## Envio de E-mails

- **Como Funciona**: Toda vez que o usuário abrir a aplicação, ela fará uma varredura nas tarefas inseridas e enviará um e-mail ao usuário quando qualquer tarefa estiver a um dia, uma hora ou menos do prazo final. Além disso, notificará caso a tarefa já tenha ultrapassado o prazo determinado.

- **Notificações Proativas**: O sistema envia automaticamente e-mails como lembretes para os usuários, informando sobre tarefas que estão se aproximando do prazo final. Isso ajuda a garantir que as tarefas não sejam esquecidas e sejam concluídas a tempo.

- **Tipos de Lembretes**: Os usuários recebem lembretes por e-mail quando falta um dia, uma hora ou menos para o prazo final definido para uma tarefa.

- **Detalhes Inclusos no E-mail**: Cada e-mail enviado contém o nome da tarefa, a data e a hora do prazo final, além de um lembrete sobre o tipo de notificação configurada (por exemplo, ‘uma hora antes’ ou ‘um dia antes’). Isso fornece todas as informações necessárias para que o usuário possa gerenciar suas tarefas eficientemente.

- **Configuração Automática de Horários**: Quando uma tarefa é adicionada sem especificar a “Hora de Início” ou a “Hora para Conclusão”, o sistema automaticamente define esses campos para facilitar o gerenciamento e as notificações. Se a “Hora de Início” não for fornecida, ela será definida como “00:00 AM” (meia-noite), e se a “Hora para Conclusão” não for fornecida, será definida como “23:59 PM” (um minuto antes da meia-noite). Essa configuração garante que todas as tarefas tenham um tempo definido e permite que as notificações sejam enviadas de maneira adequada e no tempo correto.

## Imagens da Aplicação

- **Interface do Usuário**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/interface_de_usuario.png" alt="Interface do Usuário"><br>

- **Adicionando Tarefas**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/adicionando_tarefas.png" alt="Adicionando Tarefas"><br>

- **Lista de Tarefas**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/lista_de_tarefas.png" alt="Lista de Tarefas"><br>

- **Editar Tarefas**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/editar_tarefas.png" alt="Editar Tarefas"><br>

- **Excluir Tarefas**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/excluir_tarefas.png" alt="Excluir Tarefas"><br>

- **Botão Reset**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/botao_reset.png" alt="Botão Reset"><br>

- **Notificações por E-mail**:<br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/notificacoes_por_email1.png" alt="Notificações por E-mail"><br><br><br><img src="https://github.com/RodCinelli/Executavel-Gerenciador-de-Tarefas/raw/main/images/notificacoes_por_email2.png" alt="Notificações por E-mail"><br>

## Tecnologias Utilizadas

- **Python**: Linguagem de programação escolhida para o projeto.
- **Tkinter**: Usado para criar a interface gráfica do usuário.
- **SQLite3**: Utilizado para o gerenciamento do banco de dados.
- **SMTP server**: O programa usa um servidor SMTP para enviar lembretes por e-mail.

## Como Instalar e Executar

Para instalar e executar o Gerenciador de Tarefas, você pode simplesmente seguir o passo a passo abaixo:

### Instalação: Fazer o download e executar o arquivo.exe

1. **Encontre o executável** (`Gerenciador de Tarefas.exe`) disponível na pasta `dist` e clique em `View raw`.

2. **Baixe o arquivo executável** e crie uma pasta para ele na área de trabalho.

2. **Insira o arquivo na pasta** e execute-o com um duplo clique.

## Teste de Funcionalidade

Utilize o e-mail pré-definido abaixo para ter uma visão geral da capacidade da aplicação. A aplicação tem a funcionalidade de enviar um lembrete por e-mail, alertando ao usuário quando uma tarefa estiver a apenas um dia, uma hora ou menos de atingir o seu prazo final.

Insira a tarefa normalmente através da interface do usuário e cheque a caixa de entrada do e-mail fornecido.

- **E-mail**: freegerenciador@gmail.com
- **Senha**: 123teste4

Toda vez que o usuário abrir a aplicação ela fará uma varredura nas tarefas inseridas e irá enviar um e-mail ao usuário quando qualquer tarefa que tiver sido incluída estiver a um dia, uma hora ou menos do seu prazo final.

## Licença

Esta aplicação e seu código fonte é atualmente definida como privada. Os direitos autorais e de uso são reservados ao autor do projeto, Rodrigo Cinelli. A distribuição, modificação ou uso comercial sem permissão explícita não são permitidos.

## Link do programa em distribuição

Após a conclusão definitiva do programa o coloquei para a venda no site vintepila.

- [Clique aqui para acessar o Link](https://www.vintepila.com.br/servicos/outros-servicos-programacao/eu-vou-criar-um-gerenciador-de-tarefas-personalizado/)

## Contato

Se gostou da aplicação e deseja adquirir ela de modo que envie notificações ao seu e-mail pessoal, ou empresarial, ou deseja funcionalidades exclusivas, entre em contato comigo através do e-mail ou telefone abaixo:

- Rodrigo Cinelli - [Enviar Email](mailto:rodcinelli@gmail.com)
- Telefone: (21) 98322 0819
