# O que é Utility First

É uma abordagem de uso do CSS, que tem como objetivo priorizar a estilização por meio da chamada de **classe utilitárias**, estas por suas vez representam as propriedades do CSS, como font-size, background, color, border etc.

**Utility first** (utilitário primeiro) que também é chamado de **Functional CSS** (CSS funcional), compartilha alguns princípios da **programação funcional**, como por exemplo a imutabilidade., composição, previsibilidade e prevenção de efeitos colaterais.

Imagine que você tenha em um projeto diversos cards iguais que compartilham de uma mesma classe de estilização, porém, caso você quisesse que um card tivesse um determinado estilo próprio, como você resolveria isso? Se alterar a classe .card, que é usada por todos, irá mudar todos os estilos de uma vez só e não é isso que você deseja. Ah então é só adicionar um outro seletor específico para esse card! Não é bem por aí, pois dessa forma, esse card irá carregar dois seletores, sendo que um deles irá sobrescrever o outro e isso não é o ideal. Solucionamos essa questão com CSS Funcional, onde apenas é atrelado ao elemento, a propriedade que de fato precisa.

A ideia de composição traz que as classes são adicionadas uma a uma ao elemento o construindo, compondo com suas características, ao invés de simplesmente herdá-las, o que faz com que praticamente não seja necessário sobrescrever uma propriedade.

Quando trabalhamos em um projeto e ele vai se tornando cada vez maior as classes utilitárias podem ser uma grande aliada! Isso porque nós conseguimos mensurar mais facilmente *o que exatamente está sendo aplicado em determinado elemento*, tornando tudo mais previsível de identificar e realizar manutenções. A atuação desse conceito em conjunto com a abordagem de composição ao invés de herança resulta na prevenção de efeitos colaterais no layout.

## Vantagens:

1. Não se preocupe com qual nome faz mais sentido para a classe do elemento.
1. Estilize de forma rápida e sem escrever código CSS.
1. Faça mudanças mais facilmente e sem efeito colateral.
1. Construa um layout com ajuda de estilos pré definidos mas que tenham uma leque enorme de possibilidades.