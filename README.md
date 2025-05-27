# Estudo de Análise de Dados com Azure Databricks

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

Este repositório documenta um estudo prático sobre a plataforma **Azure Databricks**, explorando seus principais conceitos e aplicando-os em um cenário real de leitura e manipulação de dados com Python e a biblioteca Pandas.

##  O que é o Azure Databricks?

O **Azure Databricks** é uma plataforma de análise de dados unificada, otimizada para a nuvem do Microsoft Azure. Seu principal objetivo é acelerar a colaboração entre cientistas de dados, engenheiros de dados e analistas de negócios.

> Ele funciona como um serviço central que faz a **interligação entre diferentes serviços e a visualização de dados**, simplificando pipelines complexos.

A plataforma se baseia em três pilares integrados:
* **Integrated Data Services:** Serviços de dados que simplificam a ingestão, preparação e processamento.
* **Integrated Management:** Gerenciamento unificado de infraestrutura, segurança e usuários.
* **End-to-end Analytic and ML:** Ciclo de vida completo para projetos de análise e Machine Learning, desde a exploração até a produção.

Dentro dele, encontramos recursos essenciais que potencializam o trabalho com dados:
* **Armazenamento:** Conexão nativa com Azure Data Lake Storage, Blob Storage, etc.
*  **Inteligência Artificial:** Ferramentas para construir e treinar modelos de Machine Learning.
*  **Governança:** Controle de acesso e gerenciamento de dados com o Unity Catalog.
*  **ETL (Extract, Transform, Load):** Capacidade de criar pipelines de dados robustos e escaláveis.
* **Compartilhamento de Dados:** Facilidade para compartilhar dados, notebooks e insights com a equipe.

---

##  Implementação Prática neste Projeto

Demonstrando o uso da plataforma, realizei os seguintes passos:

1.  **Configuração do Ambiente:**
    * Criação de um **cluster** de computação para processar os dados.
    * Desenvolvimento do código dentro de um **Notebook** interativo no workspace do Databricks.

2.  **Desenvolvimento em Python:**
    * Utilizei a linguagem Python para escrever o script de análise.
    * O script foi projetado para ler um arquivo de dados no formato `.csv` armazenado no Databricks File System (DBFS).

3.  **Uso da Biblioteca Pandas:**
    * Importei a biblioteca `pandas`, padrão da indústria para manipulação de dados em Python.
    * Carreguei os dados do arquivo CSV para um **DataFrame**, a estrutura de dados central do pandas.
    * Utilizei a função `display()` do Databricks para exibir o DataFrame de forma rica e interativa na tela.

---

## 💻 Exemplo do Código

Abaixo está um trecho simplificado do código desenvolvido no notebook, ilustrando a leitura e exibição dos dados.

```python
# Importa a biblioteca pandas, essencial para a manipulação de dados
import pandas as pd

# Define o caminho do arquivo CSV dentro do Databricks File System (DBFS)
# O caminho pode variar dependendo de onde o arquivo foi carregado.
caminho_arquivo = "/FileStore/tables/meu_arquivo_de_dados.csv"

# Utiliza a função read_csv do pandas para ler o arquivo e carregá-lo em um DataFrame
# O DataFrame 'df' agora contém todos os dados do arquivo em uma estrutura de tabela
df = pd.read_csv(caminho_arquivo)

# A função display() é específica do Databricks e renderiza o DataFrame
# de forma interativa, com opções de ordenação, filtro e visualização.
display(df)
```

---

## Documentação e Trabalho em Equipe

Um dos focos deste projeto foi a **documentação clara e objetiva do código**. Adicionar comentários e explicações, como visto no exemplo acima, é uma prática fundamental que visa:

* **Facilitar a Manutenção:** Tornar o código compreensível para futuras alterações e melhorias.
* **Promover a Colaboração:** Permitir que outros membros da equipe (ou até mesmo eu, no futuro) entendam rapidamente a lógica e o propósito do script, acelerando o trabalho em equipe e a integração em projetos maiores.

---

## Tecnologias Utilizadas

* **Cloud:** Microsoft Azure
* **Plataforma:** Azure Databricks
* **Linguagem:** Python
* **Biblioteca:** Pandas
