# Desafio6
# Questao 1
Contagem regressiva:
1. Escreva um programa que exiba uma contagem regressiva de 100 a -100
utilizando um loop while.
```java
   int numero = 100;
        while (numero >= -100) {
            System.out.println(numero);
            numero--;
        }
    }
}
```
# Questao 2
Soma dos números pares:
2. Escreva um programa que calcule a soma dos números pares de 1 a 20
utilizando um loop while.
```java
 int numero,soma;
       numero = 1;
       soma = 0;
        while (numero <= 20) {
            if (numero % 2 == 0) {
                soma += numero;
            }
            numero++;
        }
        System.out.println("A soma dos números pares de 1 a 20 é: " + soma);
    }
}
```
# Questao 3
Leitura de números até encontrar zero:
3. Escreva um programa que solicite números ao usuário até que ele insira zero e,
em seguida, exiba a soma dos números digitados.
```java
int numero,soma;
       numero = 1;
       soma = 0;
        while (numero <= 20) {
            if (numero % 2 == 0) {
                soma += numero;
            }
            numero++;
        }
        System.out.println("A soma dos números pares de 1 a 20 é: " + soma);
    }
}
```
# Questao 4
Cálculo de fatorial:
4. Escreva um programa que calcule o fatorial de um número fornecido pelo
usuário usando um loop do-while.
```java
 int numero,fatorial, i;
        Scanner ler = new Scanner(System.in);
        fatorial = 1;
        i = 1;
        System.out.println("Digite um numero");
        numero = ler.nextInt();
        if(numero<0){
            System.out.println("Numero invalido");
            return;
        } 
        do{
            fatorial *= i;
            i++;
            
        } while(i<=numero);
         System.out.println("O fatorial de " + numero + " é: " + fatorial);
    }
}
```
# Questao  5
Jogo de adivinhação:
5. Escreva um programa que implemente um jogo de adivinhação onde o usuário
deve adivinhar um número entre 1 e 100, utilizando um loop do-while para
repetir até que o usuário acerte o número. O numero da sorte deverá ser
randomizado pelo computador, pesquise como funciona a biblioteca
Math.random()
```java
int chute, numSorte;
        Scanner ler = new Scanner(System.in);

        numSorte = (int) (Math.random() * 100) + 1;

        System.out.println("Tente acerta um numero de 1 a 100");

        do {
            System.out.println("Digite seu chute");
            chute = ler.nextInt();

            if (chute < numSorte) {
                System.out.println("Tente um número maior.");
            } else if (chute > numSorte) {
                System.out.println("Tente um número menor.");
            } else {
                System.out.println("Parabéns! Você acertou!");
            }

        } while (chute != numSorte);
    }
}
```
# Questao 6

Tabuada de multiplicação:
6. Escreva um programa que exiba a tabuada de multiplicação de um número
fornecido pelo usuário usando um loop for. Você deve informar o numero e de
quanto a quanto você quer fazer a tabuada por exemplo: tabuada do 2 de 1 a
20.
```java
int numero, inicio, fim,i;
        Scanner ler = new Scanner(System.in);

        System.out.println("Digite o numero para ver a tabuada");
        numero = ler.nextInt();

        System.out.println("Numero de inicio da tabuada");
        inicio = ler.nextInt();

        System.out.println("Qual sera o fim da tabuada");
        fim = ler.nextInt();

        System.out.println("Tabuada do " + numero + " de " + inicio + " até " + fim);

        for ( i = inicio; i <= fim; i++) {
            System.out.println(numero + " x " + i + " = " + (numero * i));
        }
    }
}
```
# Questao 7
Soma dos números ímpares:
7. Escreva um programa que calcule a soma dos números ímpares de 1 a 200
utilizando um loop for.
```java
int soma, i;
        soma = 0;

        for (i = 1; i <= 200; i++) {
            if (i % 2 != 0) {
                soma += i;
            }
        }

        System.out.println("A soma dos números ímpares de 1 a 200 é: " + soma);
    }

```
