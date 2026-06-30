# ConSorAI: Copiloto de Vendas com IA para Consórcios e Serviços Financeiros 🚀

## 📋 Sobre o Projeto
O **ConSorAI** é um assistente cognitivo desenhado especificamente para apoiar consultores comerciais e vendedores do mercado de consórcios e produtos financeiros de alto valor agregado (Imóveis e Veículos). 

Diferente de um chatbot tradicional focado no cliente final, o ConSorAI atua como um **Copiloto de Vendas (B2B2C)**. Ele mune o vendedor de argumentos técnicos em tempo real, formata propostas financeiras de alto impacto para o WhatsApp e fornece as melhores táticas para desarmar as objeções mais complexas do mercado financeiro (como a comparação direta com financiamentos bancários e o medo do tempo de contemplação).

---

## 👥 Usuário Principal da Solução
* **Consultores Comerciais / Vendedores de Consórcio:** Profissionais que lidam diariamente com leads frios ou mornos vindos de campanhas de tráfego pago (Google Ads/Meta) e precisam de respostas rápidas, persuasivas e matematicamente embasadas para fechar negócios no ambiente digital.

---

## 🛠️ Problema que a Solução Resolve
1. **Perda de Leads por Demora na Resposta:** Clientes no WhatsApp exigem respostas imediatas sobre cálculos de parcelas e lances.
2. **Falta de Argumentação Técnica Complexa:** Vendedores juniores ou sob pressão muitas vezes não conseguem explicar conceitos como *Lance Embutido* ou *CET (Custo Efetivo Total)* de forma simples e persuasiva.
3. **Barreira da Ansiedade por Contemplação:** O lead hesita em comprar porque "não quer esperar o sorteio". O copiloto cria estratégias personalizadas de lances para contornar essa insegurança.

---

## 🤖 Abordagem Utilizada
O projeto foi modelado sob o conceito de **Copiloto de IA baseado em Base de Conhecimento RAG (Retrieval-Augmented Generation)**. Ele funciona recebendo dados estruturados do negócio e aplicando técnicas de engenharia de prompt para gerar respostas táticas prontas para o vendedor utilizar.

### Arquitetura de Conhecimento do Projeto:
A inteligência do modelo é alimentada por uma estrutura modular na pasta `knowledge/`:
* `contexto_negocio.md`: Regras do produto, mecânicas de lances e diferenciais financeiros.
* `perguntas_frequentes.md`: Respostas diretas para dúvidas operacionais de clientes.
* `quebra_objecoes.md`: Matriz de contra-argumentação comercial focada em conversão.

---

## 💬 Exemplo Prático de Uso (Prompt & Resposta da IA)

### Cenário de Uso do Vendedor:
O vendedor recebe a seguinte mensagem de um lead no WhatsApp: 
*"Achei o plano de consórcio imobiliário legal, mas meu gerente do banco disse que a Taxa de Administração de 15% de vocês é muito alta e que compensa mais eu fazer um financiamento direto com ele."*

O vendedor aciona o **ConSorAI** enviando a dúvida do cliente.

### 🧠 Prompt de Comando do Copiloto (System Prompt):
```text
Atue como o ConSorAI, o copiloto de vendas de elite. Seu objetivo é analisar a dúvida comercial enviada pelo vendedor, consultar as matrizes em `knowledge/` e gerar duas coisas:
1. Uma análise de estratégia interna para o vendedor saber como conduzir o fechamento.
2. Uma sugestão de mensagem formatada pronta para o WhatsApp, utilizando gatilhos de urgência, clareza financeira e formatação limpa (negritos e emojis moderados).
