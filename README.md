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

## exemplo de override
```
class Animal {
    void fazerSom() {
        System.out.println("O animal faz um som");
    }
}

class Cachorro extends Animal {
    @Override
    void fazerSom() {
        System.out.println("O cachorro late");
    }
}

class Gato extends Animal {
    @Override
    void fazerSom() {
        System.out.println("O gato mia");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal meuAnimal = new Animal();
        Animal meuCachorro = new Cachorro();
        Animal meuGato = new Gato();

        meuAnimal.fazerSom(); // Chama fazerSom() da classe Animal
        meuCachorro.fazerSom(); // Chama fazerSom() da classe Cachorro
        meuGato.fazerSom(); // Chama fazerSom() da classe Gato
    }
}
```
