# Explorando Banco de Dados Relacional, Não Relacional e Normalização🎯
---
## O que é um banco de dados relacional e um exemplo de uso!
![banco](https://www.infortrend.com.br/imagens/uploads/o-que-faz-um-servidor-de-banco-de-dados-post-o-que-sao-servidores-de-banco-de-dados.jpg)

O banco de dados **relacional** é o tipo de banco que trabalha com tabelas relacionais, isto é, **tabelas compostas por linhas e colunas**, lembrando muito uma estrutura do Excel, no qual eles tendem a funcionar de maneira semelhante a uma **biblioteca organizada** no qual os dados são separados em tabelas que contêm suas devidas informações, e cada uma delas opera como uma pratileira, enquanto as linhas e colunas são as etiquetas que ajudam a encontrar as informações rapidamente.
Os bancos de dados relacionais também são construídos para compreender a **Structured Query Language (SQL)**, uma linguagem de programação padronizada usada para armazenar, manipular e recuperar dados que estão classificados dentro do banco de dados. Dentro do SQL, há uma linguagem interna para criação de tabelas chamada **Linguagem de Definição de Dados (DDL)** e uma linguagem para manipulação de dados chamada **Linguagem de Manipulação de Dados (DML)**.

---
### Exemplo de uso:
**Um ótimo e claro exemplo que podemos perceber a utilidade de um banco de dados organizado no cotidiano são nas organizações de saúde, como hospitais, clínicas e seguradoras, que dependem de registros médicos eletrônicos (EMRs) para controlar seus paacientes e proteger seus dados de forma eficiente. Os sistemas EMR podem armazenar uma ampla gama de informações do paciente, como diagnósticos, medicamentos, resultados laboratoriais, imagens e planos de tratamento.**

- <img width="795" height="277" alt="image" src="https://github.com/user-attachments/assets/c59bc054-0ea3-4e0f-83e8-64bbb6b9d435" />
---

- <img width="748" height="340" alt="image" src="https://github.com/user-attachments/assets/3f5de6af-4447-4c70-b837-bd49991b8dfd" />
---

- <img width="775" height="302" alt="image" src="https://github.com/user-attachments/assets/77c4d572-04e3-4a6c-93b3-2fa514060184" />
---

- <img width="779" height="354" alt="image" src="https://github.com/user-attachments/assets/4aeeec4c-0017-445e-bf83-defdedb54be6" />
---
## O que é um banco de dados não relacionais e um exemplo de uso!
![nao relacionais](https://hermes.dio.me/articles/cover/4c343f88-1bbf-4d3f-ac5a-0627ecb7e5cc.png)

Bancos de dados não relacionais, também conhecidos como **NoSQL** (Not Only SQL), são sistemas de gerenciamento de banco de dados que **não utilizam o modelo tradicional de tabelas com linhas e colunas**, como ocorre nos bancos de dados relacionais (ex: MySQL, Oracle, SQL Server). Em vez disso, eles empregam diversos modelos de armazenamento, como **chave-valor, documentos, colunas largas e grafos**, para acomodar dados mais flexíveis e não estruturados. 

---
## Principais tipos de bancos de dados não relacionais:

**Chave-valor:**
Armazenam dados como pares chave-valor, ideais para dados simples e com acesso rápido.

**Documento:**
Armazenam dados em formato de documento (como JSON ou XML), permitindo consultas mais complexas.

**Coluna larga:**
Armazenam dados em colunas, otimizando consultas por colunas específicas.

**Grafo:**
Armazenam dados como nós e arestas, ideais para modelar relacionamentos complexos. 

---
## Onde são utilizados:

**Big Data:**
Ideal para armazenar e processar grandes volumes de dados com alta variabilidade. 

**Aplicações em tempo real:**
Oferecem desempenho rápido para aplicações que exigem baixa latência. 

**Redes sociais e conteúdo:**
Permitem armazenar e gerenciar dados semiestruturados e não estruturados, como posts, imagens e vídeos. 

**Aplicativos móveis e web:**
Oferecem escalabilidade e flexibilidade para atender às demandas de aplicações modernas. 

---
### Exemplo de uso:
![imagens](https://learn.microsoft.com/pt-br/azure/architecture/guide/technology-choices/images/graph.png)

**A imagem representa um exemplo de banco de dados de grafos, onde funcionários e departamentos são conectados por seus relacionamentos. Cada nó azul representa um funcionário (Employee), e cada nó bege representa um departamento (Department). As setas ("arestas") indicam os relacionamentos entre eles, como "works in" (trabalha em) e "reports to" (se reporta a).**

**Por exemplo, o funcionário Max trabalha no departamento de Sales e se reporta a Alok, que por sua vez trabalha no departamento de Marketing e se reporta a Sarah. Já Inessa trabalha no setor de Manufacturing e também se reporta a Sarah**.

---
## O que é a normalização do banco de dados e qual o seu obetivo!

A normalização de bancos de dados é um processo que consiste em organizar as tabelas e os atributos em um banco de dados relacional de forma a eliminar redundâncias e anomalias funcionais.

O objetivo é dividir as informações em estruturas lógicas coesas e independentes, evitando a repetição desnecessária de dados e garantindo a integridade dos mesmos.

---
## Como é feito:
A normalização é dividida em etapas chamadas formas normais (1FN, 2FN, 3FN...). Cada uma aplica regras para melhorar a estrutura do banco. Por exemplo:

**1ª Forma Normal (1FN)**: Elimina grupos de dados repetidos.

**2ª Forma Normal (2FN)**: Separa dados que não dependem totalmente da chave primária.

**3ª Forma Normal (3FN)**: Remove dependências entre colunas que não são chaves.

---
### Exemplo rápido
<img width="862" height="341" alt="image" src="https://github.com/user-attachments/assets/57a8a55b-7e6b-4de5-b715-e982fbad6886" />

---
## Exemplo de tabela não normalizada
<img width="754" height="155" alt="image" src="https://github.com/user-attachments/assets/eb95554a-2906-441f-a8cd-6fc90760a2e9" />

A imagem mostra um exemplo de tabela **não normalizada**, ou seja, uma estrutura de banco de dados onde as informações estão organizadas de forma redundante e sem separação adequada dos dados.

Como essa tabela foi feita:

Ela reúne informações de clientes, produtos e compras em uma única tabela.

**Cliente_Nome** e **Cliente_Endereço** estão juntos em cada linha, **mesmo que se repitam** (como no caso da "Ana Banana").

**Produto_ID** e **Produto_Nome** também se repetem a cada compra, em vez de estarem em uma tabela separada.

Os campos Quantidade e Preço_Total indicam a transação feita.

---
## Exemplo de tabela normalizada

## **1FN**
Em termos simples, ela garante que cada coluna em uma tabela tenha apenas valores atômicos (indivisíveis) e que cada linha seja única através de uma chave primária;

| Cliente_Nome | Avenida_Endereço    | Número | Produto_ID | Produto_Nome    | Quantidade | Preço_Total |
|--------------|---------------------|--------|------------|-----------------|------------|-------------|
| Ana Banana   | Rua do Sorriso      | 99     | 20         | Bola de Futebol | 3          | 45,00       |
| Ana Banana   | Rua do Sorriso      | 99     | 21         | Sorvete         | 5          | 25,00       |
| Pedro Picles | Av. das Laranjas    | 22     | 22         | Skate           | 1          | 120,00      |
| Pedro Picles | Av. das Laranjas    | 23     | 23         | Chapéu Maluco   | 2          | 60,00       |
| Clara Cacau  | Travessa das Flores | 20     | 20         | Bola de Futebol | 1          | 15,00       

---
## **2FN**
É um conceito em modelagem de bancos de dados que visa eliminar a redundância de dados, garantindo que cada atributo não chave em uma tabela dependa funcionalmente de toda a chave primária, e não apenas de parte dela.

## 1. Cliente
| Cliente_ID | Cliente_Nome | Avenida_Endereço    | Número |
|------------|--------------|---------------------|--------|
| 1          | Ana Banana   | Rua do Sorriso      | 99     |
| 2          | Pedro Picles | Av. das Laranjas    | 22     |
| 3          | Clara cacau  | Travessa das Flores | 20     |

## 2. Produto
| Produto_ID | Produto_Nome    |
|------------|-----------------|
| 20         | Bola de Futebol |
| 21         | Sorvete         |
| 22         | 	Skate          |
| 23         | Chapéu Maluco   |

## 3. Compras
| Compra_ID | Cliente_ID | Produto_ID | Quantidade | Preço_Total |
|-----------|------------|------------|------------|-------------|
| 1         | 1          | 20         | 3          | 45,00       |
| 2         | 1          | 21         | 5          | 25,00       |
| 3         | 2          | 22         | 1          | 120,00      |
| 4         | 2          | 23         | 2          | 60,00       |
| 5         | 3          | 20         | 1          | 15,00       |
|           |            |            |            |             |

---
## **3FN**
É um conceito fundamental na modelagem de bancos de dados, que visa eliminar dependências transitivas em tabelas.

## 1. Clientes
| Cliente_ID | Cliente_Nome  | Avenida_Endereço    | 	Número |
|------------|---------------|---------------------|---------|
| 1          | Ana Banana   | Rua do Sorriso      | 90      |
| 2          | Pedro Picles | 	Av. das Laranjas   | 22      |
| 3          | Clara Cacau   | Travessa das Flores | 20      |

## 2. Produtos
| Produto_ID | Produto_Nome    | Preço_Unitário |
|------------|-----------------|----------------|
| 20         | Bola de Futebol | 15,00          |
| 21         | Sorvete         | 5,00           |
| 22         | Skate           | 120,00         |
| 23         | Chapéu Maluco   | 30,00          |
|            |                 |                |

## 3. Compras
| Compra_ID | Cliente_ID | Produto_ID | Quantidade |
|-----------|------------|------------|------------|
| 1         | 1          | 20         | 3          |
| 2         | 1          | 21         | 5          |
| 3         | 2          | 22         | 1          |
| 4         | 2          | 23         | 2          |
| 5         | 3          | 20         | 1          |

---
````
```
[
  {
    "Cliente_Nome": "Ana banana",
    "Cliente_Endereço": "Rua do Sorriso, 99",
    "Produto_ID": "20",
    "Produto_Nome": "Bola de Futebol",
    "Quantidade": "3",
    "Preço_Total": "45,00"
  },
  {
    "Cliente_Nome": "Ana banana",
    "Cliente_Endereço": "Rua do Sorriso, 99",
    "Produto_ID": "21",
    "Produto_Nome": "Sorvete",
    "Quantidade": "5",
    "Preço_Total": "25,00"
  },
  {
    "Cliente_Nome": "Pedro Picles",
    "Cliente_Endereço": "Av. das Laranjas, 12",
    "Produto_ID": "22",
    "Produto_Nome": "Skate",
    "Quantidade": "1",
    "Preço_Total": "120,00"
  },
  {
    "Cliente_Nome": "Pedro Picles",
    "Cliente_Endereço": "Av. das Laranjas, 12",
    "Produto_ID": "23",
    "Produto_Nome": "Chapéu Maluco",
    "Quantidade": "2",
    "Preço_Total": "60,00"
  },
  {
    "Cliente_Nome": "Clara cacau",
    "Cliente_Endereço": "Travessa das Flores, 7",
    "Produto_ID": "20",
    "Produto_Nome": "Bola de Futebol",
    "Quantidade": "1",
    "Preço_Total": "15,00"
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  },
  {
    "Cliente_Nome": "",
    "Cliente_Endereço": "",
    "Produto_ID": "",
    "Produto_Nome": "",
    "Quantidade": "",
    "Preço_Total": ""
  }
]


```
````

