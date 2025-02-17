vamos supor que você tem que provurar um vestido em um guarda roupa com 100 roupas. 

*Na [[Busca simples]]* cabe a você conferir as 100 pecas em busca de achar a roupa escolhida.
*Na Busca Binária* Voce reduz esse número de procura por apenas 7 etapas no máximo.
isso se deve ao uso de Logaritimos.
# Exemplo em Python

```
def Pesquisa_binaria(lista,item):

    baixo=0

    alto=len(lista) -1

    while baixo<=alto:

        meio=(baixo+alto)//2

        chute=lista[meio]

        if chute == item:

            return meio

        if chute > item:

            alto= meio -1

        else:

            baixo= meio+1

    return None

Minha_lista=[1,3,5,7,9]

print (Pesquisa_binaria(Minha_lista,3))

print (Pesquisa_binaria(Minha_lista,-1))
```
Estudar knham acadmy

# Vantagens e desvantagens (Chat)

Exatamente! A busca binária é mais útil para **localizar** um número em uma lista (ou verificar se ele está lá) do que para "fazer algo" diretamente com ele.

Ela é super eficiente quando precisamos encontrar o **índice** de um elemento em uma lista **ordenada**. Esse índice pode ser usado, por exemplo, para acessar ou manipular o valor na lista. Porém, se você só quer saber **se um número existe na lista**, às vezes outros métodos podem ser mais simples.

---

### Quando a Busca Binária é útil:

1. **Listas grandes e ordenadas:**
    
    - Se a lista tiver milhões de números, a busca binária é muito mais rápida do que verificar um por um.
    - Exemplo: Procurar um nome em uma lista telefônica ou um produto em um catálogo digital.
2. **Para retornar o índice do elemento:**
    
    - Se você precisa saber a **posição exata** de um número, a busca binária é ideal.
    - Exemplo: Achar a posição de uma palavra em um dicionário ordenado.
3. **Na base de algoritmos mais complexos:**
    
    - A busca binária é usada em muitos algoritmos, como para resolver problemas de otimização ou encontrar limites em intervalos.

---

### Quando NÃO é tão útil:

1. **Listas pequenas:**
    
    - Para listas pequenas, é mais rápido verificar os números diretamente (busca linear), já que o custo de organizar a lista pode ser maior do que os ganhos.
2. **Listas desordenadas:**
    
    - A busca binária só funciona em listas ordenadas. Se a lista estiver desordenada, primeiro você terá que ordená-la, o que pode ser um trabalho extra.
3. **Se você só quer saber "sim ou não":**
    
    - Por exemplo, para verificar se "3 está na lista", usar `if 3 in lista` pode ser mais intuitivo e direto.

---

### O que torna a Busca Binária "efetiva":

- **Eficiência em grandes listas:** Cada passo reduz a busca pela metade. Se a lista tem 1 milhão de números, você encontra o resultado em no máximo 20 comparações!
- **Fundações em algoritmos importantes:** Ela é a base de sistemas de busca, como [[Banco de dados]], e de outras técnicas avançadas.

Se precisar de ajuda para aplicar isso em algo prático, como um problema do dia a dia ou algo mais simples, posso ajudar a criar exemplos! 😊