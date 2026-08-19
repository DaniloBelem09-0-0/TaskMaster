# PRD - TaskMaster

## Documento de Requisitos do Produto

> Documento-base para a entrega da Aula 2 (12/08). Os itens marcados como **Pendente de validação** devem ser confirmados pela equipe e pela professora.

## 1. Identificação e equipe

- **Nome do projeto/app:** TaskMaster
- **Equipe:** Grupo 2 - Danilo, José e Luiz Fernando
- **Disciplina:** Programação para Dispositivos Móveis II
- **Tecnologia principal:** Flutter (Dart)
- **Repositório GitHub:** **Pendente de validação** - `https://github.com/[organização-ou-usuário]/TaskMaster`

## 2. Visão geral e proposta de valor

### Problema

Estudantes e profissionais precisam organizar tarefas, prazos e prioridades em um único lugar, mas frequentemente usam anotações dispersas ou ferramentas que não oferecem uma experiência simples e confiável também quando estão sem conexão.

### Solução

O TaskMaster será um aplicativo mobile em Flutter para criação, organização e acompanhamento de tarefas. A aplicação permitirá visualizar o que precisa ser feito, acompanhar o progresso e manter os dados disponíveis localmente, sincronizando-os com uma API quando houver conexão.

### Público-alvo

Estudantes universitários e profissionais autônomos que precisam organizar atividades pessoais, acadêmicas ou profissionais.

### Cliente / Product Owner

**Pendente de validação:** professora da disciplina como avaliadora do produto e equipe do Grupo 2 como responsável pela definição e priorização do backlog.

## 3. Escopo e lista inicial de funcionalidades

### Módulo 1 - MVP, telas iniciais e navegação (Etapa 1 - A1)

- **[US01] Autenticação e onboarding:** telas de boas-vindas, login e cadastro.
- **[US02] Navegação principal:** `BottomNavigationBar` com acesso às tarefas, calendário e perfil/configurações.
- **[US03] Listagem principal:** exibição de tarefas em cards, com título, prazo, prioridade e status.
- **[US04] Cadastro e edição de tarefas:** criação, edição, conclusão e exclusão de tarefas.

### Módulo 2 - Núcleo funcional e integrações (Etapa 2)

- **[US05] Consumo de API REST:** sincronização com backend ou API externa usando `Dio` ou `http`, com tratamento de carregamento e erros.
- **[US06] Gerenciamento de estado:** atualização reativa e compartilhada da aplicação usando `Provider` ou `Riverpod`.
- **[US07] Persistência local:** cache ou banco local para consulta e edição em modo offline-first.
- **[US08] Filtros e prioridades:** filtragem por status, prazo e prioridade, além de ordenação das tarefas.

### Módulo 3 - Inteligência artificial (Etapa 3 - A2)

- **[US09] Categorização inteligente:** a IA sugerirá categoria e prioridade a partir do título e da descrição da tarefa.
- **Escopo da integração:** **Pendente de validação** - definir entre IA na nuvem, por API, ou IA embarcada, considerando credenciais, custo, privacidade e critérios da disciplina.

### Módulo 4 - Finalização e build (Etapa 4)

- **[US10] Configurações de produção:** geração do bundle `.aab`, configuração do ambiente de testes e preparação para publicação.
- **[US11] Qualidade e entrega:** revisão de fluxos principais, tratamento de estados vazios/erro e documentação da instalação e uso.

## 4. Requisitos não funcionais e arquitetura

- **Framework:** Flutter e Dart.
- **Arquitetura:** separação em camadas com Repository Pattern, mantendo apresentação, domínio e dados desacoplados.
- **Injeção de dependência:** dependências de repositórios, serviços e clientes HTTP devem ser configuráveis e testáveis.
- **Estado:** Provider ou Riverpod, conforme decisão da equipe.
- **Conectividade:** a interface deve apresentar estados de carregamento, sucesso, erro e ausência de dados.
- **Offline-first:** dados essenciais devem permanecer acessíveis localmente e ser sincronizados quando a conexão retornar.
- **Controle de versão:** Git/GitHub, com branches por funcionalidade, Pull Requests e Code Review.
- **Colaboração:** revisão cruzada com o Grupo 1, conforme orientação da disciplina.
- **Commits:** frequentes, atômicos e com mensagens descritivas, identificando a alteração realizada.

## 5. Roadmap resumido

| Etapa | Entrega principal | Situação |
| --- | --- | --- |
| 1 - A1 | MVP, telas iniciais e navegação | Planejada |
| 2 | API REST, estado e persistência local | Planejada |
| 3 - A2 | Integração e validação do caso de uso de IA | Planejada |
| 4 | Testes finais, bundle `.aab` e publicação/testes | Planejada |

## 6. Checkpoint da Aula 2 (12/08)

| Item de validação | Status | Responsável |
| --- | --- | --- |
| Definição da proposta e do escopo | Concluído | Equipe: Danilo, José e Luiz Fernando |
| Lista inicial de funcionalidades | Concluído | Equipe |
| Repositório no GitHub criado e compartilhado | Concluído | Danilo |
| Validação com a professora | Pendente - apresentação em sala | Equipe |

## 7. Decisões pendentes

- Confirmar o nome definitivo do projeto: **TaskMaster** ou outra opção.
- Substituir o endereço provisório pelo link real do repositório GitHub.
- Definir o Product Owner, caso exista um cliente externo.
- Escolher entre Provider e Riverpod.
- Confirmar a abordagem de IA e os critérios de avaliação com a professora.
