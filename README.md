# prova-computacao-em-nuvem

nome:João Gabriel de Souza Lima

saida do comando docker ps: 

CONTAINER ID   IMAGE         COMMAND                  CREATED          STATUS          PORTS                                      NAMES
3ff77e2598ee   nginx:alpine  "/docker-entrypoint..." About a minute ago Up About a minute 0.0.0.0:8081->80/tcp, [::]:8081->80/tcp   loja

 A resposta do comando curl http:/localhost:8081: 
 
 !DOCTYPE html
html lang="pt-BR"
head
meta charset="UTF-8"
title>Loja</title
/head
body
h1>Loja no ar</h1
/body
/html

A diferença entre a imagem nginx:alpine e o conteiner loja? Para que serviu o mapeamento 8081:80?

A imagem nginx:alpine é uma imagem que junta o Nginx com o Alpine Linux.

O Nginx é o servidor web que fica responsável por entregar o arquivo index.html.

O Alpine é uma distribuição Linux pequena e leve, usada como base para a imagem do Nginx.

O container loja é a instância que foi criada a partir da imagem nginx:alpine. É dentro desse container que o Nginx está rodando e mostrando a minha página. O mapeamento 8081:80 serviu para ligar a porta 8081 da minha máquina à porta 80 do container. Assim, quando eu acesso:

http://localhost:8081

a requisição é enviada para a porta 80 do container, onde o Nginx está rodando e entregando a página index.html.





