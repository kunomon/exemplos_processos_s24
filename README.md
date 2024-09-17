# Exemplos

## exemplo de overloading
```
class Calculadora {
    // Método para somar dois inteiros
    int somar(int a, int b) {
        return a + b;
    }

    // Método para somar três inteiros
    int somar(int a, int b, int c) {
        return a + b + c;
    }

    // Método para somar dois números de ponto flutuante
    double somar(double a, double b) {
        return a + b;
    }
}

public class Main {
    public static void main(String[] args) {
        Calculadora calc = new Calculadora();
        System.out.println(calc.somar(2, 3)); // Chama somar(int, int)
        System.out.println(calc.somar(2, 3, 4)); // Chama somar(int, int, int)
        System.out.println(calc.somar(2.5, 3.5)); // Chama somar(double, double)
    }
}
```
