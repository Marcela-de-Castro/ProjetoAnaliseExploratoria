# ProjetoAnaliseExploratoria
PROJETO – ANÁLISE EXPLORATÓRIA E ESTATÍSTICA DE  DADOS

CENÁRIO 
Você é um analista de dados contratado por uma loja de varejo com o objetivo de analisar os dados de vendas e fornecer insights que possam ajudar a melhorar as operações e o desempenho da loja. Além de descrever o que os dados mostram, a diretoria pediu que as conclusões venham acompanhadas de evidência estatística — ou seja, que você quantifique a incerteza das suas estimativas e teste formalmente as hipóteses de negócio antes de recomendar qualquer ação. 

CONJUNTO DE DADOS 
Para isso, você teve acesso aos dados que incluem informações diárias sobre vendas, categorias de produtos, preços, quantidades vendidas, descontos aplicados e algumas características de clientes (idade e renda) do último ano de operação da empresa. 

OBJETIVO 
Sua missão é avaliar os dados e responder às perguntas levantadas pela equipe de marketing, listadas abaixo. As respostas devem combinar Estatística Descritiva (para caracterizar e resumir o comportamento dos dados) e Estatística Inferencial (para testar hipóteses e generalizar conclusões além da amostra observada), sempre justificando o teste ou medida escolhida e interpretando o resultado no contexto do negócio — não bastam apenas números soltos. 

Perguntas de negócio (equipe de marketing) 
1. Quais foram as categorias produtos mais vendidos e em quais meses eles tiveram o maior pico de vendas? 
2. Qual foi o impacto das promoções (descontos aplicados) nas vendas? Quais produtos tiveram o maior aumento nas 
vendas durante as promoções? 
3. Qual a média de vendas diárias por categoria de produto? 
4. Quais produtos apresentam a maior sazonalidade nas vendas (ex.: frutas e vegetais, sorvetes)? 
  a. Para responder essa pergunta considere a medida de sazonalidade dada pelo coeficiente de variação mensal 
  dos produtos.
5. Quais as faixas etárias contribuíram mais para as vendas totais? 
  a. Para responder essa pergunta, crie uma coluna com a faixa etária, considerando: entre 18 e 35 (jovem), entre
  36 e 59 (adulto) e acima de 60 anos (idoso). 
6. Qual a distribuição das vendas ao longo dos dias da semana? 
7. Como as vendas mensais se comparam antes e durante a Black Friday? 
8. Qual é o ticket médio (valor médio das vendas) por faixa etária e como ele varia entre diferentes categorias de produto? 
9. Qual é a relação entre a idade dos clientes e o valor total das compras? 
10. Comparando a semana da "Black Friday" com a do Natal, qual semana a empresa teve melhores desempenhos em 
relação à média de vendas? 

REQUISITOS DE ESTATÍSTICA DESCRITIVA 
Antes (ou como parte) de responder às perguntas de negócio, apresente uma caracterização descritiva completa da base, incluindo: 
• Medidas de tendência central (média, mediana e moda) e de dispersão (desvio-padrão, variância, amplitude, 
coeficiente de variação) para as variáveis numéricas: preço, quantidade vendida, desconto, valor total da venda, idade e renda. 
• Medidas separatrizes (quartis, percentis) e identificação de outliers via boxplot e/ou regra do IQR (1,5×IQR) e/ou z score, discutindo se os outliers devem ser mantidos, tratados ou removidos. 
• Análise da forma da distribuição (histograma, assimetria/skewness e curtose) das variáveis-chave (ex.: valor da venda, idade), indicando se aparentam seguir uma distribuição normal. 
• Tabelas de frequência (absoluta e relativa) para variáveis categóricas: categoria de produto, faixa etária, dia da semana, mês. 
• Matriz de correlação (Pearson e/ou Spearman) entre as variáveis numéricas, com um mapa de calor (heatmap), 
destacando as correlações mais relevantes para as perguntas de negócio. 
Cada medida apresentada deve vir acompanhada de uma frase interpretativa (o que ela significa no contexto da loja), não apenas do valor numérico.

REQUISITOS DE ESTATÍSTICA INFERENCIAL 
Além de descrever os dados, valide estatisticamente as principais conclusões de negócio, respondendo também às 
perguntas abaixo, usando testes de hipótese simples (comparação de dois grupos, no formato de teste A/B). Para cada teste, declare claramente a hipótese nula (H0) e a alternativa (H1), o nível de significância adotado (sugestão: α = 0,05) e interprete o resultado (estatística do teste, p-valor e conclusão em termos de negócio). 
11. O aumento nas vendas durante períodos de promoção (descontos) é estatisticamente significativo, ou pode ser 
explicado por variação aleatória? Utilize um teste A/B comparando o valor médio das vendas do grupo com desconto 
(B) contra o grupo sem desconto (A). 
12. O desempenho de vendas da semana da Black Friday é estatisticamente diferente do desempenho da semana do 
Natal (pergunta 10), ou a diferença pode ser explicada por variação natural entre semanas? Utilize um teste A/B 
(teste t para duas amostras independentes) comparando as vendas diárias das duas semanas, e construa também 
intervalos de confiança de 95% para a média de vendas diárias de cada uma. 
13. Qual é a estimativa, com 95% de confiança, do ticket médio geral da loja e do ticket médio por faixa etária? Construa os intervalos de confiança correspondentes e discuta o que a amplitude de cada intervalo revela sobre a variabilidade do comportamento de compra em cada grupo.
14. O aumento de vendas durante a Black Friday (pergunta 7) é estatisticamente significativo, ou pode ser explicado por variação natural entre meses? Utilize um teste A/B comparando o valor médio de vendas no mês da Black Friday com o mês anterior. 

ENTREGÁVEIS 
• Notebook (Python) ou script comentado com todo o código de limpeza, estatística descritiva e testes inferenciais. 
• Relatório executivo (não técnico) traduzindo os resultados estatísticos em recomendações de negócio para a equipe de marketing. 
• Anexo com as hipóteses (H0/H1), estatísticas de teste, p-valores e intervalos de confiança de cada teste realizado, para fins de auditoria/reprodutibilidade da análise.
