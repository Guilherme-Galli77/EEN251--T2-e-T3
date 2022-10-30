# Trabalho T2 e T3 EEN251 - Fechadura com Reconhecimento Facial

## Integrantes do grupo
Fernando Laiser F Kon                                   RA: 19.01336-0

Guilherme Cury Galli                                    RA: 19.00374-9

Matheus dos Santos Galbiati                             RA: 19.01324-8

Daniel Scabar                                           RA: 18.01775-4



## Video do projeto

[Link do vídeo do projeto em execução]()

## Projeto desenvolvido

A ideia central de nosso projeto foi criar uma fechadura eletronica utilizando um algoritmo de reconhecimento facial para garantir a autenticação e autorização. O sistema foi concebido para funcionar após a ativação de um botão, que realiza a captura de uma imagem através da câmera conectada ao Raspberry, essa imagem é comparada com outras dentro de um modelo de machine learning em cloud, caso haja correspondência, a fechadura é aberta. No T3 esse sistema foi adaptado para funcionar de forma remota, utilizando uma dashboard que exibe o status da fechadura.

### Imagem do circuito criado
![alt text](Imagens/WhatsApp Image 2022-10-30 at 11.37.59(4).jpeg "Circuito")



## Componentes Eletrônicos

Foram utilizados os seguintes componentes eletrônicos:

- Raspberry PI 3
- LED
- Webcam
- Protoboard
- Jumpers variados
- Mini fechadura solenoide  


## Códigos

O projeto possuí 4 arquivos em sua pasta códigos. O arquivo mrfc522.py contém as funções e procedimentos relacionados ao sensor RFID e sua execução primordial. O arquivo ssd1306.py contém as funções e procedimentos do display oled. Por fim, o arquivo teste_leitura.py é o que contém o código principal do projeto, utilizando algumas funções dos outros arquivos e sendo o principal responsável por conter o código da execução sistemica do projeto.O arquivo chaves.txt contém dados que são utilizados por esse código principal. Além dos códigos da primeira parte do projeto, para garantir a compatibilidade e funcionamento, também foi criado analyze_image.py responsável por analisar a imagem obtida pela webcam e o open_fechadura.py responsável por abrir a fechadura pós reconhecimento facial
