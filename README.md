# Análise do Risco de Inadimplência.

Objetivo: Este trabalho tem como objetivo aumentar o número de contratos de uma Fintech, com diminuição do Risco de Inadimplência.

## 1 – Introdução 

Trata-se de um trabalho de análise de dados, utilizando o Excel da Microsoft como ferramenta, buscando-se, através de aplicação de métodos estatísticos, responder a uma necessidade de uma empresa Fintech.

## 2 – Contextualização 

Uma Fintech de Crédito iniciou sua operação de concessão de empréstimo pessoal e acompanhou a performance de pagamento de 1.000 clientes após 1 ano. Com base nessa amostra, solicitou uma Análise de Dados para verificar quais os fatores de risco dos clientes, de forma a conseguir aprovar mais contratos com a menor inadimplência possível.

## 3 – Metadados: 

Inadimplencia - 1 se cliente ficou inadimplente em algum momento após o empréstimo ou 0 caso contrário;

Idade - Idade do cliente:

Sexo - H: Homem e M: Mulher;

Escolaridade - Medio, Graduação e Pós Graduação; 

Tipo_Moradia - Se mora de favor, paga aluguel ou tem casa própria;

Saldo_Investimento - Tomador possui alguma conta investimento em outro banco e qual sua faixa de saldo; 

Saldo_Conta_Corrente - Se tomador possui alguma conta corrente em outro banco e qual sua faixa de saldo; 

Valor_Emprestimo - valor do empréstimo pessoal solicitado; 

Duracao_Emprestimo - Duração em meses do empréstimo pessoal solicitado.


## 4 – Metodologia 
A metodologia adotada consistiu em uma abordagem inicial baseada na teoria frequentista, seguida por uma análise de Information Value (IV) para uma análise bivariada mais aprofundada. Abaixo a descrição dessa metodologia:

### 4.1 - Análise univariada usando a teoria frequentista.
A primeira etapa foi conduzir uma análise univariada, examinando cada variável independentemente. Utilizou-se a abordagem da teoria frequentista para analisar as proporções e frequências das categorias em cada variável. Foram calculados os percentuais de ocorrência de cada categoria e as proporções de resposta (inadimplência) em relação a cada categoria. Essa análise permitiu ter uma visão geral das características individuais de cada variável e sua relação com a variável resposta (inadimplência).

### 4.2 - Análise bivariada usando o Information Value (IV).
Após a análise univariada, foi realizada uma análise bivariada usando o conceito de Information Value (IV). 
O IV é uma medida estatística que avalia a importância de cada variável independente em relação à variável resposta (inadimplência). 
O cálculo do IV envolve a comparação das proporções de resposta (inadimplência) para cada categoria da variável independente, em relação à proporção geral de resposta. Com base no cálculo do IV, foi possível determinar o grau de influência de cada variável independente na inadimplência, classificando-as em termos de sua importância para a predição do risco de inadimplência. 
Essa metodologia permitiu uma abordagem sistemática para a análise dos dados, começando com uma análise univariada para entender as características individuais de cada variável e, em seguida, realizando uma análise bivariada usando o IV para identificar as variáveis que mais contribuíam para a predição da inadimplência. 
Essa abordagem é eficaz para destacar as variáveis mais relevantes e auxiliar na tomada de decisões estratégicas para reduzir a inadimplência e aumentar o número de contratos de forma mais precisa.

## 5 - Análise dos resultados. 

Nesta seção, serão apresentados os principais resultados obtidos a partir da análise dos dados.

### 5.1 – Gráficos desenvolvidos durante a análise exploratória univariada. 
Encontra-se na aba Univariada da Planilha Base_Inadimplencia V5.xlsx.

### 5.2 - Tabela com as variáveis ordenadas pelo Valor de Informação (IV), destacando aquelas com maior poder preditivo em relação à inadimplência. 
Encontra-se na aba Bivariada da Planilha Base_Inadimplencia V5.xlsx.

### 5.3 - Aprofundando a análise com a utilização de Feature Engineering.

No arquivo Base, foi adicionada uma coluna combinando os valores das features Saldo_Invest + Saldo_CC, podendo-se assim, obter maiores detalhes da influência dessas duas variáveis, agora em conjunto, no risco que elas podem gerar para o aumento da inadimplência.

Ao observar-se abaixo, a TABELA apresentada na aba **Análise_Bi2**, da Planilha Base_Inadimplencia V5.xlsx, podemos ver as diferentes categorias da variável "Saldo_Invest + Saldo_CC" e as proporções de resposta correspondentes para cada categoria. Além disso, são fornecidos os percentuais de resposta (inadimplência) para cada categoria, bem como as proporções esperadas de resposta para cada uma.

![image](https://github.com/Mrogerioventura/Analise_Inadimplencia_Fintech/assets/67667695/69277208-f467-487c-a171-9d6800106b5e)



Aplicando-se o cálculo do IV, obtemos um valor de 0,8048. Esse valor indica uma influência significativa da variável "Saldo_Invest + Saldo_CC" na inadimplência dos clientes. 

É importante ressaltar que o IV não apenas quantifica a importância da variável, mas também indica a direção da relação. No caso em análise, observa-se que as categorias com maiores valores de IV (como "Pouco-Pouco" e "Pouco-Sem conta") estão associadas a uma maior proporção de inadimplência, enquanto categorias com valores menores de IV (como "Alto-Alto" e "Moderado-Alto") estão associadas a uma menor proporção de inadimplência.

Com base nesses resultados, conclui-se que a variável "Saldo_Invest + Saldo_CC" desempenha um papel significativo na predição da inadimplência dos clientes. Portanto, ao desenvolver estratégias para aprovar mais contratos com a menor inadimplência possível, é importante considerar e avaliar cuidadosamente essa variável, levando em conta as características e os riscos associados a cada categoria.

## 6 - Recomendações e Plano de Ação sugerido. 

Com base nos resultados da análise, foram apresentadas recomendações específicas para a empresa com o objetivo de aumentar o número de contratos sem aumentar a inadimplência, conforme o Plano de Ação, conforme aba Plano de Ação da Planilha Base_Inadimplencia V5.xlsx.


## 7 - Limitações e recomendações para estudos futuros. 
Sabemos como é importante reconhecer que o trabalho não termina com a análise de dados, e é primordial identificar oportunidades para melhorias futuras.

Alguns pontos observados que devem ser levados em conta:

• Tamanho da amostra: No momento era o que possuíamos para o desenvolvimento do trabalho, mas um estudo futuro poderá ser realizado para verificação do quanto a amostra de 1.000 clientes é representativa o suficiente para extrapolar os resultados para toda a população.

• Outras variáveis: Assim como o quantitativo da amostra, poder-se-á identificar variáveis adicionais que podem ser relevantes para uma nova análise e que não foram incluídas nos dados fornecidos. Sugerimos uma reunião como cada time de negócio, que conjuntamente poderão considerar essas novas variáveis;

• Melhoria contínua: A análise de dados é um processo contínuo em que os resultados obtidos devem ser monitorados e revisados regularmente para garantir a eficácia das estratégias implementadas.

Esses tópicos adicionais fornecerão um contexto mais completo e aprofundado para o relatório, permitindo que a empresa compreenda melhor os resultados da análise de dados e tome decisões informadas para melhorar suas políticas e processos relacionados à concessão de empréstimos.




