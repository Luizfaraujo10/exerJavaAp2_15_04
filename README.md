Algoritmo ArrayCopier:
    array1 <- {7, 4, 8, 1, 4, 1, 4}
    array2 <- new float[array1.length]
    para i = 0 até (array1.length - 1) passo 1 faça:
        Imprima array1[i]

    count <- 0
    enquanto count < array1.length e array1[count] != 1 faça:
        array2[count] <- (float) array1[count]
        Imprima array2[count]
        count <- count + 1

        É uma lista arranjo, pois o código aborda coleções com um número finito de elementos com ordem linear e elas possuem índices. Exemplo: O índice 0 acessa o primeiro elemento da coleção.
