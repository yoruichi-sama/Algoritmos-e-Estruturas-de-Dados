# Insertion Sort Código

``` java
/**
 * Ordenacao por Insercao 
 */
public void insertionSort(){

    for (int i = 1 ; i < n ; i++) {

        Personagem tmp = lista[i];
        int j = i - 1;
        
        while ((j >= 0) && (lista[j].getAnoNascimento().compareTo(tmp.getAnoNascimento()) > 0)){

            lista[j+1] = lista[j];
            j--;
        }

        lista[j+1] = tmp;
    }

}
```

## Complexidade

- Melhor caso: `T(n) = n` 
- Pior caso: `T(n) = n^2`
- Caso médio: `T(n) = n^2` 

_O algoritmo de ordenação Insertion Sort é O(n^2)_