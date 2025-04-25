# Sistema de Cadastro de Eventos - IBRENJ Comunicação

Um sistema web para cadastro e gerenciamento de eventos da IBRENJ Comunicação, desenvolvido com HTML, CSS e JavaScript vanilla.

## Sobre o Projeto
Este sistema permite que usuários registrem informações sobre eventos, incluindo departamento responsável, dados de contato, data/hora, localização e informações adicionais. A aplicação foi desenvolvida com foco em acessibilidade, responsividade e experiência do usuário.

## Funcionalidades
- Formulário de Cadastro: Interface intuitiva para inserção de dados do evento
- Persistência Local: Salvamento automático dos dados durante o preenchimento
- Validação em Tempo Real: Verificação de campos obrigatórios e formato de email
- Pré-visualização: Revisão dos dados antes do envio final
- Responsividade: Design adaptável para diferentes tamanhos de tela
- Acessibilidade: Suporte a leitores de tela e navegação por teclado

## Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript (ES6+)
- LocalStorage API

## Estrutura do Projeto

```text
├── index.html         # Estrutura HTML, estilos críticos e scripts
├── styles.css         # Estilos adicionais
└── assets/
    ├── Logo.png       # Logo da IBRENJ Comunicação
    └── favicon.ico    # Favicon do site
```
    
## Campos do Formulário

| Campo                | Tipo            | Descrição                                  | Validação                     |
|---------------------|-----------------|---------------------------------------------|-------------------------------|
| Departamento         | select          | Departamento responsável pelo evento        | Obrigatório                   |
| Responsável          | text            | Nome da pessoa responsável                  | Obrigatório                   |
| Email                | email           | Email de contato                            | Obrigatório, formato válido   |
| Evento               | text            | Nome do evento                              | Obrigatório                   |
| Data e Hora          | datetime-local  | Data e hora do evento                       | Obrigatório                   |
| Local                | text            | Local onde será realizado o evento          | Obrigatório                   |
| Informações adicionais | textarea       | Detalhes complementares sobre o evento      | Obrigatório                   |


## Fluxo de Usuário

- O usuário preenche o formulário de cadastro
- Ao submeter, uma pré-visualização dos dados é exibida
- O usuário pode editar os dados ou confirmar o envio
- Após confirmação, uma mensagem de sucesso é exibida
- O formulário é resetado para permitir um novo cadastro

## Recursos de Acessibilidade

- Atributos ARIA implementados para melhorar a navegação por leitores de tela
- Mensagens de erro associadas aos campos correspondentes
- Suporte a navegação por teclado (incluindo tecla ESC para fechar modais)
- Foco gerenciado adequadamente entre os diferentes estados da aplicação

## Segurança

- Dados de formulário são escapados antes da exibição para prevenir ataques XSS
- Validação de dados tanto no cliente quanto antes do envio

## Implementações Futuras

- Integração com backend para persistência dos dados em servidor 
- Envio dos dados via API REST
- Sistema de notificação para eventos próximos
- Funcionalidades de busca e filtragem de eventos
- Autenticação de usuários para diferentes níveis de acesso

## Como Usar

- Clone este repositório
- Abra o arquivo index.html em seu navegador
- Preencha o formulário com as informações do evento
- Revise os dados na pré-visualização
- Confirme o envio

## Limitações Atuais

- Atualmente não há persistência de dados em servidor (apenas localStorage)
- A integração com backend está comentada e precisa ser implementada

## Copyright

© 2025 IBRENJ Comunicação. Todos os direitos reservados.
