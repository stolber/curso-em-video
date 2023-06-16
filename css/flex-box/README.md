# Flex Container 🔲

O modelo de layout Flexbox permite criar layouts flexíveis e responsivos. O elemento pai que contém os itens flexíveis é chamado de flex container.

## display

A propriedade `display` define o tipo de exibição do elemento. Para criar um flex container, você precisa definir `display: flex` no elemento pai.

Exemplo:

```css
.container {
  display: flex;
}
```

## flex-direction

A propriedade `flex-direction` determina a direção dos itens flexíveis dentro do container. Existem quatro valores possíveis: `row`, `row-reverse`, `column` e `column-reverse`.

- `row` (padrão): os itens são dispostos na mesma direção do texto, da esquerda para a direita.
- `row-reverse`: os itens são dispostos da direita para a esquerda.
- `column`: os itens são dispostos de cima para baixo.
- `column-reverse`: os itens são dispostos de baixo para cima.

Exemplo:

```css
.container {
  flex-direction: row-reverse;
}
```

## flex-wrap

A propriedade `flex-wrap` especifica se os itens flexíveis devem ser quebrados em várias linhas ou não. Os valores possíveis são `nowrap`, `wrap` e `wrap-reverse`.

- `nowrap` (padrão): os itens são exibidos em uma única linha.
- `wrap`: os itens são quebrados em linhas adicionais, se necessário.
- `wrap-reverse`: os itens são quebrados em linhas adicionais, mas em ordem reversa.

Exemplo:

```css
.container {
  flex-wrap: wrap;
}
```

## flex-flow

A propriedade `flex-flow` combina as propriedades `flex-direction` e `flex-wrap` em uma única declaração. O primeiro valor representa `flex-direction` e o segundo valor representa `flex-wrap`.

Exemplo:

```css
.container {
  flex-flow: row wrap;
}
```

## justify-content

A propriedade `justify-content` alinha os itens flexíveis ao longo do eixo principal. Ela controla o espaço extra no container quando os itens não preenchem todo o espaço disponível. Existem cinco valores possíveis: `flex-start`, `flex-end`, `center`, `space-between` e `space-around`.

- `flex-start` (padrão): os itens são alinhados no início do container.
- `flex-end`: os itens são alinhados no final do container.
- `center`: os itens são centralizados no container.
- `space-between`: os itens são distribuídos igualmente ao longo do eixo principal.
- `space-around`: os itens são distribuídos igualmente ao longo do eixo principal, com espaçamento igual nas extremidades.

Exemplo:

```css
.container {
  justify-content: center;
}
```

## align-items

A propriedade `align-items` alinha os itens flexíveis ao longo do eixo transversal. Ela controla o alinhamento vertical quando os itens têm alturas diferentes. Existem cinco valores possíveis: `flex-start`, `flex-end`, `center`, `baseline` e `stretch`.

- `flex-start` (padrão): os itens são alinhados no início do eixo transversal.
- `flex-end`: os itens são alinhados no final do eixo transversal.
- `center`: os itens são centralizados no

 eixo transversal.
- `baseline`: os itens são alinhados com a linha base.
- `stretch`: os itens são esticados para preencher o container verticalmente.

Exemplo:

```css
.container {
  align-items: center;
}
```

## align-content

A propriedade `align-content` controla o comportamento dos itens flexíveis quando eles são distribuídos em várias linhas. Ela tem o efeito quando há espaço extra no eixo transversal. Existem seis valores possíveis: `flex-start`, `flex-end`, `center`, `space-between`, `space-around` e `stretch`.

- `flex-start`: os itens são agrupados no início do eixo transversal.
- `flex-end`: os itens são agrupados no final do eixo transversal.
- `center`: os itens são centralizados no eixo transversal.
- `space-between`: os itens são distribuídos igualmente ao longo do eixo transversal.
- `space-around`: os itens são distribuídos igualmente ao longo do eixo transversal, com espaçamento igual nas extremidades.
- `stretch` (padrão): os itens são esticados para preencher o container verticalmente.

Exemplo:

```css
.container {
  align-content: space-between;
}
```

# Flex Item 🔳

Os itens dentro do flex container são chamados de flex items.

## flex-grow

A propriedade `flex-grow` especifica a capacidade de crescimento de um item flexível em relação aos outros itens flexíveis dentro do mesmo container. Ela determina como o espaço extra é distribuído entre os itens. O valor padrão é `0`.

Exemplo:

```css
.item {
  flex-grow: 1;
}
```

## flex-basis

A propriedade `flex-basis` define o tamanho inicial de um item flexível antes que ele seja alocado no espaço disponível. Ela pode ser especificada em pixels, porcentagem ou `auto`. O valor padrão é `auto`.

Exemplo:

```css
.item {
  flex-basis: 200px;
}
```

## flex-shrink

A propriedade `flex-shrink` especifica a capacidade de encolhimento de um item flexível em relação aos outros itens flexíveis dentro do mesmo container. Ela determina como o espaço é reduzido quando os itens não têm espaço suficiente para caber no container. O valor padrão é `1`.

Exemplo:

```css
.item {
  flex-shrink: 0;
}
```

## flex

A propriedade abreviada `flex` combina `flex-grow`, `flex-shrink` e `flex-basis` em uma única declaração. O valor `flex` padrão é `0 1 auto`.

Exemplo:

```css
.item {
  flex: 1 0 200px;
}
```

## order

A propriedade `order` especifica a ordem em que os itens flexíveis são exibidos dentro do container. Os itens com um valor `order` menor são exibidos antes dos itens com um valor `order` maior. O valor padrão é `0`.

Exemplo:

```css
.item {
  order: 2;
}
```

## align-self

A propriedade `align-self` substitui o valor definido pela propriedade `align-items` do container para um item flexível específico. Isso permite o controle individual do alinhamento de um item em relação aos outros itens no container.



Exemplo:

```css
.item {
  align-self: flex-end;
}
```

Essas são as principais propriedades relacionadas ao layout flexbox. Utilizando essas propriedades em conjunto, você pode criar layouts flexíveis e responsivos com facilidade.