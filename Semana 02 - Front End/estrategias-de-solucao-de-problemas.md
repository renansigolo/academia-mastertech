# Estratégias de solução de problemas

## Algoritmos

[![](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192539/Algoritmos-1.jpg "Algoritmos - A melhor forma de aprender lógica de programação \| Becode")](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192539/Algoritmos-1.jpg)

Alguns confundem algoritmos com logaritmos, se você já fez isso, não se preocupe, você não está sozinho no mundo \(mas agora que você já sabe que não é a mesma coisa, não repita mais hehe\).

Bem, o que é algoritmo? Basicamente é um conjunto de instruções bem definidas, finitas e que geram um resultado.

**O que!? Como?**

Bem, se você for pensar, fazemos isso todos os dias, a todo momento. Por exemplo, quando saímos de casa para ir ao trabalho. Neste caso, precisamos identificar como fazer isso: de carro, de ônibus, a pé, qual caminho fazer, quanto tempo vou demorar, enfim… precisamos determinar uma sequência de ações para resolver um determinado problema.

Pensando no mundo da TI agora, imagina um aplicativo famoso, como o _Waze_ ou o _Google Maps_, por exemplo. Dentro destes aplicativos, existem complexos algoritmos, com conjuntos de instruções e variáveis \(rotas, tempo estimado, cálculo de velocidade média etc\) que geram resultados \(chegar até o seu trabalho da melhor forma possível\), conforme a interação do usuário.

Outro exemplo, agora mais clássico: o simples ato de tomar um banho ou ir ao supermercado.

\(Escrevendo em formato de listas para organizar o pensamento\)

#### Tomar Banho

**Início**

* Pegar a toalha e roupas;
* Entrar no banheiro e fechar a porta;
* Tirar a roupa que está usando;
* Ligar o chuveiro e esperar a água ficar na temperatura certa;
* Entrar no box \(ou espaço destinado para o banho\);
* Se molhar, ensaboar, enxaguar = banho;
* Fechar o chuveiro;
* Pegar a toalha e se secar;
* Sair do box;
* Se vestir com a roupa limpa;
* Sair do banheiro.

**Fim**

Digamos que esse seja o banho padrão, mas você pode variá-lo conforme as suas preferências.

O mesmo ocorre para softwares e funcionalidades dentro de um sistema. Você escreve algoritmos, como o escrito acima, para chegar a um resultado esperado com as instruções definidas.

A diferença entre o algoritmo acima e os algoritmos de sistemas é a linguagem utilizada. Pense da seguinte forma, o algoritmo acima foi escrito de uma forma que você, humano racional,  consiga compreender, que é o português. Agora, o que precisamos fazer para que um computador entenda?

Para que um computador entenda o seu algoritmo, basicamente,  você precisará usar uma linguagem de programação, ou seja, você estará escrevendo uma sequência de passos que um computador \(que não possui habilidades de interpretação subjetiva\) deverá executar sem ficar com dúvidas, utilizando uma linguagem que é conhecida e facilmente interpretada pelo computador.

Mesmo para nós, seres humanos autodenominados como os seres mais inteligentes do planeta, há uma série de regras pré-estabelecidas para que a listinha com as instruções de como tomar banho seja compreendida, executada e gere um resultado. E acredite, os humanos são seres muito mais complexos do que computadores \(talvez daqui uns 20 anos alguém virá me dizer que estou errado, mas por enquanto, sim, somos muito mais complexos\).

OK, mas e no caso de computadores, quais regras e conceitos eu preciso saber para otimizar e melhorar meus algoritmos, de uma maneira que o computador compreenda e execute, atingido o resultado esperado?

### Variáveis e constantes

Em termos simples, são nomes que inventamos para representar um valor, para que assim, seja possível usar este mesmo valor diversas vezes naquela lista de tarefas, sem precisar reescrevê-lo todas as vezes que ele for necessário. Com o uso de variáveis, utilizamos apenas o nome de referência.

```
let minhaVariável = 'Essa é minha variável e ela guarda essa frase';
```

### Tipos de dados

Basicamente, desenvolvemos softwares, sistemas e apps para receber informações:

* Nome
* Idade
* Salário
* E por aí vai…

Para o computador, tais informações são dados. E dados podem assumir diversos formatos. Pense da seguinte forma, nome é diferente de idade que, por sua vez, é diferente de salário. Isso em lógica de programação pode ser definido como **tipos de dados primitivos**. Estes tipos existem para otimizar a memória do computador, assim, o computador consegue identificar qual é o tipo de dado que ele irá receber/interpretar.

Tratando-se de tipos de dados primitivos, são constatados quatro formatos:

#### Tipo 1: Texto

Os dados do tipo texto representam uma sequência de um ou mais caracteres. São colocados entre aspas dupla ou simples.

Um exemplo de dado do tipo texto:  `let nome = 'Meu nome é considerado um texto';`

**Obs.: **espaços também contam como caracteres.

#### Tipo 2: Inteiro

São representados por valores numéricos, tanto negativos, quando positivos \(sem casas decimais\).

Um exemplo de dado do tipo inteiro: `let idade = 18;`

#### Tipo 3: Real

Os dados do tipo real são valores numéricos, tanto positivos, quanto negativos que utilizam casas decimais,

Como exemplo, podemos citar: `let salário = 2350.00;`

#### Tipo 4: Lógico

Por último, mas não menos importante, o tipo lógico. Este tipo de dado normalmente é representado por alternativas: SIM ou NÃO, VERDADEIRO ou FALSO. Dados do tipo lógico também podem são chamados de booleano \(em homenagem à George Boole, que criou esse tipo de lógica\).

Um exemplo de dado lógico que é frequentemente utilizado em programação é para verificar se situações são verdadeiras ou falsas: `let estouComSono = false;`

Sendo assim, temos como exemplo:

* Nome: TEXTO
* Idade: INTEIRO
* Salário: REAL
* Estou com sono? NÃO \(FALSE\)

Obs.: Você deve ter percebido que colocamos as variáveis com a seguinte sintaxe:

`let <NomeDaVariável> = <Valor da variável>;`

Essa é a sintaxe que usamos no _JavaScript_ para declarar variáveis. Mas vamos aprender isso com mais calma mais para frente.

### Estrutura de seleção e repetição

Formas e estruturas organizadas de fazer com que um computador consiga tomar decisões ou executar diversas vezes uma instrução até que um limite pré-estabelecido seja atingido, ou uma condição seja satisfeita, ou o usuário intervenha. Sim, pois o computador, diferente dos humanos ainda não consegue pensar por conta própria, ele precisa de regras bem definidas para o seu correto funcionamento. Isso é alcançado através de muito treinamento e prática com lógica de programação.

## Matemática

[![](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192544/Matematica-1.jpg "Matemática - A melhor forma de aprender lógica de programação \| Becode")](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192544/Matematica-1.jpg)

Bom, quem leu o post [“Saiba se programação é para você”](https://becode.com.br/saiba-se-programacao-softwares-e-para-voce/) deve lembrar da importância da matemática na formação de um programador.

Aqui, não irei me estender muito no assunto, contudo, vale a lembrança que a matemática é um recurso extremamente forte dentro da programação, afinal você vai criar softwares que possuirão forte vínculo com a matemática. Então, se você não se sente seguro com essa área do conhecimento ainda, talvez seja interessante revisar alguns conceitos, como: operadores lógicos, aritméticos, ordens de precedência e a teoria dos conjuntos.

Tendo estes conhecimentos sólidos, sim, **aprender lógica de programação **será algo muito mais natural.

## Linguagem de Programação Inicial

Então, depois de você já ter se acostumado em pensar nas tarefas simples do dia a dia como uma série de instruções sendo executadas pelo seu “computador interior”, após ter criado listas que representem essas tarefas, depois de ter melhorado essas listas e adicionado regras matemáticas a elas, aí sim, você precisa escolher uma linguagem de programação para por em prática o que estava no papel/teoria.

Para isso, existe o [VisualG](http://www.apoioinformatica.inf.br/produtos/visualg), um aplicativo simples, em português, que vai testar todos os seus algoritmos e conhecimentos de lógica de programação. Então, depois de praticar exaustivamente os algoritmos e fazê-los funcionar de forma correta e otimizada, aí sim, podemos dar voos mais altos e escolher uma linguagem de programação de mercado para iniciar uma nova etapa, a etapa profissional de um programador/desenvolvedor.

[![](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192542/JavaScript-1.jpg "JavaScript - A melhor forma de aprender lógica de programação \| Becode")](https://d2tycqyw09ngo1.cloudfront.net/be-content/uploads/2016/06/08192542/JavaScript-1.jpg)

A linguagem que usamos é o **JavaScript\(JS\)!**

O JS é uma linguagem capaz de executar instruções bem definidas e gerar resultados na tela do seu navegador, além da vantagem de estar usando uma linguagem que você **CERTAMENTE** irá precisar em seus projetos futuros, visto que hoje o _JavaScript_ é considerado uma das linguagens mais populares do mundo.

