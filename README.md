# Hangdamn

APS 7 - Algebra Linear e Teoria da Informação - 2023.1

## Integrantes do grupo
* [Gustavo Lindenberg](https://github.com/gustavolp1)


TROCAR TUDO LALALALALALALALALALLALA





# Índice
1. [Introdução](#introdução)
2. [Análise dos dados](#análise-dos-dados)
3. [Conclusões](#conclusões)
4. [Bibliografia](#bibliografia)

# Introdução

Por meio de classificadores, é possível determinar resultados a partir de dados específicos. Este projeto possui o objetivo de avaliar um classificador de fatores de risco para o acidente vascular cerebral (AVC). Ou seja, qualquer fator que aumente o risco de um indivíduo ter uma emergência como essa impactará o resultado. Para isso, utilizaremos as bibliotecas sklearn e autograd em python para gerar os impactos de cada um dos fatores analisados.

## Análise dos dados

Analizando os dados adquiridos no preditor de AVC, o valor com o relação mais alta com esse acidente vascular é a hipertensão, que é uma doença que afeta as artérias, seguido por ter um trabalho privado e estarem casados. Os dados encontrados estão abaixo:

* `hypertension` 1.9161797751759362
* `work_type_Private` 1.2220087468386893
* `work_type_Govt_job` 0.8501062047083867
* `ever_married_Yes` 0.7942305423397298
* `bmi` 0.04353848245863595
* `avg_glucose_level` 0.0032088682736495047
* `age` -0.023799024835772634
* `heart_disease` -0.03574279385007104
* `work_type_Never_worked` -0.10596010452077866
* `gender` -0.15203185531201022
* `smoking_status_smokes` -0.15463364674369248
* `Residence_type_Urban` -0.19160052444727962
* `smoking_status_formerly smoked` -0.3487340675519495
* `work_type_Self-employed` -0.43877985033056516
* `work_type_children` -0.8395988620444941
* `smoking_status_never smoked` -0.9365968419217553
* `smoking_status_Unknown` -1.2835729696956033
 
## Conclusões

Com os dados obtidos, conseguimos comparar os nossos resultados com outras pesquisas sobre o AVC e nossa arvore de decisões. O fator com relação mais alta é a hipertensão, que aparece como um dos fatores mais influenciais de aumentar o risco de um AVC em múltiplas pesquisas, pois ambos são problemas que acontecem em artérias e veias. Seguidamente, as pessoas que trabalham (considerando somente trabalhos não autonomos) tem chances muito maiores de ter essa emergência, que de acordo com as pesquisas feitas há uma relação entre AVC e estresse, e relação entre estresse e o trabalho; isso então pode ser relacionado com outras pesquisas que encontraram relações entre trabalho e estresse. Adicionalmente, foi encontrada uma relação com AVC e a pessoa estar casada, o que pode ser atribuido ao estress novamente, mas não há dados em outras pequisas o suficiente para afirmar que realmente há uma relação, e poderia ser algo que aparece somente neste dataset.

Além dos maiores valores de relação, podemos perceber que houve uma classificação diferente com o fumo, apesar de ainda estar dentro do esperado. As pessoas que fumam não mostraram relação com AVC, mas aqueles que não fumam mostraram uma relação inversa, ou seja, não fumar faz com que suas chances de ter um AVC diminuem. Outros fatores, como ser criança, tambem mostraram uma forte relação inversa com o AVC.

## Análise da Árvore

A árvore gerada pelo código confirma mostra, de cima para baixo, os fatores de mais relevância para se ter um AVC. É possível perceber que o tipo de trabalho, da mesma forma que a hipertensão e altos níveis de glicose, aumentam a chance de um AVC. Os dados apresentados na árvore, apesar de não terem a mesma ordenação que nosso classificador, apontam para a relevância dos fatores que encontramos atráves da regresão linear.

![Alt Text](output.png)


# Bibliografia 

1. [CDC Stroke risks and prevention](https://www.cdc.gov/stroke/risk_factors.htm#:~:text=These%20health%20conditions%20include%20obesity,and%20the%20risk%20for%20stroke.)
1. [Can Stress Cause a Stroke?](https://batonrougeclinic.com/can-stress-cause-a-stroke/#:~:text=Study%20participants%20who%20reported%20the,modest%20increases%20raised%20stroke%20risk.)
1. [Can work stress be linked to Stroke?](https://batonrougeclinic.com/can-stress-cause-a-stroke/#:~:text=Study%20participants%20who%20reported%20the,modest%20increases%20raised%20stroke%20risk.)
1. [Stroke prediction](https://www.kaggle.com/code/ahmedterry/stroke-prediction-eda-classification-models)