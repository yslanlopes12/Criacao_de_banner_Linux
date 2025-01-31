**Para quem está iniciando no mundo da cibersegurança, infraestrutura ou áreas similares, sabe como é difícil criar suas próprias ferramentas e programas. 
A maioria das vezes, o resultado é uma ferramenta funcional, mas sem um apelo visual interessante. E, convenhamos, um script sem estilo fica desinteressante
e difícil de entender por causa do excesso de texto.**

Pensando nisso, decidi compartilhar uma ferramenta que pode ajudar bastante no desenvolvimento e personalização das suas ferramentas no Linux,
tornando o processo muito mais divertido e visualmente atrativo: *Figlet* e *Lolcat*!

🔹 **Figlet:** Essa ferramenta no Linux converte qualquer texto simples em um letrão estilizado, super útil para criar banners, 
avisos ou qualquer outro tipo de personalização nos seus scripts. Vai deixar sua ferramenta muito mais atraente e impactante.

🔹 **Lolcat:** Agora, se você quer adicionar um efeito visual de arco-íris ao seu texto, o Lolcat é a escolha certa. 
Ele deixa a saída de texto no terminal mais divertida e colorida, com aquele efeito animado que todo terminal hacker deveria ter.

Com essas ferramentas, vou ensinar a vocês como usar os comandos para personalizar seus scripts e torná-los bem TOP. No mundo atual, 
não basta ser bom, tem que saber vender a sua ferramenta. Se você deseja compartilhar, vender ou até deixar a sua criação famosa, 
o design também é parte fundamental do processo!

Passo 1: Baixar Ferramentas no Terminal do Linux
  - 
Primeiro vc abre seu terminal e digite os seguintes códigos:
```` 
sudo apt install figlet  lolcat
````

- Caso dê erro, indico que você faça o update e o upgrade do seu linux, caso isso não funcione também, peço que investigue o que seja, pode ser algumas extensões do *Ruby*, 
então use este código que talvez funcione, funcionou comigo e talvez funcione com vc:

````
sudo apt install ruby-paint ruby-optimist
````
Agora é só sucesso!

Passo 2: Testar
-
Digite:
``
figlet 'Hello!'
``
- Ele criou o texto como se fosse um título.

Agora digite:
``
figlet -c  'Hello!'
``
- Agora ele centralizou o título.

Agora digite:
``
figlet -cf slant  'Hello!'
``
- Agora ele centralizou e ainda deixou *itálico*

Agora digite:
``
figlet -cf slant  'Hello!' | lolcat 
``
- Agora ele coloriu seu título.

Extra: animar e colorir
-

Agora digite:
``
echo 'Hello!' | lolcat -a -d 500
``
- Você pode usar a opção -a para animação e -d para duração, ou seja, 500 .
foi uma ajuda rapidinha 
