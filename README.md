# 📊 Projeto — Aprendizado de máquina a partir do desastre do Titanic

<img width="1408" height="768" alt="Gemini_Generated_Image_rb6d3mrb6d3mrb6d" src="https://github.com/user-attachments/assets/bad8351c-cb57-415a-8bdb-c5a27dde406b" />


## 📊 Fonte de Dados
PassengerId

Survived

Pclass

Sex

Age

SibSp

Parch

Fare	

Embarked_C

Embarked_Q

Embarked_S

Cabin_known

## ⚙️ Tecnologias Utilizadas

*Identificadas no projeto:*

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

XGBoost

Jupyter Notebook

*Os modelos utilizados foram:*
------------------------
XGBoost

SVM


### 𓂃🖊 Balanceamento de Classes: Se o seu modelo lida com problemas de classes desbalanceadas, explore técnicas como SMOTE, undersampling ou oversampling.

### 𓂃🖊 Padronização e Normalização: Lembre-se de padronizar os dados, especialmente se for usar modelos que são sensíveis à escala das variáveis.

- Apesar do XGBoost não ser sensivel à escala das variaveis, foi aplicado o StandardScaler dentro de um Pipeline para garantir a padronização e consistência no fluxo de treinamento.
------------------------------------------------------------------
### 𓂃🖊 Hiperparâmetros: Utilize GridSearchCV ou RandomSearchCV para encontrar os melhores parâmetros.

- min_child_weight: Soma mínima dos pesos das instâncias (hessiana) necessária em um filho. Se a etapa de particionamento da árvore resultar em um nó folha com a soma dos pesos das instâncias menor que min_child_weight, o processo de construção interromperá o particionamento.

- eval_metric: Evita warnings e deixa o treinamento mais explícito

- O ajuste de hiperparâmetros foi realizado usando o GridSearchCV junto de um Pipeline, garantindo que a padronização fosse corretamente aplicada dento de cada fold da validação cruzada.

- Para otimizar o modelo XGBoost, foi aplicado o GridSearchCV com validação cruzada de 5 folds, afim de encontrar a combinação mais adequada de hiperparâmetros. A métrica escolhida foi o recall.

- O melhor resultado encontrado foi um recall de aproximadamente 80%, demonstrando um bom equilíbrio.

## 👩‍💻 Sobre a Autora

Desenvolvido por Marina Napoleão — Cientista de Dados / Analista de Dados. 
### LinkedIn <https://www.linkedin.com/in/marina-napoleao/>
### GitHub <https://github.com/marinanapoleao>
