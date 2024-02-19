# Componentes visuais

Ao longo do meu trabalho percebi dificuldade no entendimento do que é um padrão visual, que nome dar a ele e até onde vai sua implementação. É importante saber o que é um componente visual, pois é ele que será incluído no CSS. Componente não são somente aquelas construções feitas em frameworks como React, os componentes visuais no CSS são padrões que podem ser reutilizados com ou sem um framework para gerar o HTML.

Componente é auto suficiente. Ele não depende de nenhum outro para existir. A composição dele pode ser feita por outros componentes, porém ele não precisa ter um pai específico ou estar combinado com outros componentes. O padrão visual é algo que muitas vezes não visto por quem está criando o componente. As interferências mais comuns para isso são quando o componente possui algumas diferenças visuais, chamadas de variantes ou modificações, também acontece quando o conteúdo é diferente ou quando se comporta de outra forma. Quem está elaborando os componentes precisa ser resistente a essas diferenças e conseguir enxergar o componente ali.

## Conteúdo ⚔ Visual

Muito da falta de reaproveitamento vem quando não conseguimos ver um padrão visual, pois há uma diferença em seu conteúdo. Um bom exercício é imaginar aquele padrão visual borrado.

![image](https://user-images.githubusercontent.com/27368585/124002320-f7811900-d9ab-11eb-9f2e-162c87b93209.png)

Se o conteúdo não importa, o nome do componente não deve ser baseado nele.

![image](https://user-images.githubusercontent.com/27368585/124010890-ce658600-d9b5-11eb-9bf3-1ba7dc7495ae.png)

## Variante

Um bom exercício é tentar imaginar um elemento visual ao lado de outro e comparar eles.

## Lógica ⚔ Visual

Não confunda eles, um botão que abre uma modal, visualmente não é um "botão de modal". Sempre perceba os padrões visuais, ignore sua lógica ou qualquer comportamento que não esteja atrelado ao componentes.

## Comportamento 💙 Visual

Diferente dos itens acima, o comportamento importa para a definição do componente. Um ícone que se comporta como botão não pode ser apenas um ícone. Quando o componente tem uma aparência e se comporta como outro componente o comum é fazer o componente baseado no comportamento e utilizar o componente que da a aparência para compor ele.

![image](https://user-images.githubusercontent.com/27368585/124006272-6a8c8e80-d9b0-11eb-99c6-dd8f7c9d573f.png)

![image](https://user-images.githubusercontent.com/27368585/124006192-53e63780-d9b0-11eb-9ee8-8e62afca9e91.png)

## Onde começa e termina um componente visual

Entender o mínimo para ser um componente visual e o limite de onde seus padrões terminam e começam outros padrões menores é uma das dificuldade que identifiquei na minha jornada como dev. Há duas abordagens que vejo para os padrões visuais que podem ser adotadas, a primeira atômica e a outra monolítica.

### Atômico

Esse termo não foi eu que cunhei, os componente atômicos já são bem famosos. Considero essa mais escalável que a outra abordagem. Ela consiste em enxergar um componente como a menor parte de um layout, onde seja possível identificar:

1. nome
2. função
3. independência do entorno

Identificando as menores partes do layout pode ir indo para partes maiores, pois como sugere o Atomic Design, os átomos são a menor parte, mas depois vêm as moléculas formadas de átomos e depois organismos... Assim vai aplicando o mesmo exercício de encontrar essas 3 características.

### Monolítico

Da forma monolítica se pensa em fazer tudo como um componente só, sem se importar com o tamanho, apenas, claro, tenha como dar uma nome, tenha função clara e seja independente, assim como no modelo atômico. A diferença aqui é que faz o componente grande e futuramente quando for percebido uma repetição de algum padrão dentro dele que seja extraído para gerar novos componente menores também com as três características já mencionadas.





