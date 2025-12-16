App de Organização de Finanças Pessoais criado por Fabio Pedrão

PRD Refinado com o Microsoft Copilot Web.

````Markdown
# Documento de Requisitos do Produto (PRD)  
**Módulo Central de Lançamentos e Extrato – Finanças Fácil (Lovable)**  

### Campo | Descrição  
- **Status do PRD**: Rascunho  
- **Data de Criação**: 15 de Dezembro de 2025  
- **Proprietário do Produto**: [Seu Nome]  
- **Público-Alvo**: Usuários existentes que precisam de uma interface de lançamento rápido e visualização de extrato  

---

## 1. Visão Geral (Overview)  
Este módulo centraliza a experiência do usuário em uma única tela, permitindo:  
- Lançamentos rápidos de gastos (💸) e receitas (💰).  
- Visualização imediata do extrato recente.  
- Acesso rápido a ferramentas como metas (🎯) e o Agente IA (✨).  

A interface deve ser **intuitiva, mobile-first e com feedback visual imediato**, substituindo a navegação por abas por **botões de ação** e **conteúdo dinâmico**.  

---

## 2. Metas do Produto (Goals)  
- **KPI Principal**: Aumentar a frequência de lançamentos diários de transações em 20% em 30 dias.  
- **Métrica de Engajamento**: Reduzir a taxa de rejeição da tela principal em 15%.  
- **Qualitativo**: Proporcionar uma UX mais fluida e moderna, com menos cliques para a ação principal (lançar gasto/receita).  

---

## 3. Requisitos Funcionais (Functional Requirements)  

### 3.1. Header e Saldo  
- **FR-H1**: Exibir o “Saldo Disponível” atualizado em tempo real.  
- **FR-H2**: Design limpo, fundo na cor principal (#064e3b).  

### 3.2. Botões de Ação (Menu Grid)  
- **FR-B1**: Grid com 4 botões: “Gasto” (💸), “Receita” (💰), “Metas” (🎯) e “IA” (✨).  
- **FR-B2**: Cada botão deve renderizar conteúdo na “Área de Detalhes Dinâmicos”.  
- **FR-B3**: Feedback visual ao pressionar (efeito scale(0.9) ou similar).  

### 3.3. Extrato Recente  
- **FR-E1**: Exibir últimas 3 a 5 transações abaixo dos botões.  
- **FR-E2**: Cada item mostra ícone, descrição, data/hora e valor.  
- **FR-E3**: Gastos em vermelho (#ef4444); receitas em verde (#059669).  
- **FR-E4**: Botões de ação em itens pendentes (ex.: “Pagar”, “Receber”).  

### 3.4. Área de Detalhes Dinâmicos  
- **FR-D1**: Área abaixo do extrato para formulários ou informações adicionais.  
- **FR-D2**: Ao clicar em “Gasto” ou “Receita”, exibir formulário de input.  
- **FR-D3**: Card muda de cor conforme ação (verde para receita, azul petróleo para gasto/info geral).  

---

## 4. Requisitos Não Funcionais (Non-Functional Requirements)  
- **NFR-P1**: Interface responsiva e otimizada para mobile.  
- **NFR-P2**: Renderização instantânea (máx. 300ms de animação).  
- **NFR-S1**: Autenticação obrigatória para acesso (fora do escopo deste módulo, mas necessária para integração).  

---

## 5. Wireframes e Mockups  
Um protótipo HTML/CSS/JS foi desenvolvido como base para implementação visual e funcionalidade básica.  
- Estrutura: header com saldo, grid de botões, extrato recente e área dinâmica.  
- Feedback visual: botões com efeito de escala, cards com cores contextuais.  
- Exemplo: botão 💸 abre formulário de gasto; botão 💰 abre formulário de receita.  

**Código para referência e cópia:**

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Finanças Fácil - Extrato c/ Ganhos</title>
  <!-- estilos e script completos conforme versão anterior -->
</head>
<body>
  <!-- header, grid de botões, extrato e área dinâmica -->
</body>
</html>
````

>>interação com o site Lovable
>>Foi criado um app de funcionalidade facil onde com os creditos provavel foi sendo refinado
>>durante a criação as metas e a ia não funcionaram sendo solicitado ao Lovable que corrigi-se, acabando assim os creditos restantes.
>>Resultado Final no Lovable:  https://easy-money-center.lovable.app
>><img width="481" height="788" alt="image" src="https://github.com/user-attachments/assets/b35ad424-cc88-43c2-9522-7e9aa8592e3f" />
>><img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0060ef21-8ba4-49b7-b8d0-d74670e551b6" />
>><img width="472" height="680" alt="image" src="https://github.com/user-attachments/assets/43151a04-030e-4feb-a3d1-be8f2681c71b" />

# Finanças Fácil – Visão Geral de Funcionalidades
Finanças Fácil é um aplicativo de gestão financeira pessoal com foco em simplicidade, agilidade e inteligência. A interface é mobile-first e oferece uma experiência fluida com assistente virtual integrado.

---
## 🧾 Funcionalidades Principais

### 💰 Saldo Disponível
- Exibição clara do saldo atual no topo da tela.
- Atualização visual imediata.
### 🔘 Menu de Ações Rápidas
- Quatro botões principais para navegação:
  - **💸 Gasto**: registrar uma nova despesa.
  - **💰 Receita**: registrar uma nova entrada de dinheiro.
  - **🎯 Metas**: acompanhar metas financeiras.
  - **✨ IA**: acessar o assistente virtual Fina.
### 🤖 Assistente IA – Fina
- Apresentação amigável:  
  “Olá! Sou a Fina, sua assistente financeira. Posso ajudar você a entender seus gastos, criar orçamentos e dar dicas personalizadas.”
- Sugestões de comandos prontos:
  - “Como posso economizar mais?”
  - “Analise meus gastos do mês”
  - “Dicas para investir”
- Campo de texto para perguntas personalizadas.
### 📄 Extrato Recente
- Lista das últimas transações com:
  - Nome da categoria (ex.: mercado, salário)
  - Data e hora
  - Valor (em vermelho para gastos, verde para receitas)
### 🧩 Área de Detalhes Dinâmicos
- Exibe formulários ou respostas conforme o botão clicado.
- Cores adaptadas à ação:
  - Verde para receita
  - Azul petróleo para gasto ou informações gerais
- Feedback visual suave com animação `fade-in`.
---
## 📱 Interface
- Design responsivo e otimizado para dispositivos móveis.
- Navegação por botões com ícones intuitivos.
- Experiência conversacional e interativa.
---
## 🚀 Objetivo
Facilitar o controle financeiro pessoal com uma abordagem leve, inteligente e acessível para todos os perfis de usuários.


##RFELEXÃO##

>> o PRD ficou muito bom no Copilot porém usei o refino dele para criar um html para ver como ficava a aparencia sendo refinada a cada instante para gerar o produto finbal com a mior facilidade de uso.
>> no site Lovable foi elaborado pelo Markdown do PRD refinado porém ao criar o app no inicio não funcionava as meta nem a ia sendo que os creditos acabaram na correção
>> o produto final ficou bom simples e facil de usar, ate mesmo meu filho gostou do produto final.

 

