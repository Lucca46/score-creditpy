# Estudo de Python - Manipulação de Dados

Este repositório reúne um estudo prático em Python com foco em leitura, análise e tratamento de dados tabulares.

## Objetivo

Consolidar fundamentos de Python aplicados a dados, trabalhando com arquivos `.csv` em um notebook organizado para estudo e evolução.

## Estrutura do Projeto

```text
.
├── inicial.ipynb
├── clientes.csv
├── novos_clientes.csv
└── README.md
```

## Arquivos

- `inicial.ipynb`: notebook principal com o desenvolvimento do estudo.
- `clientes.csv`: base de dados original.
- `novos_clientes.csv`: base complementar para testes/comparações.

## Como Executar

1. Clone este repositório:

```bash
git clone <url-do-repositorio>
cd <nome-do-repositorio>
```

2. (Opcional, recomendado) Crie e ative um ambiente virtual:

```bash
python -m venv .venv
# Windows (PowerShell)
.\.venv\Scripts\Activate.ps1
```

3. Instale as dependências usadas no notebook (caso necessário):

```bash
pip install pandas jupyter
```

4. Execute o notebook:

```bash
jupyter notebook
```

Abra o arquivo `inicial.ipynb` no navegador e rode as células em sequência.

## Conteúdo Prático Esperado

- Leitura de arquivos CSV
- Inspeção e limpeza de dados
- Transformações básicas
- Comparação/integração entre bases

## Boas Práticas Aplicadas

- Estrutura simples e objetiva para estudo
- Notebook sem conteúdo sensível
- Dados separados em arquivos `.csv` para facilitar manutenção

## Resultados e Conclusões

Durante o estudo, foi possível montar um fluxo completo de classificação de score de crédito:

- carregamento e inspeção da base `clientes.csv`
- preparação dos dados com codificação de variáveis categóricas
- divisão entre treino e teste com `train_test_split`
- treinamento de dois modelos (`RandomForestClassifier` e `KNeighborsClassifier`)
- comparação de desempenho com `accuracy_score`
- geração de previsões para novos registros em `novos_clientes.csv`

Conclusão prática do estudo:

- o pipeline de ponta a ponta foi validado com sucesso
- o modelo de árvore (Random Forest) foi definido como principal no notebook
- a base de novos clientes pode ser usada para simulações de previsão de score (`Good`, `Standard`, `Poor`)

## Licença

Uso educacional.

