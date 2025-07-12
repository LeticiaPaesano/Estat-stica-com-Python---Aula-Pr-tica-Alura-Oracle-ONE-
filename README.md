# Estatística com Python: Frequências e Medidas
Este repositório contém a **aula prática** desenvolvida durante o curso **"Estatística com Python: Resumindo e Analisando Dados"**, oferecido pela **Alura** em parceria com a **Oracle**, no programa **Oracle Next Education (ONE)**. A orientação foi conduzida pela instrutora **Danielle Oliveira**.

## 🎯 Objetivo

Aplicar, por meio de um notebook em Python, os principais conceitos de estatística descritiva, explorando dados reais com a biblioteca `pandas`, visualizando com `matplotlib` e `seaborn`, e realizando análises fundamentais para a compreensão e resumo de dados em projetos de ciência de dados.

## ✅ Aprendizados Desenvolvidos

### 📊 Exploração Inicial de Dados
- Uso de métodos básicos do `pandas` como `head()`, `shape`, `info()`;
- Identificação de variáveis qualitativas e quantitativas;
- Diferença entre variáveis numéricas discretas e contínuas.

### 📈 Visualizações com Gráficos
- Gráficos de barras com `matplotlib.pyplot`;
- Visualizações com `seaborn`: histogramas, curvas de densidade, boxplots;
- Representações para validar hipóteses de distribuição e identificar outliers e assimetrias.

### 🔧 Transformações e Preparação
- Conversão de variáveis numéricas em categóricas com `pd.cut()` e `.map()`;
- Ordenação com `sort_values()` e filtragens com `.isin()` e condições booleanas;
- Formatação de valores numéricos com `f-strings`.

### 📋 Tabelas de Frequência e Contingência
- Construção de tabelas de frequência absoluta e relativa;
- Agrupamentos com `groupby()`, `size()` e `value_counts()`;
- Uso de `pd.crosstab()` para tabelas de contingência, com aplicação do parâmetro `normalize`.

### 📐 Medidas Estatísticas
- Tendência central: média, mediana e moda;
- Dispersão: desvio médio absoluto (MAD), variância e desvio padrão;
- Medidas separatrizes: quartis e percentis;
- Interpretação da simetria e assimetria das distribuições.

### 🧮 Análises Segmentadas e Subconjuntos
- Cálculo de médias por categorias com `groupby()` + funções de agregação;
- Comparação de distribuições entre grupos com boxplots;
- Aplicação da regra de Sturges para definição do número ideal de classes.

### 🔁 Reprodutibilidade
- Geração de amostras aleatórias com `numpy.random` e uso de `seed` para replicabilidade.

## 📚 Bibliotecas Utilizadas

- `pandas`
- `matplotlib.pyplot`
- `seaborn`
- `numpy`

## 📂 Arquivo Principal

- `Projeto_Estatística_com_Python_frequencias_e_medidas.ipynb` – Notebook completo com todo o conteúdo aplicado durante o curso.

## 🧠 Instrução

Curso ministrado por **Danielle Oliveira**  
📘 Plataforma: [Alura](https://www.alura.com.br)  
🤝 Parceria: **Oracle**  
🎓 Programa: **Oracle Next Education (ONE)**

## 📸 Visualizações

Abaixo estão exemplos de visualizações, tabelas e gráficos desenvolvidos durante o notebook, organizados por tema.


### 🔹 Vendas por Categoria de Produto

| Categoria                        | Contagem |
|----------------------------------|----------|
| Eletrônicos                      | 36.060   |
| Roupas, Calçados e Acessórios    | 27.917   |
| Casa e Mobílias                  | 26.015   |
| Beleza e Cuidados Pessoais       | 22.026   |
| Esporte e Lazer                  | 19.939   |
| Alimentos e Bebidas              | 18.022   |
| Papelaria e Escritório           | 13.936   |
| Livros                           | 13.790   |
| Ferramentas e Construção         | 12.063   |
| Brinquedos                       | 10.232   |

<img width="738" height="413" alt="image" src="https://github.com/user-attachments/assets/7293fa28-259c-4ee7-80e0-ee060eaa0c55" />

### 🔹 Distribuição de Frequências das Avaliações

| Avaliação | Quantidade | Porcentagem (%)|
|-----------|------------|----------------|
| Ótimo     | 66076      | 33.0           |
| Bom       | 40980      | 20.5           |
| Regular   | 32282      | 16.1           |
| Ruim      | 28239      | 14.1           |
| Péssimo   | 32423      | 16.2           |

<img width="868" height="548" alt="image" src="https://github.com/user-attachments/assets/53bcef15-ba06-4868-99a3-9caed444798d" />

### 🔹 Tabela de contingência (distribuição de frequência bivariada)

Esta tabela de contingência detalha a distribuição das avaliações dos clientes por cada região do Brasil, permitindo uma análise comparativa da satisfação em diferentes localidades.

| Avaliação / Região | Centro-Oeste | Nordeste | Norte | Sudeste | Sul  |
|--------------------|--------------|----------|-------|---------|------|
| Péssimo            | 5005         | 7880     | 2757  | 9838    | 6943 |
| Ruim               | 4473         | 6809     | 2545  | 8810    | 5602 |
| Regular            | 3587         | 5701     | 2811  | 11345   | 4572 |
| Bom                | 7378         | 11834    | 3058  | 11845   | 6865 |
| Ótimo              | 11124        | 17343    | 5490  | 20656   | 11463|

### 🔹 Avaliação de Clientes por Região (Porcentagens)

Esta tabela de contingência exibe a distribuição percentual das avaliações dos clientes por cada região do Brasil, facilitando a comparação direta da satisfação em diferentes localidades.

| Avaliação / Região | Centro-Oeste (%) | Nordeste (%) | Norte (%) | Sudeste (%) | Sul (%) |
|--------------------|------------------|--------------|-----------|-------------|---------|
| Péssimo            | 15.9             | 15.9         | 15.6      | 15.2        | 19.0    |
| Ruim               | 14.2             | 13.7         | 14.4      | 13.6        | 15.3    |
| Regular            | 11.4             | 11.5         | 21.6      | 20.8        | 15.7    |
| Bom                | 23.4             | 23.9         | 17.3      | 18.3        | 18.8    |
| Ótimo              | 35.2             | 35.0         | 31.1      | 32.0        | 31.3    |

### 🔹 Avaliações Positivas por Região (%)

Esta tabela destaca a porcentagem combinada de avaliações "Ótimo" e "Bom" para cada região, evidenciando as áreas com maior satisfação do cliente.

| Região       |   %  |
|--------------|------|
| Centro-Oeste | 58.6 |
| Nordeste     | 58.9 |                               
| Norte        | 48.4 |                               
| Sudeste      | 50.3 |                               
| Sul          | 50.1 |                               

### 🔹 Avaliações Negativas por Região (%)

Esta tabela apresenta a porcentagem combinada de avaliações "Ruim" e "Péssimo" por região, indicando as áreas com maior insatisfação do cliente.

| Região       |  %   |
|--------------|------|
| Centro-Oeste | 30.1 |
| Nordeste     | 29.6 |
| Norte        | 30.0 |
| Sudeste      | 28.8 |
| Sul          | 34.3 |

### 🔹 Distribuição de Clientes por Região e Sexo Biológico

Esta tabela cruza os dados de clientes, mostrando a distribuição (provavelmente em termos de contagem ou média de alguma métrica) entre as regiões e o sexo biológico.

| Sexo Biológico / Região | Centro-Oeste | Nordeste |  Norte  | Sudeste |   Sul   |
|-------------------------|--------------|----------|---------|---------|---------|
| Feminino                | 1887.12      | 1861.09  | 1828.61 | 2160.82 | 2176.44 |
| Masculino               | 2025.24      | 2005.31  | 1830.54 | 1881.08 | 1871.38 |

### 🔹 Tempo Médio de Entrega por Categoria de Produto

A média ($$\mu$$) do tempo de entrega foi calculada para cada categoria de produto, conforme a fórmula: 

# $$\mu = \frac 1n\sum_{i=1}^{n}X_i = \frac{X_1 + X_2 + ... + X_n}{n}$$


| Categoria do Produto           | Tempo Médio de Entrega (dias) |
|--------------------------------|-------------------------------|
| Casa e Mobílias                | 14.4                          |
| Ferramentas e Construção       | 13.6                          |
| Papelaria e Escritório         | 12.0                          |
| Esporte e Lazer                | 10.7                          |
| Brinquedos                     | 10.1                          |
| Livros                         | 9.5                           |
| Roupas, Calçados e Acessórios  | 9.2                           |
| Beleza e Cuidados Pessoais     | 8.9                           |
| Alimentos e Bebidas            | 7.7                           |
| Eletrônicos                    | 7.2                           |

<img width="882" height="525" alt="image" src="https://github.com/user-attachments/assets/75ac90cc-1648-4891-acec-fc0453c67535" />

### 🔹 Mediana na investigação dos dados

$$
Elemento_{Md} = \begin{cases}
\frac{n+1}{2} & \text{se } n \text{ for ímpar} \\
\frac{n}{2} & \text{se } n \text{ for par}
\end{cases}
$$

---

$$
M_d = \begin{cases}
X_{Elemento_{Md}} & \text{se } n \text{ for ímpar} \\
\frac{X_{Elemento_{Md}} + X_{Elemento_{Md}+1}}{2} & \text{se } n \text{ for par}
\end{cases}
$$



<img width="580" height="433" alt="image" src="https://github.com/user-attachments/assets/4e7772aa-c1ed-4c8c-9d17-7f01584a4c43" />

### 🔹 Identificando as quantidades de livros que são mais frequentes para a campanha

Esta tabela exibe a quantidade de livros mais frequentemente comprada pelos clientes

| Região       | Contagem |
|--------------|----------|
| Sudeste      | 64603    |
| Nordeste     | 49567    |
| Sul          | 36602    |
| Centro-Oeste | 31567    |
| Norte        | 17661    |

### 🔹 Investigando as avaliações e sua relação com o tempo de entrega

![texto do link](https://github.com/afonsosr2/estatistica-r-frequencias-medidas/blob/main/imagens/outros/relacao_media_mediana_moda.png?raw=true)

<img width="589" height="432" alt="image" src="https://github.com/user-attachments/assets/24c67961-3046-43ce-8119-d079ea9eab1b" />

<img width="589" height="432" alt="image" src="https://github.com/user-attachments/assets/f14b91e2-cc09-437f-9d79-fe6012398b87" />

### 🔹 Iniciando as análises da remuneração dos colaboradores

# $$k = 1 + \frac {10}{3}\log_{10}n$$



