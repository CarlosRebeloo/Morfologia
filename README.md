<h1 align="center">Morfologia</h1>
<h3>Sobre o projeto</h3>
<p>O projeto consiste em uma aplicação de processamento de imagem utilizando as bibliotecas OpenCV e NumPy. O objetivo é realizar operações morfológicas, como erosão, dilatação, gradiente, abertura e fechamento em imagens em escala de cinza. Sintetizando o assunto as operações morfologicas são técnicas de processamento de imagem que manipulam a forma e a estrutura dos objetos presentes na imagem, utilizando operações de erosão, dilatação, abertura, fechamento, entre outras, para realizar filtragem, segmentação e manipulação de imagens. O projeto foi criado na ferramenta Google Colab</p> 

<h3>Como foi feito:</h3>
<p>O código inicia importando as bibliotecas necessárias para a aplicação de operações morfológicas em imagens, como a biblioteca cv2 da OpenCV e a biblioteca NumPy. Além disso, é importado o módulo "cv2_imshow" para exibir as imagens no ambiente do Google Colab.

Em seguida, são carregadas três imagens a serem processadas: "j.png", "j_ruido.png" e "j_furos.png". Essas imagens são carregadas em escala de cinza usando a função cv2.imread e atribuindo variáveis.

É criada uma matriz chamada "kernel" com dimensões 5x5, preenchida com o valor 1. Essa matriz é utilizada como elemento estruturante para as operações morfológicas.

O código realiza as operações de erosão e dilatação na imagem "j.png" utilizando o kernel definido. Essas operações são realizadas duas vezes, indicadas pelo parâmetro "iterations = 2". Os resultados das erosões e dilatações são armazenados nas variáveis "erosion" e "dilation", respectivamente.

Em seguida, é aplicada a operação de gradiente morfológico na imagem "j.png" utilizando o kernel. Essa operação destaca as bordas dos objetos na imagem e o resultado é armazenado na variável "gradient".

O código aplica a operação de abertura morfológica na imagem "j_ruido.png" para remover ruídos e objetos pequenos. A operação de fechamento morfológico é aplicada na imagem "j_furos.png" para preencher lacunas e conectar componentes quebrados. Os resultados são armazenados nas variáveis "opening" e "closing", respectivamente.</p>

Por fim, o código exibe as imagens originais e as resultantes das operações morfológicas, permitindo a comparação visual dos efeitos.
