# Desafio_POO_TestesUnit-rios
Este projeto tem como objetivo implementar testes unitários para um sistema existente. O sistema consiste em duas classes principais, ValidacoesLista e ValidacoesString, responsáveis por realizar diversas validações envolvendo listas e strings, respectivamente.

## Projeto Console

### Classe `ValidacoesLista`

#### Métodos

- `RemoverNumerosNegativos`: Recebe uma lista de números inteiros e retorna uma nova lista, apenas com os números positivos.
- `ListaContemDeterminadoNumero`: Recebe uma lista de números inteiros e verifica se um determinado número está presente dentro dessa lista.
- `MultiplicarNumerosLista`: Recebe uma lista de números inteiros e retorna uma nova lista, com seus valores multiplicados por um determinado número.
- `RetornarMaiorNumeroLista`: Recebe uma lista de números inteiros e retorna o maior número entre eles.
- `RetornarMenorNumeroLista`: Recebe uma lista de números inteiros e retorna o menor número entre eles.

### Classe `ValidacoesString`

#### Métodos

- `RetornarQuantidadeCaracteres`: Recebe um texto qualquer e retorna a quantidade de caracteres presentes no texto.
- `ContemCaractere`: Recebe um texto qualquer e um texto a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no texto.
- `TextoTerminaCom`: Recebe um texto qualquer e um trecho a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no final do texto apenas.

## Projeto de Testes

### Classe `ValidacoesListaTests`

#### Métodos de Teste

- `DeveRemoverNumerosNegativosDeUmaLista`: Ao passar uma lista com diversos números, incluindo positivos e negativos, deve ser retornado uma nova lista apenas com números positivos.
- `DeveConterONumero9NaLista`: Ao passar uma lista com diversos números, incluindo o número 9, deve retornar verdadeiro, pois encontrou o 9 na lista.
- `NaoDeveConterONumero10NaLista`: Ao passar uma lista com diversos números, mas sem o número 10, deve retornar falso, pois não encontrou o 10 na lista.
- `DeveMultiplicarOsElementosDaListaPor2`: Ao passar uma lista de inteiros, deve retornar uma nova lista, com todos os elementos da lista multiplicados por 2.
- `DeveRetornar9ComoMaiorNumeroDaLista`: Ao passar uma lista de números inteiros, sendo o maior deles 9, deve retornar o 9 como maior elemento dentro dessa lista.
- `DeveRetornarOitoNegativoComoMenorNumeroDaList`: Ao passar uma lista de números inteiros, sendo o menor deles -8, deve retornar o -8 como menor elemento dentro dessa lista.

### Classe `ValidacoesStringTests`

#### Métodos de Teste

- `DeveRetornar6QuantidadeCaracteresDaPalavraMatrix`: Ao passar um texto escrito a palavra "Matrix", deve retornar o número 6, representando 6 caracteres presentes na palavra.
- `DeveContemAPalavraQualquerNoTexto`: Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "qualquer", deve retornar verdadeiro, pois a palavra existe no texto.
- `NaoDeveConterAPalavraTesteNoTexto`: Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "teste", deve retornar falso, pois a palavra não existe no texto.
- `TextoDeveTerminarComAPalavraProcurado`: Ao passar um texto escrito "Começo, meio e fim do texto procurado" e procurar pela palavra "procurado", deve retornar verdadeiro, pois a palavra existe no texto e está inclusa no final do texto.

---

## Como Executar os Testes

1. Clone o repositório 'https://github.com/Hyngras/Desafio_POO_TestesUnit-rios.git' para o seu ambiente local.
2. Abra o projeto no Visual Studio.
3. Execute os testes unitários para cada método de teste nas classes `ValidacoesListaTests` e `ValidacoesStringTests`.
4. Verifique se os resultados dos testes são os esperados.
