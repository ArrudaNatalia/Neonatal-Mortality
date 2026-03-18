# Neonatal Mortality
Classificação de risco de mortalidade neonatal no Brasil (2006-2016) utilizando Machine Learning (Random Forest, XGBoost e SVM) em dados do SINASC e SIM via linkage.

# Classificação de Risco de Mortalidade Neonatal no Brasil: Uma Abordagem de Machine Learning

Este projeto investiga a associação entre características maternas, assistência à gestação/parto e condições do recém-nascido com o risco de mortalidade neonatal no Brasil entre 2006 e 2016.

## 📌 Visão Geral
A mortalidade neonatal (até 28 dias de vida) é um fenômeno complexo que exige análise de grandes volumes de dados. Este estudo utiliza métodos inovadores de aprendizado de máquina para identificar os principais preditores de risco, utilizando bases de dados nacionais integradas.

## 🗂️ Metodologia
* **Dados:** Integração entre o Sistema de Informação sobre Nascidos Vivos (SINASC) e o Sistema de Informações sobre Mortalidade (SIM) via *linkage*.
* **Amostra:** 302.943 registros (base balanceada).
* **Algoritmos Testados:**
    * Random Forest (RF)
    * Extreme Gradient Boosted Trees (XGBoost)
    * Support Vector Machine (SVM)
* **Métricas de Avaliação:** Precisão, Sensibilidade, Especificidade e Área sob a Curva ROC (AUC).

## 🚀 Principais Resultados
Os modelos identificaram que as variáveis relacionadas ao recém-nascido e à assistência são as mais críticas para a sobrevivência:
1. **Peso ao nascer**
2. **Apgar (1º e 5º minuto)**
3. **Malformações congênitas**
4. **Idade gestacional**
5. **Número de consultas pré-natal**

*Nota: Variáveis puramente maternas apresentaram menor importância relativa na classificação de risco imediato.*

## 🛠️ Tecnologias Utilizadas
* **R:** Implementação original dos modelos.
* **Python:** Scripts para portabilidade e deploy (Scikit-Learn, XGBoost).
* **Linkage de Dados:** Processamento de bases governamentais de larga escala.

## 📈 Conclusões
O uso de Machine Learning neste contexto é inovador no Brasil. Os achados reforçam que estratégias voltadas para a qualificação da assistência no pré-natal e no momento do parto são fundamentais para ampliar a sobrevivência infantil nos primeiros 28 dias de vida.

## 📂 Como utilizar este repositório
1. Clone o repositório: `git clone https://github.com/seu-usuario/mortalidade-neonatal-brasil.git`
2. Os scripts de modelagem estão localizados na pasta `/src`.
3. Certifique-se de ter as dependências instaladas: `pip install -r requirements.txt`.

---
*Estudo desenvolvido no período de 2006 a 2016.*
