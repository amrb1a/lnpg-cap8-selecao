# Questão 1: Substituição de `goto` por Laços

**Enunciado:** Reescreva o seguinte segmento de pseudocódigo usando uma estrutura de laço nas linguagens especificadas:

```text
k = (j + 13) / 27
loop:
if k > 10 then goto out
k = k + 1
i = 3 * k - 1
goto loop
out:
```

**Linguagens solicitadas:**
a. Java
b. Python
c. Haskell
d. Swift

Assuma que todas as variáveis sejam do tipo inteiro. Discuta qual linguagem, para esse código, tem a melhor facilidade de escrita, a melhor legibilidade e a melhor combinação de ambas.

---

## Resoluções
### a. Java
```java
int k = (j + 13) / 27;
int i = 0; 
while (k <= 10) {
    k++;
    i = 3 * k - 1;
}
```

### b. Python
```python
k = (j + 13) // 27
while k <= 10:
    k += 1
    i = 3 * k - 1
```

### c. Haskell
```haskell
let k_init = (j + 13) `div` 27

loop k i
  | k > 10    = (k, i)
  | otherwise =
      let k' = k + 1
      in loop k' (3 * k' - 1)

-- chamada:
loop k_init 0
```

### d. Swift
```swift
var k = (j + 13) / 27
var i = 0
while k <= 10 {
    k += 1
    i = 3 * k - 1
}
```

---

## Discussão: Escrita e Legibilidade

* **Simplicidade de escrita:** Na minha opinião, Python é a linguagem com maior facilidade de escrita nesse exemplo, porque o código fica mais curto e direto, sem precisar de muitos símbolos extras. A estrutura do while também é bem clara e fácil de entender.
* **Legibilidade:** Java foi a que achei mais fácil de ler. O uso de chaves para delimitar os blocos deixa bem claro onde cada parte do código começa e termina, o que transmite maior organização na estrutura.
* **Melhor equilíbrio:** Swift, na minha visão, é a que melhor equilibra os dois pontos. Ela mantém uma escrita simples, parecida com Python, mas ao mesmo tempo traz uma estrutura mais organizada, semelhante à do Java.

