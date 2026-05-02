# Questão 2: Estrutura de Seleção Múltipla

**Enunciado:** Reescreva o seguinte segmento de código usando uma sentença de seleção múltipla nas seguintes linguagens:

```text
if ((k==1) || (k==2)) j = 2 * k - 1
if ((k==3) || (k==5)) j = 3 * k + 1
if (k==4) j = 4 * k - 1
if ((k==6) || (k==7) || (k==8)) j = k - 2
```

**Linguagens solicitadas:**
a. C
b. Ruby
c. Erlang

Assuma que todas as variáveis são do tipo inteiro. Discuta os méritos relativos do uso dessas linguagens para esse código em particular.

---

## Resoluções

### a. C
```c
switch (k) {
    case 1:
    case 2:
        j = 2 * k - 1;
        break;
    case 3:
    case 5:
        j = 3 * k + 1;
        break;
    case 4:
        j = 4 * k - 1;
        break;
    case 6:
    case 7:
    case 8:
        j = k - 2;
        break;
}
```

### b. Ruby
```ruby
case k
when 1, 2
  j = 2 * k - 1
when 3, 5
  j = 3 * k + 1
when 4
  j = 4 * k - 1
when 6, 7, 8
  j = k - 2
end
```

### c. Erlang
```erlang
J = if
    K == 1 orelse K == 2 -> 2 * K - 1;
    K == 3 orelse K == 5 -> 3 * K + 1;
    K == 4 -> 4 * K - 1;
    K == 6 orelse K == 7 orelse K == 8 -> K - 2
end.
```

---

## Discussão: Méritos Relativos

* **C:** Na minha visão, em C o código acaba ficando mais extenso. O uso constante de break para evitar que um caso “caia” no outro deixa a escrita mais repetitiva e aumenta a chance de esquecer algum.
* **Ruby:** Já em Ruby, achei bem mais prático. A possibilidade de colocar vários valores na mesma condição deixa o código mais limpo e com melhor legibilidade.
* **Erlang:** O Erlang tem uma estrutura interessante, pois cada condição já define o valor direto. O uso de orelse também ajuda a deixar a leitura mais clara.

