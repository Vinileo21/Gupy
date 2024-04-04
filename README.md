# Gupy
Desafio da Gupy

Questao 1: 

package SomaSimples;
public class SomaSimples {

    public static void soma (){
        int indice = 13, soma = 0, k = 0;
        while(k < indice) {
            k++;
            soma+=k;
        }
        System.out.printf("A soma é igual a : %d\n", soma);
    }
}


Questao 2: 

public static boolean isFibonacci(int number) {
        int[] sequence =new int[number];
        if (number == 0 || number == 1){
            return true;
        }
        sequence[0] = 0;
        sequence[1]= 1;
        while (sequence[1] < number) {
            int temp = sequence[0];
            sequence[0] = sequence[1];
            sequence[1] = sequence[1] + temp;
        }
        return sequence[1] == number;
    }
}


Questao 3: 

a) 1, 3, 5, 7, 9

b) 2, 4, 8, 16, 32, 64, 128

c) 0, 1, 4, 9, 16, 25, 36, 49

d) 4, 16, 36, 64, 100

e) 1, 1, 2, 3, 5, 8,13

f) 2,10, 12, 16, 17, 18, 19, 200

Questao 4: 

Na primeira ida:
- Ligo o interruptor  1 por 5 minutos e o desligo, ligo o interruptor 2 e na mesma hora vou até uma das 3 salas
- Se a lampada estiver acessa, pertence ao interruptor 2, se estiver desligada e quente pertence ao interruptor 1, se estiver desligada e fria pertence ao interruptor 3.
Na segunda ida:
- Sabendo já a qual pertence um interruptor, apenas deixo um ligado e outro desligado entre o restantes
- Vou até outra sala e descubro os outros dois.

Questao 5: 

package InverteString;
public class InverteString {

    public static void inverteString(String str) {
        StringBuilder inversa = new StringBuilder();
        for (int i = str.length() - 1; i >= 0; i--) {
            inversa.append(str.toCharArray()[i]);
        }
        System.out.printf("Palavra invertida: %s\n", inversa);
    }
}
