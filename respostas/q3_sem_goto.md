# Questão 3: Remoção de gotos e breaks

**Enunciado:** Considere o seguinte segmento de programa em C. Reescreva-o sem usar gotos ou breaks em 3 linguagens diferentes à sua escolha.

```c
j = -3;
for (i = 0; i < 3; i++) {
    switch (j + 2) {
        case 3:
        case 2: j--; break;
        case 0: j += 2; break;
        default: j = 0;
    }
    if (j > 0) break;
    j = 3 - i;
}
```

**Linguagens escolhidas:**
1. Python
2. Java
3. JavaScript

---

## Resoluções

### 1. Python
```python
j = -3
continuar = True
i = 0

while i < 3 and continuar:
    val = j + 2
    if val == 3 or val == 2:
        j -= 1
    elif val == 0:
        j += 2
    else:
        j = 0
        
    if j > 0:
        continuar = False
    else:
        j = 3 - i
    i += 1
```

### 2. Java
```java
int j = -3;
boolean continuar = true;

for (int i = 0; i < 3 && continuar; i++) {
    int val = j + 2;
    if (val == 3 || val == 2) {
        j--;
    } else if (val == 0) {
        j += 2;
    } else {
        j = 0;
    }
    
    if (j > 0) {
        continuar = false;
    } else {
        j = 3 - i;
    }
}
```

### 3. JavaScript
```javascript
let j = -3;
let continuar = true;

for (let i = 0; i < 3 && continuar; i++) {
    let val = j + 2;
    if (val === 3 || val === 2) {
        j--;
    } else if (val === 0) {
        j += 2;
    } else {
        j = 0;
    }
    
    if (j > 0) {
        continuar = false;
    } else {
        j = 3 - i;
    }
}
```

---

## Discussão: Estrutura e Lógica

* **Legibilidade:** Senti que a legibilidade ficou um pouco prejudicada nesse caso. Antes, com o break, era mais fácil entender onde o fluxo do código parava,mas agora sem ele é preciso analisar toda a sequência de condições para perceber quando o laço termina, o que deixa a leitura um pouco menos direta.
* **Impacto no Código:** Na minha opinião, o código acabou ficando maior em todas as linguagens. Ao retirar o switch/case e também o uso de break, foi necessário usar vários if/else e ainda uma variável extra (continuar) para controlar o fim do laço, o que deixou a implementação mais extensa.
