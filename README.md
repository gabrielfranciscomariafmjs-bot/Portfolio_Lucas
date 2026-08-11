# 📊 E-Commerce Performance & Risk Analytics: Dashboard Executivo em Power BI

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data_Analysis_Expressions-blue?style=for-the-badge)
![Business Intelligence](https://img.shields.io/badge/Business_Intelligence-Analyst-success?style=for-the-badge)

## 📌 Visão Geral do Projeto
Este projeto é uma solução de Business Intelligence (*End-to-End*) desenvolvida para analisar a performance operacional e financeira de uma rede de E-commerce operando no Brasil entre janeiro de 2024 e o terceiro trimestre de 2026. 

O objetivo do dashboard é fornecer à diretoria executiva um controle preciso sobre a rentabilidade, gargalos logísticos regionais e simulações de cenários de risco, permitindo decisões orientadas a dados (*data-driven*).

> **Acesse o Dashboard Interativo:** [Faça o download do arquivo .pbix aqui](https://github.com/gabrielfranciscomariafmjs-bot/My_projects/raw/main/E-Commerce%20Analytics%20%26%20Business%20Intelligence%20Dashboard.pbix) para testar a navegabilidade e os filtros dinâmicos do projeto. 
> *(Requer o Power BI Desktop instalado).*
---

## 🎯 Desafios de Negócio Resolvidos

O painel foi estruturado para responder a perguntas estratégicas complexas por meio de 5 análises principais:

### 1. Diagnóstico de Rentabilidade (Causa Raiz de Margem)
* **O Desafio:** Identificar quedas na margem de lucro e suas causas reais (descartando o viés do volume de vendas).
* **A Solução:** Utilizando medidas DAX com `DIVIDE(SUM(), SUM())`, isolei a margem percentual real. O dashboard revelou que a compressão severa de margem ocorrida no **Q3 de 2025 (27,21%)** não foi causada por frete ou queda de volume, mas sim por um salto crítico no **Custo do Produto**, que consumiu 72,47% da receita naquele trimestre.
 *<img width="1255" height="794" alt="Dash 1" src="https://github.com/user-attachments/assets/8b5269ec-25ec-4ed6-b961-eb6a660379eb" />*

### 2. Análise de Risco Logístico e Satisfação
* **O Desafio:** Mapear a correlação entre atrasos/devoluções e a nota do cliente, cruzando com diferentes canais.
* **A Solução:** Aplicação do modelo visual de *Small Multiples* (Múltiplos Pequenos) para segmentar as notas por Canal de Venda. A análise provou que a correlação é universal, independente do canal: a satisfação é impulsionada apenas por entregas no prazo, enquanto atrasos anulam as avaliações máximas.
 *<img width="1153" height="791" alt="Dash 2" src="https://github.com/user-attachments/assets/ff0e60f3-9027-4b0b-8e0c-3a4664f3a012" />*

### 3. Princípio de Pareto (Curva ABC)
* **O Desafio:** Identificar quais subcategorias geram 80% do lucro total da empresa.
* **A Solução:** Desenvolvimento de um gráfico de Pareto com **Formatação Condicional Avançada**. Através de medidas DAX para cálculo de percentual acumulado, as barras mudam automaticamente de cor assim que a meta de 80% é atingida. O resultado revelou que 10 subcategorias (exclusivamente dos setores de Eletrônicos e Móveis) sustentam o negócio.
 *<img width="1313" height="631" alt="Dash 3" src="https://github.com/user-attachments/assets/2edbb864-565d-469d-b7f8-5cd1d081e78a" />*

### 4. Simulação de Cenários (What-If Parameter)
* **O Desafio:** Calcular o impacto financeiro (perda de receita e lucro) caso a empresa descontinue operações em regiões com margem de lucro abaixo de um limite definido pelo usuário.
* **A Solução:** Criação de um parâmetro de simulação conectado ao modelo de vendas. Utilizando **Tabelas Virtuais e Transição de Contexto no DAX** (`CALCULATE` iterando com `VALUES(Regiao)`), o painel avalia a margem agregada de cada região antes de aplicar o corte. O mapa regional e os KPIs reagem instantaneamente, demonstrando de forma dinâmica a perda financeira real.
 *<img width="1312" height="738" alt="Dash 4" src="https://github.com/user-attachments/assets/4ed8ef40-f3cd-4265-b5dc-d1784fb1627e" />*

### 5. Mapeamento de Risco Regional
* **O Desafio:** Diagnosticar problemas de devolução e cancelamento isolados na região Nordeste.
* **A Solução:** Através de filtros sincronizados, a análise quebrou um viés macro. Enquanto no consolidado do Brasil os Eletrônicos lideram os problemas, o filtro específico do Nordeste revelou que o grande gargalo da região é a categoria de **Vestuário**, especificamente impulsionado por um risco atípico na modalidade de **Lojas Físicas**.
 *<img width="1315" height="740" alt="Dash 5" src="https://github.com/user-attachments/assets/e5cdf25f-2d57-45b9-a14b-039007284e76" />*

### 6. Autonomia Executiva com IA Integrada (Self-Service Analytics)
* **O Desafio:** Eliminar o gargalo operacional e a dependência técnica do time de dados para responder a consultas analíticas pontuais (*ad-hoc*) da diretoria.
* **A Solução:** Integração nativa de um agente inteligente (Copilot / Q&A) na interface do dashboard. Através de uma caixa de texto, o executivo tem a liberdade de interagir com o modelo de dados em linguagem natural. Essa aplicação prática de IA e recursos conversacionais empodera a gestão a realizar investigações independentes, extraindo insights, respostas precisas e gráficos instantâneos sem a necessidade de acionar um analista de dados.

---

## 🛠️ Tecnologias e Habilidades Aplicadas

* **Ferramenta de Visualização:** Microsoft Power BI
* **Linguagens:** DAX (Data Analysis Expressions) e manipulação via Power Query (M).
* **Skills Analíticas Destacadas:**
  * Contexto de Filtro vs. Contexto de Linha (agregações dinâmicas).
  * *Sync Slicers* (Segmentadores sincronizados) para garantir fluidez na navegação executiva.
  * Storytelling com dados (uso de *Smart Narratives* e dicas de ferramentas personalizadas).
  * Design limpo (UI/UX), focado em usabilidade para tomada de decisão (sem poluição visual).
  * **Inteligência Artificial & Self-Service Analytics:** Integração de recursos do Copilot para exploração de dados em linguagem natural, promovendo autonomia executiva.

---

## 🎓 Formações e Certificações

* **Certificado Profissional Google Data Analytics** – Coursera / Google (2026)
* **Google Prompting Essentials (Inteligência Artificial)** – Coursera / Google (2026)
* **Business Intelligence com Power BI** – Witseed (2025)
* **Fundamentos de Python (Pandas, NumPy, EDA e ETL)** – Witseed (2025)
* **Liderança, Planejamento e Gestão de Pessoas (90h)** – Instituto Educacional Aprender (2026)
* **Excel Avançado** – Centro Educacional Brastemp (2024)

---
---
*Gostou do projeto ou tem alguma dúvida sobre as análises? Sinta-se à vontade para conectar-se comigo!*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-santana-98251325a)
[![E-mail](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lucas_santana321@outlook.com)
