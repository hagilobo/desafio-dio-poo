# 📚 Desafio de Orientação a Objetos em Java (DIO - Bootcamp)

Este projeto implementa a abstração de um sistema de gerenciamento de Bootcamp, aplicando os quatro pilares da Programação Orientada a Objetos (POO): Abstração, Herança, Encapsulamento e Polimorfismo.

## 🎯 Pilares da POO Aplicados

- **Abstração e Herança:** A classe `Conteudo` é abstrata (definindo o contrato `calcularXp()`), e é herdada pelas classes concretas `Curso` e `Mentoria`.
- **Polimorfismo:** O método `calcularXp()` é implementado de forma diferente em `Curso` (baseado em carga horária) e `Mentoria` (com XP adicional fixo de 20).
- **Encapsulamento:** Todos os dados internos (`nome`, `cargaHoraria`, coleções) são protegidos com `private` e acessados via métodos `public` (getters/setters).

## 💻 Simulação de Execução

Abaixo, a saída do console da classe `Main` demonstra a simulação de inscrição, progressão e o cálculo de XP total para dois Devs:

```java
// Simulação Dev Hagi (Progrediu 2x: Concluiu Curso Java e Curso JS)
Conteúdos Inscritos Hagi:[Mentoria{titulo='mentoria de java', descricao='descrição mentoria java', data=2025-11-27}]
Conteúdos Concluídos Hagi:[Curso{titulo='curso java', descricao='descrição curso java', cargaHoraria=8}, Curso{titulo='curso js', descricao='descrição curso js', cargaHoraria=4}]
XP:120.0
-------
// Simulação Dev João (Progrediu 3x: Concluiu Curso Java, Curso JS e Mentoria)
Conteúdos Inscritos João:[]
Conteúdos Concluídos João:[Curso{titulo='curso java', descricao='descrição curso java', cargaHoraria=8}, Curso{titulo='curso js', descricao='descrição curso js', cargaHoraria=4}, Mentoria{titulo='mentoria de java', descricao='descrição mentoria java', data=2025-11-27}]
XP:150.0
Process finished with exit code 0
