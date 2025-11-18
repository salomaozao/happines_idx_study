> [fonte (Dataset)](https://www.kaggle.com/code/javadzabihi/happiness-2017-visualization-prediction)
> [Aplicação](https://www.kaggle.com/code/javadzabihi/happiness-2017-visualization-prediction)

# 1. Introdução
This dataset gives the happiness rank and happiness score of 155 countries around the world based on seven factors including family, life expectancy, economy, generosity, trust in government, freedom, and dystopia residual. Sum of the value of these seven factors gives us the happiness score and the higher the happiness score, the lower the happiness rank 

The following columns: GDP per Capita, Family, Life Expectancy, Freedom, Generosity, Trust Government Corruption describe the extent to which these factors contribute in evaluating the happiness in each country.
The Dystopia Residual metric actually is the Dystopia Happiness Score(1.85) + the Residual value or the unexplained value for each country as stated in the previous answer.

If you add all these factors up, you get the happiness score so it might be un-reliable to model them to predict Happiness Scores.

! Overall rank é a posição, e Score é a pontuação (y)

# 2. Objetivo
The purpose of choosing this work is to find out which factors are more important to live a happier life. As a result, people and countries can focus on the more significant factors to achieve a higher happiness level. We also will implement several machine learning algorithms to predict the happiness score and compare the result to discover which algorithm works better for this specific dataset.

# 3. Metodologia

## 3.1. Variáveis:
[1] "Overall rank"                
[2] "Country or region"           
[3] "Score"                         Y     
[4] "GDP per capita"                X   
[5] "Social support"                X
[6] "Healthy life expectancy"       X
[7] "Freedom to make life choices"  X
[8] "Generosity"                    X
[9] "Perceptions of corruption"     X

## 3.2 Tratamento dos dados

- usar scale? Perde interpretabilidade?

## 3.3. Visualização

## 3.4 Modelagem

## 3.5. Interpretação da modelagem



========= lixo

```{r Modelagem}
#  Regressão simples
# lm(`Overall rank` ~ `GDP per capita`, data = happines_df)

#  Lasso
# Y = happines_df$`Score`
# X = happines_df[, c("GDP per capita", "Freedom to make life choices", "Overall rank")]

# cv = cv.glmnet(X, Y, nfolds = length(Y), alpha = 1)
# coef(cv, s = "lambda.min")
```


```{r}
#  Validação do modelo

# Validação por k-fold/n-fold (n usa tudo menos uma obs.)

# ctrl = caret::trainControl(method="cv", number = 10)
# caret::train(modelo, data = data, method = "lm", ctrl)
```
```{r}

```