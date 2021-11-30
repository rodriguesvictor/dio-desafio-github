# Estruturas

**Namespace**

São usados para organizar classes. Para usar uma classe de outro namespace, colocamos using no começo do código.

> namespace Namespace 1
>
> {
>
> }

**Classe**

Uma classe pode ter campos, propriedades, métodos e eventos dentro dela, que são denominados membros.

> class Pessoa
>
> {
>
> public string Nome { get; set; }
>
> public int Idade { get; set; }
>
> }

Quando uma classe é instanciada, essa instância é chamada de objeto, e nesse objeto podem ser criados os valores de acordo com os campos da classe.

> Pessoa pessoa1 = new Pessoa();
>
> pessoa1.Nome = "Allyson";
>
> pessoa1.Idade = 20;

**Interface**

É como uma classe base que serve de molde para várias classes.

Uma classe que implementa uma interface deve implementar todos os membros.

> interface IPessoa
>
> {
>
> void Nome(string nome);
>
> void Idade(int idade);
>
> }
>
> classe Pessoa : IPessoa
>
> {
>
> public string nome.
>
> public int idade;
>
> void IPessoa.Nome(string nome)
>
> {
>
> this.nome = nome;
>
> }
>
> void IPessoa.Idade(int idade)
>
> {
>
> this.idade = idade;
>
> }
>
> }

**Enum**

Declara um conjunto de constantes nomeadas que começam do 0 e aumentam de 1 em 1.

> enum Estacoes
>
> {
>
> primavera,
>
> verão,
>
> outono,
>
> inverno
>
> }
>
> var estacao = (Estacoes)0; // vai atribuir a variável no índice 0.
>
> Estacoes estacao2 = Estacoes.verão; // vai atribuir a variável a verão;