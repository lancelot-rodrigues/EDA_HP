# Challenge Sprint - HP: Análise de Anúncios de Cartuchos

Este repositório contém o desenvolvimento do Challenge Sprint para a HP, focado na análise, exploração e, futuramente, na modelagem de dados de anúncios de cartuchos de tinta coletados em sites de e-commerce.

O objetivo final do projeto é desenvolver uma solução de inteligência artificial capaz de classificar anúncios, identificando automaticamente características importantes como originalidade, tipo de produto e potenciais inconsistências.

---

## Entregável 2: Análise Exploratória e Descritiva dos Dados

Este diretório corresponde à entrega do **Sprint 2**. Nesta fase, nosso foco foi realizar uma Análise Exploratória de Dados (EDA) profunda sobre o conjunto de dados coletado. O notebook `(coloque-o-nome-do-seu-notebook-aqui.ipynb)` documenta todo o processo, que incluiu:

*   **Limpeza e Preparação dos Dados:** Tratamento de valores nulos, conversão de tipos de dados e formatação das colunas.
*   **Análise Visual:** Geração de gráficos para entender a distribuição de preços, a frequência de rótulos, as correlações entre variáveis e os termos mais comuns nos textos dos anúncios.
*   **Extração de Insights:** Interpretação dos gráficos para entender o comportamento do mercado e a estrutura dos anúncios.
*   **Identificação de Features:** Levantamento de um conjunto inicial de características (features) promissoras que servirão de base para a etapa de modelagem no próximo sprint.

---

## Sobre o Conjunto de Dados

O arquivo `ml_produtos_hp_final_features_target.csv` utilizado nesta análise é o mesmo dataset gerado e enriquecido durante o **Sprint 1**.

É importante frisar que o tamanho do dataset foi **propositalmente mantido reduzido** nesta fase do projeto. Esta abordagem nos permite ter maior agilidade e eficiência no desenvolvimento, facilitando a prototipação rápida, a validação de hipóteses e a iteração sobre o código de limpeza e análise sem a sobrecarga computacional de um grande volume de dados.

### Visão Futura do Dataset

Para a solução final do projeto, o plano é expandir significativamente nossa base de dados. Pretendemos realizar uma coleta de dados muito mais abrangente, que incluirá não apenas um volume maior de anúncios do Mercado Livre, mas também dados de **outros sites de e-commerce relevantes**. Isso garantirá que nosso modelo final seja mais generalista, robusto e representativo do mercado como um todo.

---

## Como Executar o Notebook

1.  **Pré-requisitos:** O notebook foi desenvolvido para ser executado no ambiente do Google Colab.
2.  **Clone o Repositório:** Faça o download ou clone este repositório para sua máquina local.
3.  **Abra no Colab:** Acesse o [Google Colab](https://colab.research.google.com/) e faça o upload do arquivo `.ipynb`.
4.  **Carregue os Dados:** A primeira célula de código executável do notebook solicitará o upload do arquivo `ml_produtos_hp_final_features_target.csv`. Selecione o arquivo correspondente.
5.  **Execute as Células:** Execute as células sequencialmente para reproduzir toda a análise.

---

## Principais Conclusões da Análise

*   **Padrões de Preço:** A distribuição de preços indica a existência de grupos distintos de produtos, como cartuchos individuais e kits promocionais.
*   **Qualidade dos Rótulos:** A base de dados se mostrou bem diversificada, contendo desde anúncios claramente "originais" e "compatíveis" até casos ambíguos, ideais para o treinamento de um modelo robusto.
*   **Insights das Descrições:** A análise textual revelou que, além de termos esperados como "qualidade" e "rendimento", a palavra "recarga" é surpreendentemente comum, validando a necessidade de classificar os anúncios.
*   **Correlações e Alertas:** A matriz de correlação confirmou relações lógicas (preço x rendimento) e, mais importante, levantou um alerta sobre a qualidade dos dados na coluna `volume_num`, indicando um ponto de atenção para a fase de engenharia de features.

---

## Grupo

*   Lancelot Chagas Rodrigues / 554707
*   Ana Carolina Martins da Silva / 555762
*   Kauan Alves Batista / 555082
