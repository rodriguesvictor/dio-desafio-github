# Conceitos

**O que é a POO?**

A POO é um paradigma de programação, ou seja, corresponde a uma técnica de programação para um fim específico.

Dentro desta técnica, existem quatro pilares:

- Abstração
- Encapsulamento
- Herança
- Polimorfismo

O principal conceito da POO são os de classes e objetos.
Classe é um modelo de um objeto, ela encapsula variáveis, funções, estrutura, propriedades e outros componentes.
Podemos dizer que Objeto é uma instância de uma classe.

**O que é um paradigma de Programação?**

Uma linguagem de programação implementa um ou mais paradigmas.
Nada mais é do que um modelo te técnicas, estruturas e formas de solucionar um problema.

Alguns tipos de paradigmas:

- POO
- Programação estruturada
- Programação imperativa
- Programação procedural
- Programação orientada a eventos
- Programação Lógica

**Abstração**

Abstrair um objeto do mundo real para um contexto específico, considerando apenas os atributos importantes.

**Encapsulamento**

Serve para proteger uma classe e definir limites para alteração de suas propriedades.
Serve para ocultar seu comportamento e expor somente o necessário.

[Modificadores de Acesso](https://docs.microsoft.com/pt-br/dotnet/csharp/programming-guide/classes-and-structs/access-modifiers)

**Herança**

Permite reutilizar atributos, métodos e comportamentos de uma classe em outras classes.
Serve para agrupar objetos que são do mesmo tipo, porém com características diferentes.

**Polimorfismo**

Vem do grego e significa"muitas formas".
Podemos assim, sobrescrever métodos das classes filhas para que se comportem de maneira diferente e ter sua própria implementação.

*Polimorfismo em tempo de compilação (Overload/Early Binding)*

> ```c#
> public class Calc
> {
> public int Somar (int n1, int n2)
> 	{
> 	return n1 + n2;
> 	}
>     
> public int Somar (int n1, int n2, int n3)
> 	{
> 	return n1 + n2 + n3;
> 	}
> }
> ```

*Polimorfismo em tempo de execução (Override/Late Binding)*

> ```c#
> public class Pessoa
>     {
>     public string Nome { get; set; }
> 	public int Idade { get; set; }
>     public string Documento { get; set; }
> 
>     public void Apresentar()
>    		{
>         Console.WriteLine($"Olá meu nome é {Nome} e tenho {Idade} anos");
>     	}
> 	}
> 
>     //Aplicando o conceito de Herança, Aluno Herda de Pessoa
>     class Aluno : Pessoa
>     {
>     public int Nota { get; set; }
>     
> 	public void Apresentar()
>    		{
>         Console.WriteLine($"Olá meu nome é {Nome}. Sou um aluno de nota {Nota}.");
>     	}
>      }
> ```

**Classes Abstratas**

Tem como objetivo ser exclusivamente um modelo para ser herdado, portanto não pode ser instanciada.

Você pode implementar métodos ou deixa-los a cargo de quem herdar.

**Classes Seladas**

Uma classe selada tem como objetivo de impedir que outras classes façam uma herança dela, ou seja, nenhuma classe pode ser sua derivada.
Também existem métodos e propriedades seladas.

**Classes Objetos**

A classe **System.Object** é a mãe de todas as classes na hierarquia do .NET
Todas as classes derivam, direta ou indiretamente da classe **Object**,
e ela tem como objetivo prover serviços de baixo nível para suas classes filhas.

**Interfaces**

Uma interface é um contrato que pode ser implementado por uma classe.
É como se fosse uma classe abstrata, podendo definir métodos abstratos para serem implementados.
Assim como uma classe abstrata, uma interface não pode ser instanciada.
Pode se dizer que as **Interfaces** veio trazer o conceito de Herança Múltipla no C#.

## Saber mais

[Linguagens e tipos de paradigmas utilizados por elas](https://en.wikipedia.org/wiki/Comparison_of_mult-paradigm_programming_languages)

[POO C#, Microsoft tutoriais](https://docs.microsoft.com/pt-br/dotnet/csharp/fundamentals/tutorials/oop)

[Classes Seladas](https://dotnettutorials.net/lesson/sealed-class-methods-csharp/)

[Classe Object](https://docs.microsoft.com/pt-br/dotnet/api/system.object)

