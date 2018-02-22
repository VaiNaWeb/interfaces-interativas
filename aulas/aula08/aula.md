# Comunicação entre componentes

Já aprendemos interfaces em Vue podem ser compostas de vários componentes. Naturalmente, vamos precisar trocar informações entre esses componentes.

A forma mais simples como isso acontece se dá através da própria árvore de componentes, onde um filho recebe dados do seu componente pai. Vamos a um exemplo prático!

Navegando numa famosa rede social, podemos perceber que há um componente que se repete em mais de um lugar. Se você abrir a rede social você sabe qual, e em diversos outros sistemas, pode procurar, que você vai encontrar muitos componentes se repetindo em várias páginas ou simplesmente lugares diferentes dentro da mesma tela. Essa é uma das características ou vantagens de componentes, eles permitem o seu reuso.

![exemplo de componente](assets/componente.png "exemplo de componente")
![exemplo de componente](assets/componentes.png "exemplo de componente")
