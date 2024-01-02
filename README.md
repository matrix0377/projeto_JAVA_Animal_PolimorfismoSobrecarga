# projeto_JAVA_Animal_PolimorfismoSobrecarga

Repositório para projetos Java implementação de POO pilar Polimorfismo Sobrecarga

Conceitos aplicados:

- Algorítmo
- Pilar Encapsulamento
- Pilar Herança
- Pilar Polimorfismo
  - Polimorfismo Sobreposição
  - Polimorfismo Sobrecarga



Algorítmo

Polimorfismo Sobreposição

    classe abstrata Animal
        protegido peso: Real
        protegido idade: Inteiro
        protegido membros: Inteiro
        
        publico metodo abstrato emitirsom()
        fimMetodo
    FimClasse
    
    classe Mamifero estende Animal
        protegido corPelo: Caractere
        @Sobrepor
        publico metodo emitirSom()
            Escreva("Som de Mamífero")
        fimMetodo
    FimClasse
    
    classe Lobo estende Mamifero
        @Sobrepor
        publico metodo emitirsom()
            Escreva("Auuuuuu!")
        fimMetodo
    Fimclasse
    
    classe Cachorro estende Lobo
        @Sobrepor
        publico metodo emitirSom()
            Escreva("au! Au! Au!")
        fimMetodo
    FimClasse

    // Mesma Assinatura. Classes Diferentes É SOBREPOSIÇÃO!


Polimorfismo Sobrecarga

    classe Cachorro estende Lobo
        publico metodo reagir(frase: Caractere)
            se(frase="toma comida" ou frase="Olá")
                escreva("Abanar e Latir")
            senao
                escreva("Rosnar")
            fimSe
        fimMetodo
    
        publico metodo reagir(hora, min: Inteiro)
            se(ora<12)
                escreva("Abanar")
            senaoSE (hora>=18)
                escreva("Ignorar")
            senao
                escreva("Abanar e Latir")
            fimSe
        fimMetodo
    
        publico metodo reagir(dono: Logico)
            se (dono = verdadeiro)
                escreva("Abanar")
            senao
                escreva("Rosnar e Latir")
            fimSe
        fimMetodo
        
        publico metodo reagir(idade: Inteiro, , peso: Real)
            se(idade<5)
                se(peso<10)
                    escreva("Abanar")
                senao
                    escreva("Latir")
                fimSe
            senao
                se(peso<10)
                    escreva("Rosnar")
                senao
                    esreva("Ignorar")
                fimSe
            fimSe
        fimMetodo
    FimClasse
    
    // Assinaturas diferentes. Mesma classe É SOBRECARGA!

