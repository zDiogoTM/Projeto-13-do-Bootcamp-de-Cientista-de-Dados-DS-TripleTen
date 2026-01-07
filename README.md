# Projeto-13-do-Bootcamp-de-Cientista-de-Dados-DS-TripleTen
Projeto 13 do Bootcamp de Cientista de Dados (DS) TripleTen
# 🚖 Previsão de Demanda de Táxi - Série Temporal

## 🎯 Sobre o Projeto
Projeto de Machine Learning para prever a demanda de pedidos de táxi por hora nos aeroportos da empresa Taxi Corrida Maluca. O objetivo é otimizar a alocação de motoristas durante horários de pico através de previsões precisas da demanda futura.

## 🔍 Contexto do Negócio
Para atrair mais motoristas durante horários de alta demanda, a empresa precisa prever com antecedência a quantidade de pedidos de táxi para a próxima hora. Isso permite:
- Melhor planejamento operacional
- Otimização da distribuição de motoristas
- Redução do tempo de espera dos passageiros
- Aumento da satisfação de clientes e motoristas

## 📊 Desafio
**Meta:** Desenvolver um modelo com RMSE ≤ 48 no conjunto de teste.

## 📂 Dados
- Dados históricos de pedidos de táxi em aeroportos
- Série temporal com informações horárias
- Reamostragem para intervalos de uma hora

## 🛠️ Metodologia

### 1. Preparação dos Dados
- Reamostragem dos dados para intervalos horários
- Análise exploratória de padrões temporais
- Identificação de sazonalidades (horária, diária, semanal)
- Divisão: 90% treino / 10% teste

### 2. Análise Exploratória
- Visualização de tendências temporais
- Identificação de padrões de pico
- Análise de sazonalidade
- Detecção de outliers

### 3. Modelagem
Treinamento e comparação de múltiplos modelos:
- Testes com diferentes hiperparâmetros
- Validação cruzada temporal
- Seleção do melhor modelo baseado em RMSE

### 4. Modelo Final
**LightGBM** selecionado como melhor modelo

## 💻 Tecnologias Utilizadas
- **Python 3.x**
- **pandas** - manipulação de dados
- **numpy** - operações numéricas
- **scikit-learn** - modelagem base
- **LightGBM** - modelo de gradient boosting
- **matplotlib / seaborn** - visualização
- **statsmodels** - análise de séries temporais
- **Jupyter Notebook** - desenvolvimento

## 📈 Resultados

### Modelo Final: LightGBM
- **RMSE no conjunto de teste: 42.66** ✅
- **Meta do projeto: RMSE ≤ 48** ✅
- **Status: APROVADO**

### Capacidades do Modelo
✓ Captura eficiente de padrões horários
✓ Identificação de sazonalidade semanal
✓ Previsões dentro da margem de erro aceitável
⚠️ Dificuldade em prever picos muito abruptos (comportamento esperado em séries de alta variabilidade)

### Conclusão
O modelo LightGBM apresentou o melhor desempenho entre todos os modelos testados, alcançando RMSE de aproximadamente 42.66 — **dentro da meta estabelecida**. O modelo está **RECOMENDADO** para uso em produção na previsão de pedidos de táxi por hora.

## 🚀 Como Executar

### Pré-requisitos
```bash
pip install pandas numpy scikit-learn lightgbm matplotlib seaborn statsmodels jupyter
```

### Executando o projeto
1. Clone este repositório
2. Abra o Jupyter Notebook:
```bash
jupyter notebook
```
3. Execute o notebook principal

## 📁 Estrutura do Projeto
```
├── README.md
├── sprint_13_previsao_taxi.ipynb    # Notebook principal
└── dados/                            # Dados históricos
```

## 💡 Aplicações Práticas
Este projeto demonstra:
- Análise e modelagem de séries temporais
- Feature engineering para dados temporais
- Tratamento de sazonalidade
- Seleção e otimização de modelos
- Validação de modelos em dados temporais
- Aplicação prática em otimização operacional

## 🎓 Contexto Acadêmico
**Sprint 13 - Bootcamp de Ciência de Dados TripleTen (2024)**

---

**Desenvolvido por:** Diogo  
**GitHub:** [@zDiogoTM](https://github.com/zDiogoTM)
