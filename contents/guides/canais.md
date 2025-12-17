---
title: Guia de Canais
description: Aprenda a configurar e gerenciar canais de comunicação no Agendo Certo
---

# Guia de Canais

Canais são as conexões entre seus bots e as plataformas de mensagens. É através dos canais que seus clientes conversam com seus bots.

## O que são Canais?

Um canal conecta seu bot a uma plataforma:

```
WhatsApp Business ←→ Canal ←→ Bot ←→ Agendo Certo
```

### Tipos de Canal

| Canal | Descrição | Status |
|-------|-----------|--------|
| **WhatsApp Business** | Canal oficial | ✅ Disponível |
| **Canal de Teste** | Para desenvolvimento | ✅ Disponível |
| Instagram | Mensagens do Instagram | 🔜 Em breve |
| Telegram | Bot do Telegram | 🔜 Em breve |

## Acessando Canais

1. Clique em **Configurações** no menu lateral
2. Selecione **Canais**
3. Você verá a lista de todos os canais

## Canal de Teste

O Canal de Teste é um ambiente seguro para testar seus bots.

### Características

- ✅ Não afeta clientes reais
- ✅ Funcionalidades completas
- ✅ Mensagens gratuitas
- ✅ Ideal para desenvolvimento

### Configurando o Canal de Teste

1. Clique no **Canal de Teste**
2. Veja o número do canal
3. Adicione números autorizados
4. Vincule um bot

### Números Autorizados

Apenas números autorizados podem testar:

1. Na seção **Números Autorizados**
2. Clique em **Adicionar Número**
3. Digite o número com DDD:
   - Formato: `5511999999999`
   - Sem espaços ou caracteres especiais
4. Clique em **Salvar**

> [!WARNING]
> Este passo é **obrigatório**! Sem número autorizado, você não consegue testar.

### Vinculando um Bot

1. Clique em **Editar Canal**
2. No campo **Bot**, selecione seu bot
3. Clique em **Salvar**

Pronto! Agora você pode testar enviando mensagem para o número do canal.

## WhatsApp Business

O canal de WhatsApp é para uso em produção com clientes reais.

### Requisitos

Para usar o WhatsApp Business API:

- ✅ Conta Meta Business verificada
- ✅ Número de telefone dedicado
- ✅ Política de uso do WhatsApp aceita
- ✅ Plano Agendo Certo compatível

### Processo de Configuração

```
1. Verificar empresa no Meta
2. Registrar número de telefone
3. Configurar conta WABA
4. Conectar ao Agendo Certo
5. Vincular bot ao canal
```

> [!NOTE]
> A configuração do WhatsApp Business requer verificação da Meta, que pode levar alguns dias.

## Configurações do Canal

### Informações Básicas

| Campo | Descrição |
|-------|-----------|
| Nome | Nome identificador do canal |
| Descrição | Detalhes sobre o uso |
| Status | Ativo ou Inativo |
| Bot | Bot vinculado |

### Configurações Avançadas

| Configuração | Descrição |
|--------------|-----------|
| **Horário** | Quando o bot responde |
| **Mensagem de ausência** | Fora do horário |
| **Timeout** | Tempo máximo de conversa |
| **Retorno** | Mensagem após inatividade |

## Mensagens do WhatsApp

### Tipos de Mensagem

| Tipo | Iniciado por | Custo |
|------|--------------|-------|
| **Conversa de Usuário** | Cliente | Incluído |
| **Conversa de Marketing** | Empresa | Cobrado |
| **Conversa de Utilidade** | Empresa | Cobrado |
| **Conversa de Autenticação** | Empresa | Cobrado |

### Janela de 24 Horas

O WhatsApp tem uma regra importante:

```
Cliente envia mensagem → Janela abre → 24 horas para responder
                                                  ↓
                              Janela fecha → Só templates permitidos
```

> [!TIP]
> Respostas automáticas do bot mantêm a conversa ativa dentro da janela!

### Templates de Mensagem

Para iniciar conversas ou responder após 24h:

1. Crie um template no Meta Business
2. Aguarde aprovação (24-48h)
3. Use no Agendo Certo

```
Olá {{1}}! 👋

Seu agendamento está confirmado:
📅 {{2}} às {{3}}
💇 {{4}}

Te esperamos!
```

## Métricas e Relatórios

Acompanhe o desempenho do canal:

### Métricas Disponíveis

| Métrica | Descrição |
|---------|-----------|
| **Mensagens Recebidas** | Total de mensagens de clientes |
| **Mensagens Enviadas** | Total de respostas do bot |
| **Conversas** | Número de conversas únicas |
| **Taxa de Resolução** | % resolvido pelo bot |
| **Tempo Médio** | Duração das conversas |

## Múltiplos Canais

Você pode ter vários canais ativos:

```
Empresa XYZ
├── Canal de Teste → Bot de Desenvolvimento
├── WhatsApp Vendas → Bot Comercial
└── WhatsApp Suporte → Bot de Suporte
```

### Casos de Uso

- **Por departamento** - Vendas, suporte, RH
- **Por unidade** - Filial A, Filial B
- **Por propósito** - Agendamento, informações

## Boas Práticas

### ✅ Faça

- Sempre teste antes de ir para produção
- Mantenha números autorizados atualizados
- Configure mensagens de ausência
- Monitore métricas regularmente
- Responda dentro de 24 horas

### ❌ Evite

- Publicar bot sem testar
- Ignorar políticas do WhatsApp
- Enviar spam ou mensagens em massa
- Deixar clientes sem resposta
- Usar números pessoais

## Solução de Problemas

### Canal não recebe mensagens

1. Verifique se o canal está **Ativo**
2. Confirme se há um **Bot vinculado**
3. Cheque se o número está **Autorizado** (teste)
4. Verifique a conexão com a Meta (produção)

### Bot não responde

1. Verifique se o bot está **Publicado**
2. Confira se o bot está **Vinculado ao canal**
3. Teste o bot no **Visualizador**
4. Verifique logs de erro

### Mensagens atrasadas

1. Verifique sua conexão de internet
2. Cheque status dos servidores
3. Contate o suporte se persistir

> [!TIP]
> A maioria dos problemas se resolve verificando: Bot publicado? Canal ativo? Número autorizado?

---

## Próximos Passos

- 📖 [Guia de Bots](/app/tutorials?doc=guides/bots) - Crie e personalize bots
- 📖 [Tutorial de Configuração](/app/tutorials?doc=getting-started/02-configuracao-inicial) - Passo a passo completo
- 📖 [Bem-vindo](/app/tutorials?doc=getting-started/01-bem-vindo) - Visão geral da plataforma
