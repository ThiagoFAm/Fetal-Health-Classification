# Fetal-Health-Classification
![medicina-fetal-feto2](https://github.com/user-attachments/assets/931bcbe3-4423-407e-9a97-b8f4c4ce9eee)

# Problema: Previsão do Risco de Complicações no Feto Durante a Gestação com Base em Indicadores Fisiológicos

## Contexto

Durante a gestação, monitorar a saúde do feto é essencial para garantir o bem-estar tanto da mãe quanto da criança. Em muitos casos, complicações podem surgir, como falta de oxigenação (hipóxia fetal), distúrbios no batimento cardíaco ou distúrbios nas contrações uterinas. Essas complicações podem levar a situações de risco durante o parto, incluindo o uso de intervenções médicas urgentes, como cesarianas, ou até mesmo a necessidade de monitoramento intensivo após o nascimento.

O monitoramento contínuo da saúde fetal é realizado por meio de dados obtidos de **cardiotocografias**, que medem o batimento cardíaco do feto, contrações uterinas e outros indicadores fisiológicos, como movimentos fetais e desacelerações no ritmo cardíaco. Esses dados fornecem informações cruciais sobre o estado de saúde do feto e podem indicar sinais precoces de complicações.

## Problema a Ser Resolvido

Com base em dados de monitoramento da saúde fetal, como batimentos cardíacos, movimentos fetais, contrações uterinas e variações nas acelerações e desacelerações, é possível prever se o feto está em risco elevado, risco moderado ou se está saudável. O objetivo é construir um modelo preditivo capaz de classificar fetos com base nos sinais fisiológicos coletados durante a gestação.

## Objetivo do Estudo

Construir um modelo de aprendizado de máquina capaz de classificar o risco da saúde fetal em três categorias:

- **Saudável (target = 1)**: O feto está em boas condições de saúde, sem sinais de estresse fetal ou complicações iminentes.
- **Risco Moderado (target = 2)**: O feto apresenta sinais de risco, mas a situação não é crítica, necessitando apenas de monitoramento.
- **Risco Elevado (target = 3)**: O feto está em situação crítica, apresentando sinais claros de complicações que podem necessitar de intervenções imediatas.

## Desafios e Questões

### Desafios técnicos:
- Como lidar com a variabilidade nos dados, como valores extremos nas acelerações e desacelerações, ou variações nas contrações uterinas que podem ser interpretadas de maneiras diferentes dependendo da fase da gestação?

### Classificação de múltiplas classes:
- A classificação de fetos em três categorias de risco (saudável, moderado e elevado) envolve um problema de classificação multiclasse, o que pode ser mais desafiador do que uma classificação binária.

### Interpretação clínica:
- Como garantir que o modelo preditivo possa ser interpretado de forma que médicos e obstetras possam tomar decisões informadas? Qual a explicabilidade dos resultados do modelo para uso clínico?

### Desbalanceamento de classes:
- A distribuição de fetos saudáveis, moderadamente em risco e em risco elevado pode ser desbalanceada, o que poderia afetar a precisão do modelo para prever corretamente os casos de risco elevado.

## Tarefas

### 1. Pré-processamento dos Dados:
- Limpeza dos dados.
- Tratamento de valores ausentes.
- Normalização das variáveis (como os batimentos cardíacos e o número de contrações).
- Transformação das variáveis de categoria para um formato adequado para modelagem.

### 2. Análise Exploratória dos Dados (EDA):
- Visualização das distribuições das variáveis.
- Análise de correlações entre as variáveis e o alvo (target).
- Identificação de padrões relevantes nos dados.

### 3. Desenvolvimento de Modelos Preditivos:
  
-(a definir)

### 4. Avaliação e Implementação:
- Avaliar a explicabilidade do modelo preditivo usando técnicas de interpretação de modelo, como **SHAP** ou **LIME**, para garantir que os resultados sejam compreensíveis para profissionais médicos.
