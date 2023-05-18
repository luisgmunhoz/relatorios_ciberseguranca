# Insp3ct0r

## Visão Geral

Pontos: 50
Categoria: Web Exploitation

## Descrição

Kishor Balan tipped us off that the following code may need inspection: <https://jupiter.challenges.picoctf.org/problem/44924/> (link) or <http://jupiter.challenges.picoctf.org:44924>

## Abordagem

Aqui, vemos um site com pouco conteúdo. Somos sugeridos pela declaração do problema para "inspecionar" o site. Usando as ferramentas de desenvolvimento de um navegador, podemos ver o código-fonte do site. No Chrome, esta é a opção Inspecionar elemento, que pode ser encontrada clicando com o botão direito do mouse ou Ctrl+Shift+C no Windows, Cmd+Shift+C no Linux/MacOS. Em seguida, vamos para a guia Origem e visualizamos os arquivos index.html, mycss.css e myjs.js, cada um contendo uma parte do sinalizador.

[primeiraparte](primeiraparte.png)

[segundaparte](segundaparte.png)

[terceiraparte](terceiraparte.png)

## Flag

picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?f10be399}
