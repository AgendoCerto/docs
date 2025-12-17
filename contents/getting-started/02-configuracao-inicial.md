---
title: Tutorial de Configuração Inicial
description: Passo a passo completo para configurar sua conta e começar a usar o Agendo Certo
---

# Tutorial de Configuração Inicial

Este tutorial irá guiá-lo por todas as etapas necessárias para configurar sua conta e deixar tudo pronto para começar a atender seus clientes automaticamente.

> [!NOTE]
> Reserve cerca de **15-20 minutos** para completar toda a configuração inicial.

## Visão Geral das Etapas

```
1. Configurar Estabelecimento    ⏱️ ~5 min
2. Cadastrar Serviços           ⏱️ ~3 min
3. Adicionar Profissionais      ⏱️ ~3 min
4. Criar seu Bot                ⏱️ ~2 min
5. Configurar Canal de Teste    ⏱️ ~3 min
6. Vincular Bot ao Canal        ⏱️ ~1 min
```

---

## Etapa 1: Configurar o Estabelecimento

O estabelecimento representa seu negócio ou unidade. É aqui que você define informações básicas, endereço e horários de funcionamento.

### Como acessar

1. Clique no menu **Configurações** na barra lateral
2. Selecione **Estabelecimentos**
3. Clique no seu estabelecimento para editar

### Informações obrigatórias

Preencha os seguintes campos:

| Campo | Descrição | Exemplo |
|-------|-----------|---------|
| **Nome** | Nome do seu negócio | "Barbearia do João" |
| **Telefone** | Contato principal | "(11) 99999-9999" |
| **E-mail** | E-mail de contato | "contato@barbearia.com" |

### Endereço e Geolocalização

Preencha o endereço completo para que clientes possam encontrar você:

- **CEP** - Ao preencher, os campos serão preenchidos automaticamente
- **Logradouro** - Rua, avenida, etc.
- **Número** - Número do estabelecimento
- **Complemento** - Sala, andar, etc. (opcional)
- **Bairro** - Bairro do estabelecimento
- **Cidade** e **Estado** - Localização

> [!TIP]
> A geolocalização é usada para mostrar a localização no mapa para seus clientes. Verifique se o pin está no local correto!

### Horário de Funcionamento

Configure os dias e horários que seu estabelecimento opera:

1. Clique na aba **Horários**
2. Para cada dia da semana, defina:
   - Se está **aberto** ou **fechado**
   - **Horário de início** (ex: 08:00)
   - **Horário de término** (ex: 18:00)

> [!WARNING]
> Os horários do estabelecimento afetam a disponibilidade de agendamentos. Certifique-se de configurar corretamente!

### Calendário e Bloqueios

Você pode bloquear datas específicas (feriados, férias, etc.):

1. Acesse a aba **Bloqueios**
2. Clique em **Adicionar Bloqueio**
3. Selecione a data e horário
4. Adicione uma descrição (opcional)

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

## Etapa 3: Adicionar Profissionais

Profissionais são as pessoas que realizam os serviços. Cada profissional tem seus próprios horários e serviços.

### Como acessar

1. Vá em **Configurações** → **Profissionais**
2. Clique em **Novo Profissional**

### Informações do profissional

Preencha os dados básicos:

| Campo | Descrição |
|-------|-----------|
| **Nome** | Nome completo |
| **E-mail** | E-mail do profissional |
| **Telefone** | Telefone de contato |
| **Foto** | Imagem do profissional (opcional) |

### Vincular Serviços

Se você cadastrou serviços na etapa anterior:

1. Na aba **Serviços**, clique em **Adicionar Serviço**
2. Selecione os serviços que este profissional realiza
3. Opcionalmente, defina um preço diferente para cada serviço

> [!NOTE]
> Um profissional pode realizar vários serviços, e um serviço pode ser realizado por vários profissionais.

### Horários do Profissional

Configure a agenda do profissional:

1. Acesse a aba **Horários**
2. Defina os dias e horários de trabalho
3. Os horários devem estar dentro do funcionamento do estabelecimento

---

## Etapa 4: Criar seu Bot

Agora vamos criar seu assistente virtual! O bot é quem vai conversar com seus clientes no WhatsApp.

### Como acessar

1. Vá em **Configurações** → **Bots**
2. Clique em **Novo Bot**

### Usando um Template

A forma mais fácil de começar é usando um template:

1. Na tela de criação, escolha **Usar Template**
2. Selecione um template que se adeque ao seu negócio:
   - **Agendamento Simples** - Para serviços básicos
   - **Agendamento Completo** - Com seleção de profissional
   - **Atendimento Híbrido** - Bot + atendimento humano
3. Clique em **Criar Bot**

> [!TIP]
> Os templates já vêm configurados e prontos para usar! Você pode personalizá-los depois.

### Explorando o Bot

Após criar o bot, clique nele para abrir o editor:

- **Área de trabalho** - Visualize o fluxo de conversa
- **Componentes** - Blocos que formam o bot
- **Configurações** - Ajustes gerais do bot
- **Pré-visualização** - Teste o bot antes de publicar

> [!NOTE]
> Não se preocupe em entender todos os componentes agora. Os templates já vêm prontos para uso!

---

## Etapa 5: Configurar Canal de Teste

O canal é a conexão entre o bot e o WhatsApp. Vamos configurar o canal de teste.

### Como acessar

1. Vá em **Configurações** → **Canais**
2. Clique no **Canal de Teste**

### Sobre o Canal de Teste

O Canal de Teste é um ambiente seguro para você testar seu bot antes de colocá-lo em produção:

- ✅ Não envia mensagens para clientes reais
- ✅ Permite testar todas as funcionalidades
- ✅ Ideal para validar seu fluxo

### Números Autorizados

Para receber mensagens do canal de teste, você precisa autorizar seu número:

1. Na seção **Números Autorizados**, clique em **Adicionar Número**
2. Digite seu número de WhatsApp com DDD
3. Formato: `5511999999999` (sem espaços ou caracteres especiais)
4. Clique em **Salvar**

> [!WARNING]
> Este passo é **obrigatório** para continuar. Sem um número autorizado, você não conseguirá testar o bot.

---

## Etapa 6: Vincular Bot ao Canal

Última etapa! Vamos conectar o bot que você criou ao canal de teste.

### Como fazer

1. Na tela do Canal de Teste, clique em **Editar Canal**
2. No campo **Bot**, selecione o bot que você criou
3. Clique em **Salvar**

### Testando seu Bot

Agora você pode testar! 

1. Abra o WhatsApp no seu celular
2. Envie uma mensagem para o número do Canal de Teste
3. O bot irá responder automaticamente!

> [!TIP]
> O número do Canal de Teste está na tela de configuração do canal.

---

## Parabéns! 🎉

Você completou a configuração inicial do Agendo Certo! Seu bot já está funcionando e pronto para atender.

### Próximos Passos

- 📖 [Guia de Estabelecimentos](/app/tutorials?doc=guides/estabelecimentos) - Configure múltiplas unidades
- 📖 [Guia de Serviços](/app/tutorials?doc=guides/servicos) - Organize seus serviços
- 📖 [Guia de Profissionais](/app/tutorials?doc=guides/profissionais) - Gerencie sua equipe
- 📖 [Guia de Bots](/app/tutorials?doc=guides/bots) - Personalize seu assistente
- 📖 [Guia de Canais](/app/tutorials?doc=guides/canais) - Configure WhatsApp para produção

### Precisa de Ajuda?

Se tiver dúvidas durante a configuração, entre em contato com nosso suporte!
