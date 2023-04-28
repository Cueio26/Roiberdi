//atividade 1

int INDICE = 13, SOMA = 0, K = 0;

while (K < INDICE) {
    K = K + 1;
    SOMA = SOMA + K;
}

System.out.println(SOMA);



// atividade 2 

import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Digite um número para verificar se pertence à sequência de Fibonacci: ");
        int num = input.nextInt();
        input.close();

        int[] fib = { 0, 1 };
        
        while (fib[fib.length - 1] < num) {
            int[] newFib = new int[fib.length + 1];
            for (int i = 0; i < fib.length; i++) {
                newFib[i] = fib[i];
            }
            newFib[newFib.length - 1] = fib[fib.length - 1] + fib[fib.length - 2];
            fib = newFib;
        }

 
        if (fib[fib.length - 1] == num) {
            System.out.println(num + " pertence à sequência de Fibonacci");
        } else {
            System.out.println(num + " não pertence à sequência de Fibonacci");
        }
    }
}

// atividade 3

a) 1, 3, 5, 7, 9

b) 2, 4, 8, 16, 32, 64, 128

c) 0, 1, 4, 9, 16, 25, 36, 50

d) 4, 16, 36, 64, 80

e) 1, 1, 2, 3, 5, 8, 13

f) 2,10, 12, 16, 17, 18, 19, 30

// atividade 4
 Usando a fórmula:

tempo = distância / velocidade

Para o carro, temos:

tempo = 100 km / 110 km/h = 0,909 horas

Para o caminhão, temos:

tempo = 100 km / 80 km/h = 1,25 horas

Se o caminhão leva 5 minutos a mais em cada um dos dois pedágios, ele perderá 2/12 de hora no total. Assim, o tempo total que o caminhão leva para percorrer a distância entre as duas cidades é:

tempo = 1,25 horas + 2/12 horas = 1,417 horas

Agora, para determinar qual veículo está mais próximo de Ribeirão Preto quando eles se cruzam na rodovia, é necessário comparar a distância que cada veículo percorreu até o ponto de encontro. Como eles estão se aproximando um do outro, a distância percorrida pelo carro será menor do que a distância percorrida pelo caminhão. Portanto, o carro estará mais próximo de Ribeirão Preto.

Para calcular a distância percorrida por cada veículo, podemos usar a mesma fórmula:

distância = tempo x velocidade

Para o carro, temos:

distância = 0,909 horas x 110 km/h = 100 km

Para o caminhão, temos:

distância = 1,417 horas x 80 km/h = 113 km

Assim, o carro está a uma distância de 100 km de Ribeirão Preto, enquanto o caminhão está a uma distância de 13 km de Ribeirão Preto. Logo, o carro está mais próximo da cidade de Ribeirão Preto quando eles se cruzam na rodovia.

// atidade 5

import java.util.Scanner;

public class InverterString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Digite uma string para ser invertida: ");
        
        String original = sc.nextLine();
        
        String invertida = "";
        
        for (int i = original.length() - 1; i >= 0; i--) {
            invertida += original.charAt(i);
        }

        System.out.println("String invertida: " + invertida);

        sc.close();
    }
}

