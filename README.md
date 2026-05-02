# LNPG - Capítulo 8: Estruturas de Seleção

**Nome:** Alicia Maria Rocha de Barros
**LLM utilizado:** ChatGPT
**Versão/modelo:** GPT-5.3

---

## Análise Comparativa das Atividades 

### [cite_start]Atividade 1: Substituição de `goto` por Laços (Java, Python, Haskell, Swift)
* **Facilidade de Escrita:** Na minha opinião, Python é a linguagem com maior facilidade de escrita nesse exemplo, porque o código fica mais curto e direto, sem precisar de muitos símbolos extras. A estrutura do while também é bem clara e fácil de entender.
* **Legibilidade:** Java foi a que achei mais fácil de ler. O uso de chaves para delimitar os blocos deixa bem claro onde cada parte do código começa e termina, o que transmite maior organização na estrutura.
* **Melhor Combinação:** Swift, na minha visão, é a que melhor equilibra os dois pontos. Ela mantém uma escrita simples, parecida com Python, mas ao mesmo tempo traz uma estrutura mais organizada, semelhante à do Java.

### Atividade 2: Sentença de Seleção Múltipla (C, Ruby, Erlang)
* **C:** Na minha visão, em C o código acaba ficando mais extenso. O uso constante de break para evitar que um caso “caia” no outro deixa a escrita mais repetitiva e aumenta a chance de esquecer algum.
* **Ruby:** Já em Ruby, achei bem mais prático. A possibilidade de colocar vários valores na mesma condição deixa o código mais limpo e com melhor legibilidade.
* **Erlang:** O Erlang tem uma estrutura interessante, pois cada condição já define o valor direto. O uso de orelse também ajuda a deixar a leitura mais clara.

### Atividade 3: Remoção de gotos e breaks (Python, Java, JavaScript)
* **Legibilidade:** Senti que a legibilidade ficou um pouco prejudicada nesse caso. Antes, com o break, era mais fácil entender onde o fluxo do código parava,mas agora sem ele é preciso analisar toda a sequência de condições para perceber quando o laço termina, o que deixa a leitura um pouco menos direta.
* **Impacto no Código:** Na minha opinião, o código acabou ficando maior em todas as linguagens. Ao retirar o switch/case e também o uso de break, foi necessário usar vários if/else e ainda uma variável extra (continuar) para controlar o fim do laço, o que deixou a implementação mais extensa.

### Atividade 4: Construção `for` em 5 linguagens diferentes 
* **Comparação Sintática:** Achei que linguagens como C++, Go e JavaScript facilitaram bastante nesse tipo de código, porque permitem controlar e atualizar mais de uma variável já na própria estrutura do laço,o que deixa tudo mais concentrado em uma linha. Em Python e Rust, a lógica funciona igual, mas a atualização da segunda variável precisa ser feita dentro do bloco, o que acaba deixando o código um pouco mais espalhado.
* **Preferência Pessoal:** Particulamente,gostei mais da versão em Python. Mesmo tendo esse detalhe da variável extra dentro do laço, a escrita é bem simples e fácil de entender, o que para mim faz diferença na hora de ler o código.
