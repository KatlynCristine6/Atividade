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








