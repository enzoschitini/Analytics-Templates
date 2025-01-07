# Analytics-Templates

## Tipos de estruturas

---

Existem diferentes tipos de estruturas que podem ser aplicadas às colunas de uma tabela, dependendo do tipo de dado que a coluna armazena. Esses tipos são fundamentais para o tratamento e análise de dados. Aqui estão alguns dos principais tipos de estruturas para colunas de uma tabela:

### 1. **Estruturas Categóricas (Qualitativas)**

Essas colunas representam categorias ou grupos discretos, sem uma ordem específica ou com uma ordem implícita.

- **Categóricas Nominais**: Não há ordem ou hierarquia entre os valores.
    - Exemplos: `Marital_Status`, `Education`, `Country`, `Color`.
- **Categóricas Ordinais**: Existe uma ordem ou hierarquia entre os valores, mas as diferenças entre eles podem não ser bem definidas.
    - Exemplos: `Satisfaction Level` (Muito insatisfeito, Insatisfeito, Neutro, Satisfeito, Muito satisfeito).

### 2. **Estruturas Numéricas (Quantitativas)**

Colunas que contêm valores numéricos que podem ser manipulados matematicamente. Podem ser contínuas ou discretas.

- **Numéricas Inteiras (Discretas)**: Representam contagens ou valores inteiros.
    - Exemplos: `Age`, `FamilySize`, `Number_of_Purchases`.
- **Numéricas Reais (Contínuas)**: Representam valores que podem assumir qualquer valor dentro de um intervalo.
    - Exemplos: `Income`, `Price`, `Temperature`, `Height`.
- **Numéricas Binárias**: Colunas que contêm apenas dois valores possíveis, frequentemente representando sim/não, verdadeiro/falso, etc.
    - Exemplos: `IsMarried`, `HasChildren`.

### 3. **Estruturas de Texto**

Colunas que armazenam dados textuais ou alfanuméricos.

- **String**: Armazena uma sequência de caracteres. Pode ser usada para armazenar nomes, descrições, ou qualquer outro tipo de texto.
    - Exemplos: `Name`, `Address`, `Description`.
- **Texto Longo (ou Blob)**: Utilizado para armazenar grandes quantidades de texto ou dados não estruturados.
    - Exemplos: `Comment`, `Review`.

### 4. **Estruturas Temporais**

Colunas que armazenam informações sobre data e/ou hora.

- **Data**: Representa uma data (sem a parte de hora).
    - Exemplos: `BirthDate`, `StartDate`, `EndDate`.
- **Data e Hora**: Armazena tanto a data quanto o horário.
    - Exemplos: `Timestamp`, `LastLogin`.
- **Duração**: Representa um intervalo de tempo (diferença entre duas datas ou horas).
    - Exemplos: `TimeSpent`, `Duration`.

### 5. **Estruturas Geográficas**

Colunas que armazenam dados relacionados à geografia e localização.

- **Ponto Geográfico**: Coordenadas de latitude e longitude.
    - Exemplos: `Latitude`, `Longitude`.
- **Área Geográfica**: Pode ser um polígono ou uma área representando uma região geográfica.
    - Exemplos: `City`, `Region`, `Country`.
- **Caminho ou Polígono Geográfico**: Representa trajetórias ou áreas com múltiplos pontos.
    - Exemplos: `Route`, `RegionBounds`.

### 6. **Estruturas Lógicas**

Colunas que armazenam valores que representam uma condição booleana (verdadeiro/falso, sim/não).

- **Booleano (Lógico)**: Armazena valores de "verdadeiro" ou "falso", frequentemente representados por 1 e 0.
    - Exemplos: `HasChildren`, `IsActive`, `IsPremium`.

### 7. **Estruturas de Relacionamento (Referências)**

Colunas que fazem referência a outras tabelas ou entidades.

- **Chave Primária (Primary Key)**: Um identificador único para cada linha na tabela.
    - Exemplos: `ID`, `UserID`.
- **Chave Estrangeira (Foreign Key)**: Uma coluna que cria uma relação com uma chave primária de outra tabela.
    - Exemplos: `CustomerID` (referência a uma tabela de clientes).

### 8. **Estruturas Compostas**

Colunas que armazenam múltiplos valores ou elementos agrupados.

- **Listas ou Arrays**: Armazena uma sequência de elementos do mesmo tipo.
    - Exemplos: `Tags`, `ProductIDs`.
- **Dicionários ou Mapas**: Armazenam pares chave-valor.
    - Exemplos: `Settings`, `Attributes`.

### 9. **Estruturas de Identificação e Classificação**

Colunas que armazenam identificadores únicos ou classificações associadas a uma entidade.

- **Identificadores de Categoria**: Usado para indexar ou categorizar entidades.
    - Exemplos: `ProductCategory`, `EmployeeLevel`.

Essas estruturas ajudam a entender como organizar e tratar dados dentro de uma tabela, garantindo que os tipos de dados sejam manipulados corretamente em análises e processos de modelagem.

## Combinação dessas estruturas de dados

---

Com a combinação dessas estruturas de dados, é possível criar diversos tipos de gráficos que ajudam a visualizar e analisar diferentes aspectos dos dados. Abaixo, sugiro algumas ideias de gráficos baseadas nas estruturas de dados que você mencionou.

### 1. **Estruturas Categóricas (Qualitativas)**

- **Gráfico de Barras (Bar Chart)**
    - **Quando usar**: Para comparar a frequência ou a contagem de categorias.
    - **Exemplo**: Visualizar a distribuição de `Education` (Ex: Graduation, PhD, etc.) ou `Marital_Status` (Ex: Married, Single, Together).
- **Gráfico de Pizza (Pie Chart)**
    - **Quando usar**: Para visualizar a proporção de categorias dentro de um conjunto de dados.
    - **Exemplo**: Visualizar a porcentagem de cada `Education` ou `Marital_Status`.
- **Gráfico de Colunas Empilhadas (Stacked Bar Chart)**
    - **Quando usar**: Para comparar várias categorias dentro de uma única variável.
    - **Exemplo**: Analisar a distribuição de `Income` para cada `Education` ou `Marital_Status`.

### 2. **Estruturas Numéricas (Quantitativas)**

- **Histograma (Histogram)**
    - **Quando usar**: Para visualizar a distribuição de uma variável numérica.
    - **Exemplo**: Distribuição de `Income`, `Age`, ou `Recency`.
- **Gráfico de Dispersão (Scatter Plot)**
    - **Quando usar**: Para observar a relação entre duas variáveis numéricas.
    - **Exemplo**: Analisar a relação entre `Age` e `Income`.
- **Boxplot**
    - **Quando usar**: Para visualizar a distribuição e identificar outliers em variáveis numéricas.
    - **Exemplo**: Visualizar a distribuição de `Income` por diferentes categorias de `Education`.
- **Gráfico de Linha (Line Chart)**
    - **Quando usar**: Para observar tendências ao longo do tempo.
    - **Exemplo**: Mostrar como a variável `Income` evolui ao longo do tempo com base na `Date` de cada registro.

### 3. **Estruturas Temporais**

- **Gráfico de Linha (Line Chart)**
    - **Quando usar**: Para mostrar a evolução de uma variável ao longo do tempo.
    - **Exemplo**: Evolução do `Income` ou `Recency` ao longo do tempo (usando a coluna `Date`).
- **Gráfico de Área (Area Chart)**
    - **Quando usar**: Para mostrar a quantidade acumulada de uma variável ao longo do tempo.
    - **Exemplo**: Acumulação de `Complaints` ao longo de um período de tempo.

### 4. **Estruturas Geográficas**

- **Mapa de Calor (Heatmap)**
    - **Quando usar**: Para visualizar a densidade de pontos geográficos em uma área.
    - **Exemplo**: Mostrar a densidade de clientes em diferentes regiões (usando `Latitude` e `Longitude`).
- **Gráfico de Dispersão Geográfico (Geospatial Scatter Plot)**
    - **Quando usar**: Para mostrar a localização de pontos no espaço geográfico.
    - **Exemplo**: Plotar clientes em um mapa usando `Latitude` e `Longitude`.

### 5. **Estruturas Lógicas**

- **Gráfico de Barras ou Colunas para Valores Booleanos**
    - **Quando usar**: Para comparar a frequência de valores binários.
    - **Exemplo**: Visualizar a proporção de clientes que são `IsMarried` (casado ou não) ou `HasChildren` (tem filhos ou não).

### 6. **Estruturas de Identificação e Classificação**

- **Gráfico de Dispersão com Cores (Colored Scatter Plot)**
    - **Quando usar**: Para visualizar a relação entre variáveis numéricas, com a possibilidade de usar uma variável categórica para colorir os pontos.
    - **Exemplo**: Relacionar `Income` e `Age`, com a cor representando o `Education`.
- **Gráfico de Caixa por Categoria (Boxplot by Category)**
    - **Quando usar**: Para mostrar a distribuição de uma variável numérica por categorias.
    - **Exemplo**: Exibir a distribuição de `Income` para cada `Education` ou `Marital_Status`.

### 7. **Combinação de Variáveis Categóricas e Numéricas**

- **Gráfico de Dispersão 3D**
    - **Quando usar**: Para observar a relação entre três variáveis numéricas.
    - **Exemplo**: Analisar `Income`, `Age` e `Recency` em um gráfico 3D.
- **Gráfico de Barras Agrupadas (Grouped Bar Chart)**
    - **Quando usar**: Para comparar múltiplas variáveis categóricas e numéricas ao mesmo tempo.
    - **Exemplo**: Comparar `Income` entre diferentes categorias de `Education` e `Marital_Status`.
- **Matriz de Correlação (Correlation Matrix)**
    - **Quando usar**: Para mostrar a correlação entre várias variáveis numéricas.
    - **Exemplo**: Mostrar como `Income`, `Age` e `Recency` estão relacionados.

### 8. **Estruturas Compostas**

- **Gráfico de Radar (Radar Chart)**
    - **Quando usar**: Para mostrar múltiplas variáveis em um gráfico radial.
    - **Exemplo**: Comparar diferentes atributos de um cliente, como `Age`, `Income`, `Complaints`, `FamilySize` em um gráfico de radar.

Esses gráficos podem ser usados de maneiras criativas, dependendo da combinação dos tipos de dados presentes na tabela. Cada tipo de gráfico oferece uma maneira única de entender e analisar padrões, relações e distribuições nos dados.

## Templates

---

Entendido! Aqui estão algumas ideias de gráficos que combinam diferentes tipos de estruturas de dados para explorar as relações entre as variáveis categóricas (estrutura 1) e numéricas (estrutura 2), além de outras combinações criativas:

### 1. **Combinação de Variáveis Categóricas e Numéricas (Estruturas 1 e 2)**

### 1.1 **Gráfico de Barras com Valores Numéricos Agregados**

- **Quando usar**: Para comparar valores numéricos agregados (como médias, somas, contagens) para diferentes categorias.
- **Exemplo**: Comparar a média de `Income` para cada `Education` (variável categórica).
    - **Tipo de gráfico**: Gráfico de barras, onde cada barra representa uma categoria de `Education` e a altura da barra representa a média de `Income`.

### 1.2 **Boxplot por Categoria**

- **Quando usar**: Para visualizar a distribuição de uma variável numérica em diferentes categorias, identificando a mediana, quartis e outliers.
- **Exemplo**: Exibir a distribuição de `Income` para cada `Education` ou `Marital_Status`.
    - **Tipo de gráfico**: Boxplot, onde cada caixa representa uma categoria (como `Education`) e a variável numérica (`Income`) é visualizada dentro de cada caixa.

### 1.3 **Gráfico de Dispersão com Cores para Categorias**

- **Quando usar**: Para mostrar a relação entre duas variáveis numéricas, com uma variável categórica sendo usada para colorir os pontos.
- **Exemplo**: Analisar a relação entre `Age` e `Income`, com a cor representando o `Marital_Status`.
    - **Tipo de gráfico**: Gráfico de dispersão, onde os pontos são coloridos de acordo com a categoria de `Marital_Status`.

### 1.4 **Gráfico de Barras Empilhadas**

- **Quando usar**: Para comparar múltiplas variáveis categóricas e numéricas ao mesmo tempo, exibindo a distribuição de categorias dentro de uma variável numérica.
- **Exemplo**: Comparar a distribuição de `FamilySize` (numérico) por `Education` (categórica).
    - **Tipo de gráfico**: Barras empilhadas, onde a altura das barras representa a soma de `FamilySize` dentro de cada categoria de `Education`.

### 2. **Combinação de Variáveis Temporais e Numéricas (Estruturas 3 e 2)**

### 2.1 **Gráfico de Linha por Categoria**

- **Quando usar**: Para mostrar a evolução de uma variável numérica ao longo do tempo, segmentada por uma variável categórica.
- **Exemplo**: Analisar a evolução do `Income` ao longo do tempo (`Date`), com uma linha para cada `Education`.
    - **Tipo de gráfico**: Gráfico de linha, onde as diferentes linhas representam diferentes valores de `Education` e a evolução de `Income` ao longo do tempo.

### 2.2 **Gráfico de Área Empilhada**

- **Quando usar**: Para mostrar a evolução acumulada de uma variável numérica ao longo do tempo, segmentada por uma variável categórica.
- **Exemplo**: Exibir a soma de `Complaints` ao longo do tempo (`Date`), com cada cor representando uma categoria de `Education`.
    - **Tipo de gráfico**: Gráfico de área empilhada, onde as áreas são empilhadas para representar diferentes categorias de `Education`.

### 3. **Combinação de Variáveis Geográficas e Numéricas (Estruturas 4 e 2)**

### 3.1 **Mapa de Calor (Heatmap) com Dados Numéricos**

- **Quando usar**: Para visualizar a distribuição de valores numéricos em diferentes regiões geográficas.
- **Exemplo**: Exibir a densidade de `Income` em diferentes regiões geográficas usando `Latitude` e `Longitude`.
    - **Tipo de gráfico**: Mapa de calor, onde as áreas geográficas são coloridas de acordo com a intensidade de `Income`.

### 3.2 **Gráfico de Dispersão Geográfico com Tamanho de Ponto**

- **Quando usar**: Para exibir a relação entre variáveis numéricas e localização geográfica.
- **Exemplo**: Mostrar `FamilySize` e `Income` em diferentes locais usando as coordenadas geográficas (`Latitude`, `Longitude`), com o tamanho do ponto representando o valor de `Income`.
    - **Tipo de gráfico**: Gráfico de dispersão geográfico, com os pontos representando localizações e o tamanho dos pontos variando com base no `Income`.

### 4. **Combinação de Variáveis Categóricas e Lógicas (Estruturas 1 e 5)**

### 4.1 **Gráfico de Barras por Categoria com Booleano**

- **Quando usar**: Para comparar a frequência de uma variável categórica, segmentada por uma variável booleana.
- **Exemplo**: Comparar o número de pessoas `IsMarried` para diferentes categorias de `Education`.
    - **Tipo de gráfico**: Gráfico de barras agrupadas, onde as barras representam categorias de `Education` e cada grupo de barras mostra a contagem de `IsMarried` (sim ou não).

### 4.2 **Gráfico de Colunas Empilhadas com Valores Booleanos**

- **Quando usar**: Para mostrar a distribuição de variáveis booleanas dentro de uma variável categórica.
- **Exemplo**: Mostrar a proporção de pessoas com `HasChildren` (verdadeiro/falso) dentro de cada categoria de `Marital_Status`.
    - **Tipo de gráfico**: Gráfico de colunas empilhadas, onde cada coluna é dividida entre os valores de `HasChildren` (0 ou 1), representando a distribuição de filhos dentro de cada estado civil.

### 5. **Combinação de Variáveis Temporais e Categóricas (Estruturas 3 e 1)**

### 5.1 **Gráfico de Linha com Categorias**

- **Quando usar**: Para observar a tendência temporal de uma variável categórica, dividindo o gráfico por diferentes categorias.
- **Exemplo**: Analisar como `Marital_Status` muda ao longo do tempo (`Date`).
    - **Tipo de gráfico**: Gráfico de linha, onde a linha representa o tempo e cada categoria de `Marital_Status` tem uma linha distinta.

### 5.2 **Gráfico de Barras Empilhadas ao Longo do Tempo**

- **Quando usar**: Para comparar a distribuição de categorias ao longo do tempo.
- **Exemplo**: Visualizar a distribuição de `Education` ao longo do tempo (`Date`).
    - **Tipo de gráfico**: Gráfico de barras empilhadas, onde o eixo X é o tempo (representado pela variável `Date`) e o eixo Y é a contagem de cada categoria de `Education` ao longo do tempo.

### 6. **Combinação de Variáveis Categóricas e Identificação (Estruturas 1 e 6)**

### 6.1 **Gráfico de Barras com Categorias de Identificação**

- **Quando usar**: Para comparar variáveis de identificação com uma variável categórica.
- **Exemplo**: Comparar `Income` por diferentes categorias de `Education` e `IsMarried`.
    - **Tipo de gráfico**: Gráfico de barras, onde cada barra representa uma categoria de `Education`, com cores ou marcas representando o estado de `IsMarried`.

Essas combinações de gráficos podem fornecer insights valiosos ao analisar como diferentes tipos de dados interagem uns com os outros. Usando essas combinações, você pode explorar de maneira mais profunda as relações entre variáveis categóricas, numéricas, temporais, lógicas e até geográficas.

---

### 7. **Combinação de Variáveis Numéricas e Lógicas (Estruturas 2 e 5)**

### 7.1 **Histograma com Distorção por Booleano**

- **Quando usar**: Para visualizar a distribuição de uma variável numérica, dividida por uma variável booleana.
- **Exemplo**: Exibir a distribuição de `Income` para as categorias `IsMarried` (verdadeiro ou falso).
    - **Tipo de gráfico**: Histograma com duas barras para cada faixa de `Income`, uma para valores de `IsMarried = True` e outra para `IsMarried = False`.

### 7.2 **Gráfico de Barras Agrupadas com Booleano**

- **Quando usar**: Para comparar a distribuição de uma variável numérica para categorias booleanas.
- **Exemplo**: Comparar a média de `Age` entre pessoas casadas (`IsMarried = 1`) e não casadas (`IsMarried = 0`).
    - **Tipo de gráfico**: Barras agrupadas, onde cada grupo de barras representa uma categoria de `IsMarried` (0 ou 1), e a altura das barras mostra a média de `Age`.

### 7.3 **Boxplot com Valores Booleanos**

- **Quando usar**: Para observar a distribuição de uma variável numérica, segmentada por uma variável booleana.
- **Exemplo**: Exibir a distribuição de `Recency` para clientes com e sem reclamações (`Complain`).
    - **Tipo de gráfico**: Boxplot dividido por valores de `Complain` (0 ou 1).

### 8. **Combinação de Variáveis Temporais, Numéricas e Categóricas (Estruturas 3, 2 e 1)**

### 8.1 **Gráfico de Linhas Empilhadas ao Longo do Tempo**

- **Quando usar**: Para observar a evolução de múltiplas categorias ao longo do tempo.
- **Exemplo**: Mostrar a evolução de `Income` ao longo do tempo (`Date`), segmentada por `Education` ou `Marital_Status`.
    - **Tipo de gráfico**: Gráfico de linha empilhada, onde a linha representa o tempo e as diferentes cores representam categorias como `Education`.

### 8.2 **Heatmap Temporal com Variáveis Categóricas**

- **Quando usar**: Para observar a intensidade de uma variável numérica ao longo do tempo, dividida por categorias.
- **Exemplo**: Analisar a intensidade de `Income` ao longo do tempo (`Date`), segmentada por `Education`.
    - **Tipo de gráfico**: Heatmap, onde o eixo X representa o tempo (`Date`), o eixo Y as categorias de `Education` e a intensidade de cor representa a média ou soma de `Income`.

### 8.3 **Gráfico de Linhas com Múltiplas Categorias**

- **Quando usar**: Para comparar a evolução de uma variável numérica ao longo do tempo para diferentes categorias.
- **Exemplo**: Analisar a evolução de `Recency` ao longo do tempo (`Date`), com uma linha para cada categoria de `Marital_Status`.
    - **Tipo de gráfico**: Gráfico de linha, onde diferentes linhas representam categorias de `Marital_Status`.

### 9. **Combinação de Variáveis Geográficas e Lógicas (Estruturas 4 e 5)**

### 9.1 **Mapa de Calor com Variáveis Booleanas**

- **Quando usar**: Para observar a intensidade de uma variável booleana em diferentes regiões geográficas.
- **Exemplo**: Visualizar a distribuição de `IsMarried` nas diferentes regiões geográficas, usando `Latitude` e `Longitude` para mapear as localizações.
    - **Tipo de gráfico**: Mapa de calor, onde a intensidade de cor reflete a concentração de casados (ou não) em uma determinada área.

### 9.2 **Gráfico de Dispersão Geográfico com Booleano**

- **Quando usar**: Para mostrar a relação entre variáveis geográficas e booleanas.
- **Exemplo**: Exibir a localização dos clientes que têm filhos (`HasChildren = 1`) e os que não têm filhos (`HasChildren = 0`).
    - **Tipo de gráfico**: Gráfico de dispersão geográfico, com pontos representando as localizações de clientes e a cor do ponto representando a variável `HasChildren`.

### 10. **Combinação de Variáveis de Identificação e Numéricas (Estruturas 6 e 2)**

### 10.1 **Gráfico de Barras com Identificadores e Variáveis Numéricas**

- **Quando usar**: Para comparar o valor de uma variável numérica em diferentes categorias de identificação.
- **Exemplo**: Comparar o `Income` médio entre diferentes grupos de identificação de cliente, como `CustomerID` ou `UserID`.
    - **Tipo de gráfico**: Gráfico de barras, onde cada barra representa um identificador (como `UserID`), e a altura das barras representa a média de `Income`.

### 10.2 **Gráfico de Dispersão com Identificadores**

- **Quando usar**: Para observar a relação entre duas variáveis numéricas, com um identificador único colorindo os pontos.
- **Exemplo**: Analisar a relação entre `Age` e `Income`, com o identificador `UserID` sendo utilizado para colorir os pontos de acordo com a categoria de `Education`.
    - **Tipo de gráfico**: Gráfico de dispersão, onde cada ponto tem uma cor baseada no identificador (como `UserID` ou `CustomerID`), que pode refletir uma variável como `Education`.

### 11. **Combinação de Variáveis Categóricas, Numéricas e Lógicas (Estruturas 1, 2 e 5)**

### 11.1 **Gráfico de Barras Empilhadas com Booleano e Categoria**

- **Quando usar**: Para comparar a distribuição de uma variável numérica para diferentes categorias, segmentada por uma variável booleana.
- **Exemplo**: Comparar a distribuição de `Income` para diferentes categorias de `Education` (como "Graduation", "PhD", etc.), segmentada pela variável `IsMarried` (casado ou não).
    - **Tipo de gráfico**: Gráfico de barras empilhadas, onde as barras representam `Education` e as empilhamentos mostram a divisão entre casados e não casados (`IsMarried`).

### 11.2 **Boxplot com Categórica e Lógica**

- **Quando usar**: Para observar a distribuição de uma variável numérica por categorias, dividida por uma variável booleana.
- **Exemplo**: Exibir a distribuição de `Recency` para cada categoria de `Education`, segmentado por `Complain` (com ou sem reclamações).
    - **Tipo de gráfico**: Boxplot, onde cada caixa representa uma categoria de `Education`, e a segmentação é feita por `Complain` (0 ou 1).

### 11.3 **Gráfico de Dispersão com Categórica, Numérica e Lógica**

- **Quando usar**: Para exibir a relação entre variáveis numéricas e categóricas, com uma segmentação booleana representando uma terceira variável.
- **Exemplo**: Analisar a relação entre `Age` e `Income`, com diferentes categorias de `Education` representadas por diferentes cores, e `IsMarried` sendo refletido no tamanho dos pontos.
    - **Tipo de gráfico**: Gráfico de dispersão, onde as cores indicam a categoria de `Education` e o tamanho dos pontos indica se a pessoa é casada (`IsMarried`).

Essas são algumas ideias adicionais de gráficos para combinar diferentes estruturas de dados. Com essas combinações, você consegue explorar as interações entre variáveis de maneiras mais detalhadas e visuais, o que pode revelar padrões e insights valiosos em seus dados.

## Proporções, médias, taxas e KPIs

---

Aqui estão combinações de estruturas que podem revelar métricas ocultas e comportamentos complexos, explorando relações implícitas entre variáveis:

---

### **1. Comportamento de Proporções em Diferentes Categorias (Estruturas 1, 2 e 5)**

### **1.1 Gráfico de Área Normalizada**

- **Quando usar**: Para mostrar como uma proporção ou taxa se comporta dentro de categorias ao longo de uma variável numérica ou booleana.
- **Exemplo**: Exibir a proporção de `IsMarried` (lógico) para diferentes categorias de `Education`, considerando faixas de `Income`.
    - **Tipo de gráfico**: Gráfico de área normalizada, onde cada camada representa uma categoria de `Education`, e as proporções refletem a variável booleana `IsMarried` dentro das faixas de `Income`.

### **1.2 Gráfico de Taxa por Categoria**

- **Quando usar**: Para calcular e exibir uma taxa (como a média de reclamações por grupo).
- **Exemplo**: Mostrar a taxa de `Complain` (reclamações) para cada categoria de `Marital_Status`, ponderada por `FamilySize`.
    - **Tipo de gráfico**: Barras agrupadas ou linha para cada categoria de `Marital_Status`, com a altura ou posição mostrando a taxa calculada.

---

### **2. Comportamento de Variação Temporal por Categorias (Estruturas 3, 1 e 2)**

### **2.1 Gráfico de Gradiente de Evolução**

- **Quando usar**: Para mostrar a variação de uma variável numérica ao longo do tempo, separada por categorias.
- **Exemplo**: Visualizar a variação média de `Age` ao longo do tempo (`Date`), para diferentes categorias de `Education`.
    - **Tipo de gráfico**: Heatmap temporal, onde o eixo X é o tempo, o eixo Y as categorias de `Education`, e a intensidade da cor reflete a média de `Age`.

### **2.2 Gráfico de Linhas com Derivadas**

- **Quando usar**: Para mostrar a taxa de variação de uma variável numérica em relação ao tempo e categorias.
- **Exemplo**: Mostrar a taxa de crescimento ou redução de `Income` ao longo do tempo (`Date`), separada por `Marital_Status`.
    - **Tipo de gráfico**: Gráfico de linhas, com inclinações indicando a taxa de variação, segmentadas por `Marital_Status`.

---

### **3. Variação Geográfica de Taxas ou Comportamentos (Estruturas 4, 2 e 5)**

### **3.1 Mapa de Variação de Taxa**

- **Quando usar**: Para exibir a taxa de ocorrência de um evento ou a média de uma variável numérica em diferentes localizações.
- **Exemplo**: Mostrar a média de `Income` em regiões geográficas, ponderada pelo número de pessoas com `Complain = 1`.
    - **Tipo de gráfico**: Mapa de calor geográfico, com intensidade refletindo a taxa de média ponderada.

### **3.2 Mapa de Dispersão com Tamanho e Cor**

- **Quando usar**: Para mostrar múltiplas métricas em um mesmo gráfico.
- **Exemplo**: Exibir a densidade de `FamilySize` por região geográfica, com o tamanho dos pontos representando a média de `Recency` e a cor representando a proporção de `IsMarried`.
    - **Tipo de gráfico**: Gráfico de dispersão geográfico.

---

### **4. Relações entre Variáveis Categóricas, Numéricas e Temporais (Estruturas 1, 2 e 3)**

### **4.1 Gráfico de Taxa Condicional**

- **Quando usar**: Para observar como uma taxa muda dependendo de várias condições.
- **Exemplo**: Mostrar a variação da proporção de `FamilySize` em relação a `Marital_Status` ao longo do tempo (`Date`).
    - **Tipo de gráfico**: Gráfico de linhas ou barras empilhadas ao longo do tempo.

### **4.2 Boxplot com Divisão Temporal**

- **Quando usar**: Para observar mudanças na dispersão de uma variável numérica para diferentes categorias ao longo do tempo.
- **Exemplo**: Exibir a distribuição de `Income` por `Education` para diferentes períodos (`Date` agrupado por ano).
    - **Tipo de gráfico**: Boxplot separado por períodos de tempo.

---

### **5. Correlação Complexa entre Variáveis Geográficas, Numéricas e Categóricas (Estruturas 4, 2 e 1)**

### **5.1 Heatmap Geográfico de Proporções**

- **Quando usar**: Para analisar como proporções de categorias variam geograficamente.
- **Exemplo**: Exibir a proporção de pessoas com `Complain = 1` para diferentes regiões geográficas.
    - **Tipo de gráfico**: Heatmap geográfico.

### **5.2 Gráfico de Bolhas Geográficas**

- **Quando usar**: Para visualizar múltiplas métricas numéricas e categóricas em um contexto geográfico.
- **Exemplo**: Exibir a média de `Income` por região, com o tamanho das bolhas representando a soma de `FamilySize` e as cores representando a categoria predominante de `Marital_Status`.
    - **Tipo de gráfico**: Mapa de bolhas.

---

### **6. Combinação de Variáveis Lógicas, Temporais e Numéricas (Estruturas 5, 3 e 2)**

### **6.1 Gráfico de Percentuais Acumulados**

- **Quando usar**: Para mostrar como uma métrica booleana se comporta em relação ao tempo e a outras variáveis numéricas.
- **Exemplo**: Mostrar o percentual acumulado de reclamações (`Complain = 1`) ao longo do tempo (`Date`), ponderado pelo tamanho da família (`FamilySize`).
    - **Tipo de gráfico**: Gráfico de área empilhada.

### **6.2 Gráfico de Taxa Temporal**

- **Quando usar**: Para exibir uma taxa (como a proporção de `IsMarried`) ao longo do tempo, ponderada por uma variável numérica.
- **Exemplo**: Mostrar a proporção de pessoas casadas (`IsMarried = 1`) ao longo do tempo, ponderada por `Income`.
    - **Tipo de gráfico**: Gráfico de linha com pontos representando médias ponderadas.

---

Esses gráficos exploram relações mais profundas e podem revelar métricas ocultas que não são óbvias à primeira vista. Cada ideia visa combinar diferentes dimensões de dados para criar visualizações que gerem insights mais ricos e contextuais.