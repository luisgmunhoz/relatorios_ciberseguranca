# Get aHead

## Descrição do Desafio

Encontre a flag que está sendo mantida neste servidor para se adiantar na competição [http://mercury.picoctf.net:45028/]
<http://mercury.picoctf.net:45028/>)

## Informações

Pontos: 20

## Dicas

1. Talvez você tenha mais do que 2 opções.

2. Confira ferramentas como o Burp Suite para modificar suas solicitações e analisar as respostas.

## Solução

Ao verificar o Burp Suite, uma de suas principais capacidades é interceptar e modificar solicitações. [Burp Suite](https://www.sciencedirect.com/topics/computer-science/burp-suite)

A partir daqui, vemos que o método usado para o Vermelho foi "GET" e para o Azul foi "POST". Podemos fazer mais pesquisas sobre eles, pois são diferentes solicitações HTTP.

Faz sentido, pois descobrimos anteriormente que o Burp Suite pode interceptar e alterar solicitações. Ao percorrer a lista, vemos que o segundo método de solicitação é "HEAD", que parece bastante familiar. Se voltarmos para o título do desafio "Get aHead", a palavra "Head" se destaca, provavelmente se referindo ao método de solicitação HTTP "HEAD".

Após abrir o aplicativo (ele é baixado como um aplicativo), escolha a opção "request" e crie uma pastaiser. A partir daí, insira o link do site na barra "Enter request url", altere o método para "HEAD" e clique em enviar. Agora, encontre a flag na guia headers "Headers"!

## Flag

picoCTF{r3j3ct_th3_du4l1ty_775f2530}
