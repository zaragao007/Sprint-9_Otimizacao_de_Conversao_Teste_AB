# 📈 Otimização de Conversão (CRO) e Teste A/B - E-commerce

## 🎯 Contexto do Projeto
Como analista de uma grande loja online, fui encarregado de trabalhar junto ao departamento de marketing para alavancar a receita. O projeto foi dividido em duas fases críticas: primeiro, aplicar frameworks de priorização (ICE/RICE) para descobrir qual hipótese testar primeiro; segundo, conduzir uma análise estatística rigorosa de um Teste A/B para validar os resultados no mundo real.

Este projeto destaca o uso de estatística inferencial (Teste de Mann-Whitney) na tomada de decisão em negócios, separando o "ruído" (anomalias/outliers) do sinal verdadeiro de crescimento.

## 🔗 Links Rápidos
* **[Painel Executivo: Monitoramento de CRO (Tableau Public)](https://public.tableau.com/app/profile/marcelo.aragao/viz/CRO_AB_Test_Monitoring_Sprint9/MonitoramentodeCROTesteAB?publish=yes)**
* **[Apresentação Executiva do Teste A/B (PDF)](Apresentacao_Executiva_TesteAB.pdf)**

## 🛠️ Ferramentas e Tecnologias
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, SciPy (Estatística), Matplotlib
* **Visualização de Negócios:** Tableau
* **Técnicas Estatísticas:** Frameworks ICE/RICE, Cálculo de Percentis (95 e 99), Teste U de Mann-Whitney, P-values, Filtragem de Outliers.

## 📂 Estrutura do Repositório
* `Apresentacao_Executiva_TesteAB.pdf`: Resumo executivo com a recomendação final de negócios.
* `Sprint-9_Notebook.ipynb`: Motor analítico em Python (limpeza, cálculo de anomalias e testes de hipótese estatísticos).
* `dados_ab_test_tableau.csv`: Dados diários acumulados exportados do Python para visualização no Tableau.
* `hypotheses_us.csv`, `orders_us.csv`, `visits_us.csv`: Bases de dados brutas.
* `requirements.txt`: Dependências do projeto.

## 💡 Principais Insights Analíticos
1. **O Peso do Alcance (RICE vs ICE):** A hipótese de "Adicionar formulário de assinatura" saltou para o topo da prioridade quando o framework RICE foi aplicado, provando que o alcance (Reach) é um fator multiplicador crucial que não pode ser ignorado.
2. **A Vitória na Conversão:** O Grupo B superou o Grupo A em taxa de conversão de forma consistente e estatisticamente significante, indicando que a alteração testada atrai mais compradores.
3. **O Impacto das Anomalias:** O teste capturou uma compra gigantesca no dia 19 de agosto no Grupo B. A análise estatística provou que, mesmo removendo esse outlier extremo da base, o Grupo B continua sendo o vencedor isolado em taxa de conversão, sem perder no ticket médio.

## 🚀 Decisão de Negócios (Veredito)
**Recomendação:** Parar o teste e declarar o Grupo B como o vencedor.
O Grupo B gera um volume maior de compradores (maior conversão) e entrega mais receita total para a empresa, sem diminuir o valor gasto por pedido (ticket médio). A implementação da variante B deve ser colocada em produção.

---
*Desenvolvido por Marcelo - Analista de Dados*
