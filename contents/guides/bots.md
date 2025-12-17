---
title: Guia de Bots
description: Aprenda a criar e gerenciar bots no Agendo Certo
---

# Guia de Bots

Os bots são assistentes virtuais que conversam com seus clientes no WhatsApp. Eles podem agendar serviços, responder dúvidas e muito mais!

## O que é um Bot?

Um bot é um fluxo de conversa automatizado:

```
Cliente: Olá!
   ↓
Bot: Olá! 👋 Bem-vindo à Barbearia do João!
     O que você gostaria de fazer?
     1️⃣ Agendar horário
     2️⃣ Ver meus agendamentos
     3️⃣ Falar com atendente
   ↓
Cliente: 1
   ↓
Bot: Ótimo! Qual serviço você deseja?
     📋 [Lista de Serviços]
```

## Acessando Bots

1. Clique em **Configurações** no menu lateral
2. Selecione **Bots**
3. Você verá a lista de todos os bots

## Criando um Bot

### Opção 1: Usar Template (Recomendado)

Templates são bots prontos que você pode personalizar:

1. Clique em **Novo Bot**
2. Escolha **Usar Template**
3. Selecione o template desejado:
   - **Agendamento Simples** - Fluxo básico
   - **Agendamento Completo** - Com profissional
   - **Atendimento Híbrido** - Bot + humano
4. Clique em **Criar**

> [!TIP]
> Templates já vêm configurados! Você pode personalizar mensagens e adicionar recursos depois.

### Opção 2: Criar do Zero

Para usuários avançados:

1. Clique em **Novo Bot**
2. Escolha **Bot em Branco**
3. Dê um nome ao bot
4. Clique em **Criar**

## Estrutura de um Bot

Um bot é composto por **nós** (componentes) e **conexões** (arestas):

```
[Início] → [Mensagem] → [Botões] → [Serviços] → [Profissional] → [Agendamento]
                           ↓
                    [Atendimento Humano]
```

### Componentes Principais

| Componente | Função |
|------------|--------|
| **Mensagem** | Envia texto ao cliente |
| **Botões** | Menu de opções clicáveis |
| **Lista** | Lista scrollável de opções |
| **Serviços** | Seleção de serviços |
| **Profissional** | Seleção de profissional |
| **Agendamento** | Escolha de data/hora |
| **Termos** | Aceite de termos |
| **Atendimento** | Transfere para humano |

## Editor de Bot

O editor é sua área de trabalho para criar fluxos.

### Área de Trabalho

- **Arrastar** - Mova componentes
- **Conectar** - Ligue saídas às entradas
- **Zoom** - Use scroll ou botões
- **Centralizar** - Botão de ajuste

### Barra Lateral

- **Componentes** - Arraste para adicionar
- **Configurações** - Ajustes do bot
- **Variáveis** - Dados dinâmicos

### Barra de Ferramentas

- **Salvar** - Salva alterações
- **Desfazer/Refazer** - Ctrl+Z / Ctrl+Y
- **Visualizar** - Testa o fluxo
- **Publicar** - Coloca em produção

## Componentes Essenciais

### Mensagem

Envia uma mensagem de texto:

```
Olá {{cliente.nome}}! 👋

Seja bem-vindo à Barbearia do João!
Como posso ajudar você hoje?
```

> [!TIP]
> Use `{{variavel}}` para personalizar mensagens!

### Botões

Cria menu com opções clicáveis:

```
Texto: O que deseja fazer?

Botões:
├── 📅 Agendar Horário
├── 📋 Meus Agendamentos
└── 💬 Falar com Atendente
```

### Seleção de Serviço

Lista serviços disponíveis:

- Mostra serviços ativos
- Exibe preço e duração
- Cliente seleciona um

### Seleção de Profissional

Lista profissionais disponíveis:

- Filtra por serviço selecionado
- Mostra foto e nome
- Opção "qualquer profissional"

### Agendamento

Permite escolher data e hora:

- Mostra dias disponíveis
- Horários livres do profissional
- Confirmação do agendamento

## Variáveis

Variáveis armazenam informações durante a conversa:

### Variáveis do Sistema

| Variável | Conteúdo |
|----------|----------|
| `{{cliente.nome}}` | Nome do cliente |
| `{{cliente.telefone}}` | Telefone |
| `{{servico.nome}}` | Serviço escolhido |
| `{{profissional.nome}}` | Profissional |
| `{{agendamento.data}}` | Data marcada |
| `{{agendamento.hora}}` | Horário |

### Usando Variáveis

```
Perfeito, {{cliente.nome}}! 🎉

Seu agendamento está confirmado:
📅 {{agendamento.data}}
⏰ {{agendamento.hora}}
💇 {{servico.nome}}
👤 {{profissional.nome}}

Te esperamos!
```

## Publicando o Bot

Após criar ou editar o bot:

1. Clique em **Salvar**
2. Clique em **Publicar**
3. Confirme a publicação

> [!WARNING]
> A publicação substitui a versão em produção! Sempre teste antes.

### Versões

O Agendo Certo mantém histórico de versões:

- **Rascunho** - Versão em edição
- **Produção** - Versão ativa
- **Histórico** - Versões anteriores

## Testando o Bot

### No Editor

1. Clique em **Visualizar** ou **Testar**
2. Uma simulação abrirá
3. Interaja como se fosse um cliente

### No WhatsApp

1. Configure o [Canal de Teste](/app/tutorials?doc=guides/canais)
2. Vincule o bot ao canal
3. Envie mensagem para o número de teste

## Atendimento Híbrido

Combine bot com atendimento humano:

```
Bot conversa com cliente
   ↓
Cliente pede atendente
   ↓
Bot transfere para humano
   ↓
Atendente assume a conversa
   ↓
Atendente finaliza
   ↓
Bot retoma o controle
```

### Componente de Atendimento

- Verifica horário comercial
- Checa disponibilidade de atendentes
- Transfere a conversa
- Notifica sobre fila

## Boas Práticas

### ✅ Faça

- Comece com templates
- Use mensagens curtas e claras
- Adicione emojis com moderação
- Teste antes de publicar
- Ofereça opção de atendente

### ❌ Evite

- Mensagens muito longas
- Muitas opções de uma vez
- Fluxos muito complexos
- Publicar sem testar
- Ignorar fallbacks (erro)

## Dicas Avançadas

### Fallback

Configure o que acontece quando o cliente envia algo inesperado:

```
Bot: Escolha uma opção:
     1️⃣ Agendar
     2️⃣ Cancelar

Cliente: "Quero saber o preço"

Bot: Desculpe, não entendi. 
     Por favor, escolha uma das opções:
     1️⃣ Agendar
     2️⃣ Cancelar
```

### Horário Comercial

Configure o bot para horários específicos:

- **Dentro do horário** → Fluxo normal
- **Fora do horário** → Mensagem especial

### Múltiplos Estabelecimentos

Se você tem várias unidades:

1. Adicione componente de **Seleção de Estabelecimento**
2. Posicione antes de serviços/profissionais
3. O fluxo continuará para a unidade escolhida

---

## Próximos Passos

- 📖 [Guia de Canais](/app/tutorials?doc=guides/canais) - Conecte seu bot ao WhatsApp
- 📖 [Guia de Serviços](/app/tutorials?doc=guides/servicos) - Configure serviços
- 📖 [Guia de Profissionais](/app/tutorials?doc=guides/profissionais) - Configure equipe
