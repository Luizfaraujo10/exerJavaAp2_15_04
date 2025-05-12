Observação: Visualize este arquivo no modo "Code" do Git Hub.

ALUNOS:
Caio Felix de Moura | RA: 2401161
Vinicuius Sousa Santos | RA: 2401090
Luiz Felipe Araujo dos SAntos | RA: 2400228
Thiago Malta da Silva | RA: 2400048
Gabriel Vicente Aiala | RA: 2100253
Diego Fonseca de Oliveira | RA: 1902388

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

        --------------------------------------------------------------

    CODIGO REFORMULADO.

    
        public class ArrayCopier {
    public static void main(String[] args) {
        int[] array1 = {7, 4, 8, 1, 4, 1, 4};
        float[] array2 = new float[array1.length];
        System.out.println(array2.length);
        int count = 0;
        System.out.print("array1: [ ");
        while (count < array1.length + array2.length) {
            if (count < array1.length) {
                System.out.print(array1[count] + " ");
                count++;
            } else {
                if (count == array1.length) {
                    System.out.println(" ]");
                    System.out.print("array2: [ ");
                }
                int count2 = count - array1.length;
                if (array1[count2] == 1) {
                    break;
                }
                array2[count2] = (float) array1[count2];
                System.out.print(array2[count2] + " ");
                count++;
            }
        }
        System.out.println(" ]");
    }
}
/*
Algoritmo ArrayCopier:
    array1 <- {7, 4, 8, 1, 4, 1, 4}
    array2 <- new float[array1.length]
    count <- 0
    enquanto count < array1.length + array2.length faça:
        if count < array1.length:
            Imprima array1[count]
            count <- count + 1
        else:
            count2 <- count - array1.length
            if array1[count2] == 1:
                break
            array2[count2] <- (float) array1[count2]
            Imprima array2[count2]
            count <- count + 1


