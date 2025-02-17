 **Listas**: São coleções dinâmicas de elementos do mesmo tipo, cujo tamanho pode ser alterado dinamicamente durante a execução do programa. As listas oferecem métodos para adicionar, remover e acessar elementos de forma mais flexível.
 
 ![[Pasted image 20250201213537.png]]
 
## Exemplos em python

```
numeros = [10,20,30]
numeros.append(60) => [10,20,30,60]
numeros.remove(30) => [10,20,60]
numeros.reverse()  =>[60,20,10]
numeros.extend(60,90)=> [10,20,60,90]
```

A diferença entre o append e o extend é que o primeiro só passa um numero por vez a lista. Já o extend adiciona mais de um elemento.



## Quando usar listas ou [[Array]]s

**Quando usar listas ou arrays?**

- Use arrays quando o tamanho dos dados é conhecido antecipadamente e não mudará ao longo do tempo.

- Use listas quando precisar de uma estrutura de dados flexível que possa crescer ou diminuir dinamicamente.