# O que é o React?

O React é uma`biblioteca`para criar interfaces, que foi idealizada pela galera do Facebook e Instagram.

Ele funciona como o`V`do`MVC`, permitindo criar seus próprios componentes. Numa aplicação em React, você deve quebrar os diferentes elementos dela em pequenos componentes reutilizáveis. Cada vez que algo for complexo, quebre em pequenas partes e desenvolva esses componentes, essa técnica é chamada de`component driven development`.

**Mas e esse React? É tipo um Angular né?**

Não, não, não e não! O Angular é um`framework`, ou seja, um conjunto de ferramentas para resolver vários tipos de coisas. Já uma biblioteca serve para resolver uma coisa em específico, no caso do React é renderizar componentes.

##  Como funciona?

A principal mágica do React é de fato o uso do`Virtual DOM`, mas como ele funciona?

Como todos sabemos o`DOM`é super lento e devemos evitar ao máximo manipulá-lo em excesso, visto que precisaríamos fazer muitos repaints e reflows, que iriam custar muito para o nosso browser.

**É aí que o React brilha!**

Quando um componente é inicializado, o método`render`é chamado, gerando uma representação da view. Dessa representação, um markup é produzido e injetado no documento. Quando algum dado muda, o método`render`é chamado novamente e para que tenhamos uma atualização mais eficiente possível, o React faz um diferenciação \(`diff`\) do valor novo com o valor velho e aplica no DOM somente a nova mudança.

Segue um exemplo abaixo:

  


