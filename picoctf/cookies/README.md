# Cookies

## Visão Geral

Pontos: 40
Categoria: Web Exploitation

## Descrição

Quem não gosta de cookies? Tente descobrir o melhor. <http://mercury.picoctf.net:54219/>

## Abordagem

O link leva a algo parecido com isso:

página inicial

Digitei "snickerdoodle" e pressionei Enter.

> I love snickerdoodle cookies!

Pressionar Ctrl + Shift + I revelará algumas coisas, navegue até o armazenamento e encontre o armazenamento de cookies.

Notei que há um único cookie com um valor de 0. Alterei o valor para 1 e atualizei a página.

> I love chocolate chip cookies!

Continuei aumentando o valor numérico de "value" em 1 até chegar a 18, quando o flag foi exibido:

Flag
picoCTF{3v3ry1_l0v3s_c00k135_96cdadfd}
