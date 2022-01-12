
# Concrete Slump Test

O Slump Test é um teste realizado para medir a trabalhabilidade do concreto, e com isso moldá-lo da melhor forma desejada. <br>
Um concreto mais trabalhável tende a ser menos resistente, portanto essa característica depende da finalidade da utilização do concreto. <br>
Para essa análise foi colhido um dataset do repositório público da UCI, que pode ser acessado <a href="http://archive.ics.uci.edu/ml/datasets/concrete+slump+test">aqui</a><br>
O dataset consiste em 7 atributos de entrada e 3 de saída, e os atributos de entrada são compostos por kg/m³ de concreto:<br>
<b>Atributos de entrada:</b>
<ul>
<li>Cimento</li>
<li>Escória de Alto Forno</li>
<li>Cinzas Volantes</li>
<li>Água</li>
<li>Superplastificante</li>
<li>Agregado Graúdo (Pedra)</li>
<li>Agregado Miúdo (Areia)</li>
</ul>
<b>Atributos de Saída</b>
<ul>
<li>SLUMP (cm)</li>
<li>FLOW (cm)</li>
<li>Resistência a Compressão após 28 dias (Mpa)</li>
</ul>

## Metodologia
Primeiramente foi feito uma análise exploratória dos dados e visualização das distribuições de frequência e correlação entre as variáveis.<br>
Após constatar que um modelo de Regressão Linear não seria o adequado, foi feita a separação dos dados em categorias, a fim de utilizar algoritmos de aprendizado de máquina que fosse capaz de classificar corretamente a classe que o Slump Test pertence com base na dosagem dos componentes do concreto.<br>
Foram utilizados 4 tipos de algoritmos:
<ul>
<li>KNN</li>
<li>Logistic Regression</li>
<li>SVM</li>
<li>Decision Tree</li>
</ul>

## Conclusão
Todos os modelos demonstraram uma acurácia muito abaixo de um modelo de predição ideal, e isso provavelmente se dá pela grande independência entre as variáveis e também pela baixa amostragem dos dados. Talvez com um conjunto com mais dados seja possível obter um modelo mais preciso.<br>
Mais detalhes pode ser conferido no notebook.
