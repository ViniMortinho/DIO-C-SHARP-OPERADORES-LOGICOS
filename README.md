# Documentação de Operadores Lógicos em C#

Os operadores lógicos em C# são usados para combinar expressões condicionais. Os operadores lógicos mais comuns em C# são:

## Operador AND (&&)

O operador `&&` retorna verdadeiro se ambas as expressões à sua esquerda e à sua direita forem verdadeiras. Caso contrário, retorna falso.

```csharp
bool a = true;
bool b = false;
bool result = a && b; // result será falso
```

## Operador OR (||)

O operador `||` retorna verdadeiro se qualquer uma das expressões à sua esquerda ou à sua direita for verdadeira. Se ambas forem falsas, retorna falso.

```csharp
using ExemplosFundamentos.models;

Console.WriteLine("Digite sua idade");
int idade = int.Parse(Console.ReadLine());

bool ehMaiorDeIdade = true;
ehMaiorDeIdade = (idade >= 18);
bool possuiAutorizacaoDoResponsavel = false;

if (ehMaiorDeIdade || possuiAutorizacaoDoResponsavel)
{
    Console.WriteLine("Entrada Liberada");
}
else{
    Console.WriteLine("Entrada negada");
}
```

## Operador NOT (!)

O operador `!` é usado para inverter o valor booleano de uma expressão.

```csharp
bool a = true;
bool result = !a; // result será falso
```

Para mais informações sobre operadores lógicos em C#, você pode consultar a [documentação oficial da Microsoft](https://docs.microsoft.com/pt-br/dotnet/csharp/language-reference/operators/boolean-logical-operators).