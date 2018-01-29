# Dados Computados

Além dos methods, data, temos também o computed. O computed é onde incluímos dados que precisam ser computados. Essa função é útil quando precisamos fazer algum procedimento em nosso dado antes de exibi-lo.

Nós já aprendemos que é possível colocar expressões dentro do mustache. Todavia, nem sempre uma expressão vai ser tão simples quanto concatenar um nome e um sobrenome. Eventualmente podemos precisar tratar esse dado com uma lógica mais complexa, e o código pode ficar pouco legível e ruim para dar manutenção. 

```vue
<p>{{nome + sobrenome}}</p>
```

Usando o computed podemos colocar essa lógica dentro do script e não mais diretamente no template. Exemplo:

```vue
data: {
  nome: 'Maria',
  sobrenome: 'da Silva'
},
computed: {
  pessoa() {
    return this.nome + ' ' + this.sobrenome
  }
}
```

Um dado computado pode ser chamado no template como uma propriedade do data.

```vue
<p>{{pessoa}}</p>
```