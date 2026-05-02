# Questão 4: Laço "for" em Multilinguagens

**Enunciado:** Escreva a seguinte construção `for` de Java em 5 Linguagens de Programação diferentes à sua escolha:

```java
int i, j, n = 100;
for (i = 0, j = 17; i < n; i++, j--)
    sum += i * j + 3;
```

**Linguagens escolhidas:**
1. Python
2. C++
3. Rust
4. JavaScript
5. Go

---

## Resoluções

### 1. Python
```python
n = 100
sum = 0
for i in range(n):
    j = 17 - i
    sum += (i * j) + 3
```

### 2. C++
```cpp
int n = 100;
int sum = 0;
for (int i = 0, j = 17; i < n; i++, j--) {
    sum += i * j + 3;
}
```

### 3. Rust
```rust
let n = 100;
let mut sum = 0;
let mut j = 17;

for i in 0..n {
    sum += i * j + 3;
    j -= 1;
}
```

### 4. JavaScript
```javascript
let n = 100;
let sum = 0;
for (let i = 0, j = 17; i < n; i++, j--) {
    sum += i * j + 3;
}
```

### 5. Go
```go
n := 100
sum := 0
for i, j := 0, 17; i < n; i, j = i+1, j-1 {
    sum += i * j + 3
}
```

---

## Discussão: Comparativo de Laços

* **Comparação Sintática:** Achei que linguagens como C++, Go e JavaScript facilitaram bastante nesse tipo de código, porque permitem controlar e atualizar mais de uma variável já na própria estrutura do laço,o que deixa tudo mais concentrado em uma linha. Em Python e Rust, a lógica funciona igual, mas a atualização da segunda variável precisa ser feita dentro do bloco, o que acaba deixando o código um pouco mais espalhado.
* **Preferência Pessoal:** Particulamente,gostei mais da versão em Python. Mesmo tendo esse detalhe da variável extra dentro do laço, a escrita é bem simples e fácil de entender, o que para mim faz diferença na hora de ler o código.
