## Javascript

Vamos começar a desbravar o fantástico mundo do [Javascript](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/First_steps), a linguagem de programação mais popular do mundo, muito poderosa e que está em todos os lugares. Podemos encontra-la em robôs, aplicações web, mobile, e em tantas outras coisas, inclusive em seu navegador.

Faça o teste! Clique com o botão direito do mouse em qualquer lugar na tela e pressione Inspecionar elemento ou pressione `(ctrl + shift + i)` e clique em Console.

Digite o comando alert`("Olá mundo");`

O `alert();` é uma função em Javascript, não se preocupe em conhecer o conceito disso agora, ele vai ficar mais claro nas próximas aulas, por enquanto entenda isso como uma ação.

## VueJS

Criada e mantida pela comunidade Open Source. É um framweork em Javascript para construção de **interfaces** com o usuário.

> Uma interface com o usuário é um espaço em que interações entre humanos e máquinas acontecem.
> Wikipedia

O desenvolvimento que acontece no browser, ou frontend, foi ficando muito complexo com o passar dos anos e as pessoas começaram a pensar formas para tornar esse desevovlvimento melhor e mais simples. Uma dessas formas, é a **componentização**.

Uma interface pode ser divida em **componentes**, e esses componentes se comunicam entre eles. Podemos dividir uma interface em vários componentes.

Um componente tem algumas características especiais, ele costuma ser dividido em unidades pequenas, um bom indicador que um componente precisa ser dividido em outros componentes é o tamanho ou complexidade de seu código por exemplo. Uma outra característica é que um componente também é altamente especializado, ou seja, um componente tem como responsabilidade fazer uma determinada coisa e deve fazer essa coisa de forma bem feita.

Componentes também devem permitir composição, ou seja, diversos componentes criam funcionalidades que compõem uma aplicação. Uma outra coisa legal também é que você consegue atingir um famoso conceito em programação que em inglês é chamado de DRY, ou don't repeat yourself, que em português quer dizer não repita a si mesmo. Funciona como lego, eu tenho uma pecinha que eu posso reaproveitar em mais de um lugar em minha construção, assim eu eu não preciso cria-lo novamente, repetindo assim um processo que já foi feito antes.

Interfaces web modernas construídas em VueJS têm componentes **reativos**, ou seja componentes que reagem às interações com o usuário, se o usuário insere um dado de entrada em um componente por exemplo, esse componente pode mostrar em tempo real uma reação a essa entrada.

Há muitas bibliotecas criadas para resolver os mesmos problemas que o Vue foi criado para resolver, não se apresse em conhecer outras ainda, por enquanto entenda que optamos por começar com o Vue por sua simplicidade.

## Criando um projeto

Vamos usar o Vue-cli, ele nos dá alguns templates para criar a estruta inicial de nossos projetos. Enquanto estamos conhecendo o Vue, vamos usar o [webpack](http://vuejs-templates.github.io/webpack/structure.html), que possui o **Webpack** configurado, **vue-router** já estruturado e mais algumas coisas que vão facilitar a nossa vida.

Com tudo instalado corretamente, use o comando para iniciar o projeto:

```bash
vue init webpack MeuProjeto
```

Ele vai te perguntar algumas coisas durante o processo de instalação, aperte enter para continuar quando ele te perguntar o nome do projeto, autor e descrição. Digite Y quando ele te perguntar sobre o Vue-Router, e depois N quando ele te perguntar sobre testes, não precisaremos disso agora. Por fim, entre na pasta criada

```bash
cd MeuProjeto
```

Sempre que iniciamos um novo projeto em nossa máquina, precisamos instalar as dependências dele. Instale as dependências de seu projeto

```bash
npm install
```
O Vue-cli já criou várias pastas e arquivos para gente a partir do template que usamos. Essa é a nossa estrutura de pastas que ele criou:

```
.
├── build/                      # arquivos de configuração do webpack
│   └── ...
├── config/                     # configurações de compilação
│   └── ...
├── src/
│   ├── main.js                 # raíz da aplicação
│   ├── App.vue                 # componente raíz
│   ├── components/             # outrios componentes da interface
│   │   └── Hello.vue           # olá mundo
│   └── assets/                 # assets do projeto (processados com webpack)
│       └── ...
│   └── router/                 
│       └── index.js            # configuração das rotas usando router
├── static/                     # outros assets
├── .babelrc                    # configurações do babel
├── .postcssrc.js               # configurações do postcss
├── .editorconfig               # configurações do editor
├── index.html                  # index.html template
└── package.json                # scripts, dependências, e outras descrições do projeto
```
Agora já podemos iniciar o projeto

```bash
npm run dev
```
Nossos componentes ficam dentro de src/components. Ele criou também um componente chamado Hello.vue, podemos apagar ou editar esse componente, depois criar novos. 

Vá em frente! Abra em seu editor de códigos o Hello.vue, encontre a frase Welcome to Your Vue.js App na linha 28, apague essa frase e escreva seu primeiro Olá mundo.