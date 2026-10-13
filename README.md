# Manutenção Eficiente

## 1. Sobre o projeto

O **Manutenção Eficiente** é um projeto de Inteligência Artificial para análise preditiva de falhas em máquinas industriais. O objetivo é explorar dados operacionais e desenvolver modelos de classificação capazes de identificar padrões associados à ocorrência de falhas.

O projeto foi desenvolvido como atividade avaliativa do módulo **Desenvolvimento de IA para Análise Preditiva**, com Python e bibliotecas de análise de dados e Machine Learning.

## 2. Objetivos

- Explorar e compreender os dados industriais.
- Tratar dados ausentes e verificar registros duplicados.
- Criar novas variáveis para representar características relevantes do processo.
- Preparar os dados para treinamento e teste.
- Comparar modelos de classificação e avaliar seus resultados.

## 3. Tecnologias utilizadas

- Python
- Pandas e NumPy
- Matplotlib e Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Google Colab
- Git e GitHub

As versões das principais bibliotecas estão registradas no arquivo `requirements.txt`.

## 4. Etapas do desenvolvimento

O notebook está organizado em sete fases:

1. **Análise exploratória:** inspeção da estrutura, dos tipos de dados, das estatísticas descritivas e das distribuições.
2. **Tratamento dos dados:** análise de valores ausentes e registros duplicados.
3. **Engenharia de atributos:** criação de variáveis derivadas, incluindo diferença de temperatura e estimativa de potência mecânica.
4. **Preparação dos dados:** separação entre variáveis preditoras e variável-alvo, divisão estratificada entre treino e teste e balanceamento do treino com SMOTE.
5. **Padronização:** aplicação do StandardScaler aos dados utilizados pelo KNN.
6. **Treinamento e comparação:** avaliação de diferentes configurações do KNN e da árvore de decisão.
7. **Avaliação final:** comparação dos modelos selecionados e justificativa da escolha final.

## 5. Resultado

Na avaliação final, a árvore de decisão com `max_depth=10` obteve acurácia de **93,75% no conjunto de teste**, enquanto o KNN com `n_neighbors=3` obteve **91,50%**.

A árvore de decisão foi selecionada por apresentar maior acurácia no teste e menor diferença entre os resultados de treino e teste entre as duas configurações finais avaliadas.

A acurácia, isoladamente, não é suficiente para avaliar um sistema de manutenção preditiva. Como trabalhos futuros, recomenda-se analisar a precisão, o recall, a matriz de confusão e os falsos negativos, considerando o impacto de falhas não identificadas.

## 6. Como executar

1. Abra o notebook `Manutencao_Eficiente_Final.ipynb` no GitHub.
2. Para executar o projeto, abra o arquivo no Google Colab ou em um ambiente Jupyter com Python instalado.
3. Disponibilize o conjunto de dados utilizado pelo notebook conforme o caminho definido no código.
4. Instale as dependências listadas em `requirements.txt`.
5. Execute as células em ordem, da primeira à última fase.

## 7. Estrutura do repositório

- `Manutencao_Eficiente_Final.ipynb` — notebook com as sete fases do projeto.
- `requirements.txt` — versões das principais bibliotecas utilizadas.
- `README.md` — documentação do projeto.

---

**Projeto acadêmico — Desenvolvimento de IA para Análise Preditiva.**
