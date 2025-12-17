---
title: Tutorial de Configuração Inicial
description: Passo a passo completo para configurar sua conta e começar a usar o Agendo Certo
---

# Tutorial de Configuração Inicial

Este tutorial irá guiá-lo por todas as etapas necessárias para configurar sua conta e deixar tudo pronto para começar a atender seus clientes automaticamente.

> [!NOTE]
> Reserve cerca de **15-20 minutos** para completar toda a configuração inicial.

## Visão geral

| Etapa | Tempo estimado |
|-------|----------------|
| Configurar estabelecimento | 5 min |
| Cadastrar serviços | 3 min |
| Adicionar profissionais | 3 min |
| Criar bot | 2 min |
| Configurar canal de teste | 3 min |
| Vincular bot ao canal | 1 min |

---

## Etapa 1: Configurar o estabelecimento

O estabelecimento representa seu negócio ou unidade. Configure informações básicas, endereço e horários de funcionamento.

### Como acessar

1. Clique no menu **Configurações** na barra lateral
2. Selecione **Estabelecimentos**
3. Clique no seu estabelecimento para editar

### Informações obrigatórias

| Campo | Descrição | Exemplo |
|-------|-----------|----------|
| **Nome** | Nome do negócio | Barbearia do João |
| **Telefone** | Contato principal | (11) 99999-9999 |
| **E-mail** | E-mail de contato | contato@barbearia.com |

### Endereço

Preencha o endereço completo:

- **CEP** — Preencha para autocompletar os demais campos
- **Logradouro** — Rua, avenida, etc.
- **Número** e **Complemento** (opcional)
- **Bairro**, **Cidade** e **Estado**

> [!TIP]
> Verifique se o pin do mapa está no local correto. A geolocalização é exibida para seus clientes.

### Horário de funcionamento

Configure os dias e horários de operação:

1. Acesse a aba **Horários**
2. Para cada dia, defina se está aberto ou fechado
3. Configure horário de início e término

> [!WARNING]
> Os horários do estabelecimento afetam a disponibilidade de agendamentos.

### Bloqueios

Bloqueie datas específicas (feriados, férias):

1. Acesse a aba **Bloqueios**
2. Clique em **Adicionar Bloqueio**
3. Selecione data, horário e descrição

---

## Etapa 2: Cadastrar Serviços

Serviços são o que você oferece aos clientes. Cada serviço tem um nome, duração e preço.

### Como acessar

1. Vá em **Configurações** → **Serviços**
2. Clique em **Novo Serviço**

### Informações do serviço

| Campo | Descrição | Exemplo |
|-------|-----------|---------|
| **Nome** | Nome do serviço | "Corte de Cabelo" |
| **Descrição** | Detalhes do serviço | "Corte masculino completo" |
| **Duração** | Tempo em minutos | 30 |
| **Preço** | Valor do serviço | R$ 50,00 |

### Configurações avançadas

- **Ativo** - Se o serviço está disponível para agendamento
- **Ordem** - Posição na lista de serviços
- **Categoria** - Agrupamento de serviços similares

> [!TIP]
> Você pode pular esta etapa e cadastrar serviços depois. Porém, sem serviços, não será possível realizar agendamentos.

---

## Etapa 3: Adicionar profissionais

Profissionais são as pessoas que realizam os serviços.

### Como acessar

1. Vá em **Configurações** → **Profissionais**
2. Clique em **Novo Profissional**

### Informações do profissional

| Campo | Descrição |
|-------|-----------|
| **Nome** | Nome completo |
| **E-mail** | E-mail do profissional |
| **Telefone** | Telefone de contato |
| **Foto** | Imagem (opcional) |

### Vincular serviços

1. Na aba **Serviços**, clique em **Adicionar Serviço**
2. Selecione os serviços que o profissional realiza
3. Opcionalmente, defina um preço diferente para cada serviço

> [!NOTE]
> Um profissional pode realizar vários serviços, e um serviço pode ser realizado por vários profissionais.

### Horários do profissional

Configure a agenda na aba **Horários**. Os horários devem estar dentro do funcionamento do estabelecimento.

---

## Etapa 4: Criar o bot

O bot é o assistente virtual que conversa com seus clientes no WhatsApp.

### Como acessar

1. Vá em **Configurações** → **Bots**
2. Clique em **Novo Bot**

### Usando um template

1. Na tela de criação, escolha **Usar Template**
2. Selecione o template adequado ao seu negócio:
   - **Agendamento Simples** — Para serviços básicos
   - **Agendamento Completo** — Com seleção de profissional
   - **Atendimento Híbrido** — Bot + atendimento humano
3. Clique em **Criar Bot**

> [!TIP]
> Templates já vêm configurados. Você pode personalizá-los depois.

### Editor do bot

Após criar, clique no bot para abrir o editor:

- **Área de trabalho** — Fluxo de conversa
- **Componentes** — Blocos que formam o bot
- **Configurações** — Ajustes gerais
- **Pré-visualização** — Teste antes de publicar

---

## Etapa 5: Configurar canal de teste

O canal de teste é um ambiente sandbox que permite testar seu bot antes de colocá-lo em produção.

### Como acessar

1. Vá em **Configurações** → **Canais**
2. Clique no **Canal de Teste**

### Vincular o bot

1. Clique em **Editar Canal**
2. Selecione o bot que você criou
3. Clique em **Salvar**

### Cadastrar seu número

Para testar, você precisa autorizar seu telefone:

1. Na seção **Números Autorizados**, clique em **Adicionar Número**
2. Digite seu número no formato internacional: `+5511999999999`
3. Clique em **Salvar**

> [!WARNING]
> Sem um número autorizado, suas mensagens serão ignoradas pelo sistema.

---

## Etapa 6: Testar o bot

Agora você pode testar o bot no WhatsApp.

### Como testar

1. No WhatsApp, adicione o número `+1 555 190-6729` aos seus contatos
2. Envie uma mensagem para esse número
3. O bot vinculado ao seu canal responderá automaticamente

> [!TIP]
> O número `+1 555 190-6729` é o sandbox oficial da Meta. Todas as mensagens enviadas para ele são roteadas com base no seu número cadastrado.

---

## Configuração concluída

Seu bot está funcionando e pronto para atender.

### Próximos passos

- [Guia de Estabelecimentos](/app/tutorials?doc=guides/estabelecimentos) — Configure múltiplas unidades
- [Guia de Serviços](/app/tutorials?doc=guides/servicos) — Organize seus serviços
- [Guia de Profissionais](/app/tutorials?doc=guides/profissionais) — Gerencie sua equipe
- [Guia de Bots](/app/tutorials?doc=guides/bots) — Personalize seu assistente
- [Guia de Canais](/app/tutorials?doc=guides/canais) — Configure WhatsApp para produção
