# Processamento Digital de Imagens – Prof. Bruno Fernandes

## Atividade 1

### Tópico 1 – Redimensionamento de imagens

1. Implemente uma metodologia para aumentar o tamanho das imagens, de forma que a imagem fique na resolução objetivo.

| Imagem      | Resolução Original | Objetivo   |
|-------------|-------------------|------------|
| `img_1.png` | 500 x 500         | 1280 x 720 |
| `img_2.png` | 300 x 277         | 640 x 480  |
| `img_3.png` | 360 x 403         | 640 x 480  |

2. Componha uma única imagem com a img1, img2, img3 (em ordem qualquer, uma do lado da outra). A resolução final tem deve ser HD (1280x720).

---

### Tópico 2 – Contraste e brilho

3. As imagens: `gato.jpg`, `Recife_antigo.jpg` e `upe.jpg` foram alteradas. Faça os ajustes necessários para que os detalhes fiquem mais nítidos.

---

### Tópico 3 – Filtros espaciais

4. Remova o ruído das imagens `cc-w.jpg`, `saturn.png` e `toro.jpg` de modo a deixar os detalhes mais nítidos.

5. Note que a imagem `cc-c.jpg` possui uma distribuição do musgo semelhante ao ruído salt-and-pepper, tente removê-lo.

---

### Tópico 4 – Desafio

6. Uma aplicação muito comum de visão computacional é o reconhecimento de caracteres, conhecido como OCR (*Optical Character Recognition*). Um exemplo frequente dessa aplicação é o reconhecimento de placas de veículos, ou LPR (*License Plate Recognition*). Um problema comum em sistemas de LPR é o *motion blur*, que ocorre devido à velocidade do obturador da câmera. Quanto mais tempo o obturador fica aberto, mais luz entra na câmera e, consequentemente, maior é o blur que uma imagem pode apresentar se o objeto fotografado/filmado está em movimento.

A figura abaixo ilustra a relação entre a velocidade do obturador e o blur:

![Figura com bonecos em diferentes velocidades de obturador](imagem_ilustrativa)

> **Descrição da figura presente no PDF:**  
> A figura mostra um boneco estilizado (silhueta de uma pessoa) repetido em duas linhas, cada um associado a um valor de velocidade do obturador (em segundos). Os valores vão de `1/1000` a `1/2`. Conforme o tempo de exposição aumenta (denominador menor), a silhueta do boneco fica cada vez mais desfocada (*motion blur*). A linha superior apresenta os valores: 1/1000, 1/500, 1/250, 1/125, 1/60; a linha inferior: 1/30, 1/15, 1/8, 1/4, 1/2. As primeiras figuras são nítidas, e as últimas aparecem como borrões.

O blur em cenários de LPR pode ser facilmente mitigado pelo aumento da velocidade do obturador. Contudo, as câmeras possuem um limite físico de velocidade máxima e, às vezes, por falta de recursos, não é possível adquirir uma câmera com maior velocidade. Assim, para tentar reduzir esse ruído, podemos recorrer ao processamento digital da imagem. Faça um algoritmo que melhore a nitidez das informações da placa na imagem `car.jpg`.

---

## Observações

- As imagens devem ser processadas em escala de cinza.
- Apresente os histogramas e faça uma análise das imagens originais e resultantes de cada questão.
- A solução deve ser capaz de funcionar em qualquer máquina sem necessidade de muitos comandos de instalação. Recomendamos utilizar o Google Colab para apresentar as atividades.
- As partes do código relacionadas ao processamento das imagens devem ser implementadas pelo aluno sem o uso de bibliotecas de terceiros. Pode-se usar o Numpy para as operações de array.
