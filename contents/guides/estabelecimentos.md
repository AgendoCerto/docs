---
title: Guia de Estabelecimentos
description: Aprenda a configurar e gerenciar estabelecimentos no Agendo Certo
order: 1
---

# Guia de Estabelecimentos

O estabelecimento é a base do seu negócio no Agendo Certo. Aqui você configura informações, horários e tudo que seus clientes precisam saber.

## O que é um Estabelecimento?

Um estabelecimento representa uma unidade do seu negócio. Se você tem várias filiais, cada uma será um estabelecimento diferente.

```
Seu Negócio
├── Unidade Centro     → Estabelecimento 1
├── Unidade Shopping   → Estabelecimento 2
└── Unidade Bairro     → Estabelecimento 3
```

## Acessando Estabelecimentos

1. Clique em **Configurações** no menu lateral
2. Selecione **Estabelecimentos**
3. Você verá a lista de todos os estabelecimentos

## Informações Básicas

### Dados Principais

| Campo | Obrigatório | Descrição |
|-------|-------------|-----------|
| Nome | ✅ | Nome exibido para os clientes |
| Telefone | ✅ | Número de contato principal |
| E-mail | ✅ | E-mail para notificações |
| Descrição | ❌ | Texto sobre o estabelecimento |
| Logo | ❌ | Imagem do seu negócio |

### Endereço Completo

O endereço é importante para que clientes possam encontrar você:

| Campo | Descrição |
|-------|-----------|
| CEP | Preencha para autocompletar |
| Logradouro | Rua, avenida, travessa... |
| Número | Número do imóvel |
| Complemento | Sala, andar, bloco... |
| Bairro | Bairro do estabelecimento |
| Cidade | Cidade |
| Estado | UF |

> [!TIP]
> Ao digitar o CEP, os campos de endereço serão preenchidos automaticamente!

### Geolocalização

A localização no mapa ajuda seus clientes:

1. Após preencher o endereço, o mapa será atualizado
2. Você pode arrastar o marcador para ajustar a posição
3. A localização é usada no componente de **Localização** do bot

## Horário de Funcionamento

Configure os dias e horários que o estabelecimento opera.

### Configurando Horários

Para cada dia da semana, defina:

- **Status** - Aberto ou Fechado
- **Hora de abertura** - Quando abre
- **Hora de fechamento** - Quando fecha

Exemplo de configuração:

| Dia | Status | Abertura | Fechamento |
|-----|--------|----------|------------|
| Segunda | Aberto | 08:00 | 18:00 |
| Terça | Aberto | 08:00 | 18:00 |
| Quarta | Aberto | 08:00 | 18:00 |
| Quinta | Aberto | 08:00 | 18:00 |
| Sexta | Aberto | 08:00 | 18:00 |
| Sábado | Aberto | 08:00 | 12:00 |
| Domingo | Fechado | - | - |

### Múltiplos Períodos

Se você fecha para almoço, pode configurar múltiplos períodos:

- Período 1: 08:00 - 12:00
- Período 2: 14:00 - 18:00

> [!NOTE]
> Os horários do estabelecimento afetam a disponibilidade de todos os profissionais vinculados.

## Bloqueios de Agenda

Bloqueie datas específicas quando o estabelecimento não irá funcionar.

### Quando usar bloqueios

- 🎄 Feriados
- 🏖️ Férias coletivas
- 🔧 Manutenção
- 📅 Eventos especiais

### Criando um Bloqueio

1. Acesse a aba **Bloqueios**
2. Clique em **Adicionar Bloqueio**
3. Preencha:
   - **Data** - Data do bloqueio
   - **Tipo** - Dia todo ou período específico
   - **Motivo** - Descrição (opcional)
4. Clique em **Salvar**

> [!WARNING]
> Bloqueios afetam todos os profissionais do estabelecimento. Use bloqueios individuais para folgas de profissionais específicos.

## Calendário

A aba Calendário oferece uma visão geral:

- 📅 Visualize agendamentos
- 🔴 Veja bloqueios
- 📊 Acompanhe a ocupação

### Cores do Calendário

| Cor | Significado |
|-----|-------------|
| 🔵 Azul | Agendamento confirmado |
| 🟡 Amarelo | Agendamento pendente |
| 🔴 Vermelho | Bloqueio |
| 🟢 Verde | Horário disponível |

## Múltiplos Estabelecimentos

Se você tem mais de uma unidade:

### Criando novo estabelecimento

1. Na lista de estabelecimentos, clique em **Novo Estabelecimento**
2. Preencha todas as informações
3. Configure horários e bloqueios
4. Vincule profissionais e serviços

### Gerenciando múltiplas unidades

- Cada estabelecimento tem seus próprios profissionais
- Serviços podem ser compartilhados ou exclusivos
- Bots podem atender um ou múltiplos estabelecimentos

## Boas Práticas

### ✅ Faça

- Mantenha informações de contato atualizadas
- Configure horários corretamente
- Adicione bloqueios com antecedência
- Use uma foto/logo do estabelecimento

### ❌ Evite

- Deixar campos obrigatórios em branco
- Esquecer de atualizar horários de feriados
- Bloquear datas sem avisar clientes com antecedência

---

## Próximos Passos

- 📖 [Guia de Serviços](/app/tutorials?doc=guides/servicos) - Configure o que você oferece
- 📖 [Guia de Profissionais](/app/tutorials?doc=guides/profissionais) - Adicione sua equipe
- 📖 [Guia de Bots](/app/tutorials?doc=guides/bots) - Crie seu assistente virtual
