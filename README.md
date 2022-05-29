<img src ='https://i.pinimg.com/originals/f7/0d/a5/f70da59711a903515d6aed0ee62b92cc.jpg' align = "center"><br><br>
# Análise de Dados: Vendas de Jogos de Videogame
--<br><br>
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)<br>

--

## Sobre o Estudo

Este notebook apresenta um estudo de **análise de dados** provenientes do dataset <a href="https://www.kaggle.com/datasets/gregorut/videogamesales">Video Game Sales</a> publicado pelo usuário Gregory Smith no Kaggle quem contém diversas informações a respeito de vendas de jogos de videogames durante as décadas de 1980, 1990, 2000 e 2010.

## Desenvolvimento

Este estudo foi realizado em duas principais partes: 

### 1ª - Tratamento dos dados
--

<img src ='https://cdn.startschoolnow.org/wp-content/uploads/Statistics-Descriptive-and-inferential-statistics.png' align = "center"><br><br>



Foi carregado o *dataset* no Jupyter Notebook através do método pandas.read_csv() para que fosse possível identificar o conteúdo presente no arquivo .csv.
O *dataset*, inicialmente, era compsto de 11 colunas e 16.598 linhas, com todo o conteúdo em Inglês. As colunas presentes no *dataset* estavam contidas com os seguintes registros:
> - **Rank**: Se trata da posição daquele determinado jogo no *ranking* de vendas;
> - **Name**: Se trata do título do jogo;
> - **Platform**: Se trata do console em que o jogo foi lançado;
> - **Year**: Se refere ao ano de lançamento daquele título;
> - **Genre**: Se trata do gênero daquele jogo;
> - **Publisher**: Empresa responsável pela publicação do jogo;
> - **NA_Sales**: Vendas na América do Norte, em milhões de dólares;
> - **EU_Sales**: Vendas na Europa, em milhões de dólares;
> - **JP_Sales**: Vendas no Japão, em milhões de dólares;
> - **Other_Sales**: Vendas no em outras regiões além de Japão, Europa e América do Norte;
> - **Global_Sales**: Total de vendas mundiais.

Após a apresentação inicial ao conteúdo do *dataset*, começaram, então, os tratamentos dos dados, através da tradução do Inglês para Português-brasileiro e alteração em alguns registros, visando facilitar o entendimento do conteúdo pelo leitor. Além disto, foram identificados dados sem registros e estes foram tratados de forma como melhor convinha de acordo com os objetivos do estudo.
Por fim, foram realizadas as conversões necessárias para lidar com os dados, como converter a coluna de Anos de Lançamento de *float* para *int*, anos cujos dados foram considerados incompletos também foram removidos do *dataframe* e foi realizada uma **soma** de vendas de cada jogo, incluindo as vendas em multiplataforma, para que fosse criado um *ranking* de vendas condizente com a realidade da época em que o *dataset* foi publicado, **2016**.

#### Ranking de Vendas de Jogos de 1980 até 2016 
> - 1º - Wii Sports / 82.74 milhões de cópias vendidas<br><br>
> - 2º - Grand Theft Auto V / 55.92 milhões de cópias vendidas<br><br>
> - 3º - Super Mario Bros. / 45.31 milhões de cópias vendidas<br><br>
> - 4º - Tetris / 35.84 milhões de cópias vendidas<br><br>
> - 5º - Mario Kart Wii	 / 35.82 milhões de cópias vendidas<br><br>
> - 6º - Wii Sports Resort / 33.00 milhões de cópias vendidas<br><br>
> - 7º - Pokemon Red/Pokemon Blu / 31.37 milhões de cópias vendidas<br><br>
> - 8º - Call of Duty: Modern Warfare 3 / 30.83 milhões de cópias vendidas<br><br>
> - 9º - New Super Mario Bros. / 30.01 milhões de cópias vendidas<br><br>
> - 10º - Call of Duty: Black Ops II / 29.72 milhões de cópias vendidas<br><br>

--

### 2ª - Visualizando os Dados
--

<img src ='https://cdn.startschoolnow.org/wp-content/uploads/Statistical-treatment-of-data-696x261.jpg' align = "center"><br><br>


A visualização dos dados foi realizada por meio das bibliotecas *matplotlib*, *seaborn* e *plotly* e foi feita de acordo com as colunas do *dataset*, abordando, então, os **jogos, consoles, publicadoras, ano de lançamento, gênero e regiões** respeitando as particularidades de cada categoria de dados presentes no estudo.
Através das visualizações, foi possível identificar os jogos mais vendidos, os gêneros mais populares, as empresas mais rentáveis, consoles mais populares,etc...


## Conclusão 


As principais conclusões que foram feitas por meio do estudo foram:<br><br>
- Até 2016, o **jogo mais vendido** da história dos videogames era o Wii Sports, lançado pela Nintendo para o console Nintendo Wii em 2006, com 82.74 milhões de cópias vendidas, seguido por Grand Theft Auto V da Take-Two Interactive e Super Mario Bros. da Nintendo, respectivamente.<br> <br> 
- O console que mais vendeu jogos até então segue sendo o PlayStation 2, lançado primeiramente no Japão em 4 de março de 2000 e que atingiu alta popularidade em todas as regiões abordadas no estudo.<br> <br> 
- **Ação**,**esporte** e **tiro** foram os três gêneros mais rentáveis em todas as regiões do mundo durante 1980 e 2016, exceto no Japão, onde o gênero de **RPG** foi o mais rentável.
- A Nintendo foi a publicadora que mais vendeu jogos durante o período e 7 dos 10 jogos mais vendidos foram publicados pela empresa.<br> <br> 
- A América do Norte foi a região mais rentável para a indústria dos videogames, seguida pelo Japão, durante as décadas de 1980 e 1990. A partir dos últimos anos de 1990 e durante as décadas de 2000 e 2010, a Europa passou o Japão nos números de venda e passou a ser a 2ª região mais rentável para a indústria.<br> <br> 
- Por fim, se conclui que a indústria apresentou forte expansão durante os anos de 1990 e 2000, atingindo seu ápice por volta de 2008 e, então, desacelerando seu crescimento durante os anos 2010, justamente na mesma época em que os *smartphones* começaram a ganhar espaço e o florescimento de uma nova indústria de jogos mobile.<br><br>




### Bibliotecas utilizadas
> - Pandas
> - Seaborn
> - Matplotlib
> - Plotly
> - Numpy

---

## Author:
**Luís Fernando Torres**
