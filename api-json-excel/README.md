# Consumo de API e Manipulação de Arquivos com Python

## Objetivo

Este projeto tem como objetivo demonstrar, de forma prática, como consumir dados de uma API pública, manipular arquivos JSON e exportar informações para uma planilha Excel utilizando Python.

O exemplo utiliza a API pública do IBGE, que disponibiliza informações sobre os estados brasileiros.

---

## Tecnologias utilizadas

* Python 3
* Requests
* Pandas
* OpenPyXL

---

## API utilizada

**IBGE – Estados Brasileiros**

https://servicodados.ibge.gov.br/api/v1/localidades/estados

---

## Etapas do projeto

Durante a aula, o processo será desenvolvido em um único notebook Jupyter, seguindo as seguintes etapas:

1. Consumir os dados da API utilizando a biblioteca `requests`;
2. Receber os dados no formato JSON;
3. Salvar os dados em um arquivo `estados.json`;
4. Ler o arquivo JSON utilizando `json.load()`;
5. Converter os dados para um DataFrame do Pandas;
6. Selecionar e tratar as colunas desejadas;
7. Exportar os dados para uma planilha Excel (`estados.xlsx`).

Além do notebook, o repositório contém um exemplo em Python que realiza todo o processo diretamente da API para o DataFrame e, em seguida, exporta para Excel, sem a necessidade de salvar o JSON localmente.

---

## Estrutura do projeto

```text
api-json-excel/
│
├── etl_api_json_excel.ipynb
├── api_para_excel.py
├── estados.json
├── estados.xlsx
└── README.md
```

---

## Instalação

Instale as bibliotecas necessárias:

```bash
pip install requests pandas openpyxl
```

---

## Resultado esperado

Ao executar o notebook, serão gerados os seguintes arquivos:

* **estados.json** → Dados retornados pela API no formato JSON.
* **estados.xlsx** → Planilha contendo as colunas:

  * UF
  * Estado
  * Região

---

## Aprendizados

Neste exemplo são apresentados os seguintes conceitos:

* Consumo de APIs REST;
* Requisições HTTP utilizando a biblioteca `requests`;
* Manipulação de arquivos JSON;
* Leitura e gravação de arquivos com `json.load()` e `json.dump()`;
* Conversão de JSON para DataFrame com Pandas;
* Seleção e tratamento de colunas;
* Exportação de dados para Excel.

---

**Curso:** Análise de Dados com Python
**Módulo:** Manipulação de Arquivos com Python
