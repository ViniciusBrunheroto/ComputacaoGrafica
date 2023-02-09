# ComputacaoGrafica
Disciplina de Computação Gráfica ministrada pelo profº Denis Salvadeo na Unesp de Rio Claro


--------------------------Atividade 1: Geração de Linhas e Circunferências-------------------------------------------------

1. Implemente um método na classe Line do código usado na aula que gera linhas em
diferentes estilos (tal como pontilhado, traço e ponto), recebendo como entrada
as extremidades do segmento (x1,y1) e (x2, y2), além de um padrão a ser
desenhado (um vetor de bits). Por exemplo, no caso de traço e ponto o
padrão poderia ser algo como [1 1 0 1 0]. Para tracejado seria algo
como [1 1 0], por exemplo. Para uma linha pontilhada, poderia ser  [1 0]. Incluir 3
exemplos dos resultados gerados.


2. Implemente um método na classe Circle do código usado na aula que gere um
círculo preenchido com determinada cor diferente da borda, baseado no Algoritmo
de Bresenham, recebendo como entrada o (xC,yC) do centro, o raio e a cor de
preenchimento. Incluir 3 exemplos dos resultados gerados.


3. Implemente um método na classe Circle do código usado na aula que gera círculos
preenchidos em diferentes estilos (quadriculado, por exemplo), recebendo como o
(xC,yC) do centro, o raio, além de um padrão a ser desenhado (uma pequena
matriz representando o padrão, tal como 2x2 ou 3x3). Por exemplo, no caso de quadriculado,
poderia ter uma matriz 2 x 2 com valores binários [1 0; 0 1]. Incluir 3
exemplos dos resultados gerados. SUGESTÃO: Combinar a solução pensada em (1) e (2).


--------------------------Atividade 2: Preenchimento de polígonos-------------------------------------------------


1. Estenda o código em Python criando um método que recebe uma tabela de arestas ativas (AET) 
de uma determinada linha de varredura e retorna uma lista com as paridades em cada aresta. 
Por exemplo, para o polígono do exemplo de aula, e a AET correspondente à linha de varredura y = 8, 
nós teremos 4 arestas sendo interceptadas, sendo que o algoritmo de paridade retornaria a sequência 1 0 1 0 para o bit de paridade em cada aresta. 
Faça ao menos 3 exemplos de linha de varredura para mostrar o funcionamento.


2. Modifique a implementação do algoritmo Scanline para gerar áreas preenchidas com determinado padrão de preenchimento (hachuras). 
A ideia é fazer uma implementação que aceite qualquer padrão passado como parâmetro. Uma ideia consiste em usar uma matriz para representar um padrão, 
composto de valores 0 e 1 que definem a hachura a ser desenhada. Faça 3 exemplos usando três padrões diferentes. DICA: Lembre do preenchimento de circunferências.




--------------------------Atividade 4: Objetos 3D-------------------------------------------------
Q1. Adicionar um método generateNormalVector na classe Polygon

Q2. Crie uma classe Object 3D (herdando de Primitive), formado por um conjunto de planos (possui lista de faces poligonais).

Q3. Estenda a classe Object 3D para criar uma classe Parallelepiped (com base em x, y e z, mínimos e máximos, fornecidos pelo usuário). 
OBS: Criar as 6 faces poligonais internamente

Q4. Crie um método privado isBackFace em Object 3D, que recebe dois vetores (Normal e Zview) e retorna se isso corresponde a uma face traseira

Q5. Crie um método cullBackFace em Object 3D que elimina faces traseiras e adicione esta chamada no pipeline
