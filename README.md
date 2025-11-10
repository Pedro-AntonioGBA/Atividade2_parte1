# 1. Explique o que é JSON e por que ele se tornou tão popular para troca de dados entre aplicações.
## Json é um objeto de notação utilizado para agrupar e armazenar dados, que pode ser interpretado por diversas linguagens de programação, permitindo se comunicar com diversos sistemas.

# 2. Qual a diferença fundamental entre JSON.stringify() e JSON.parse()? Dê um exemplo prático de quando usar cada um.

## JSON.parse():

### JSON.parse() converte uma string Json eu um objeto Javascript:

```js
var pessoa1 = `{
    "nome": "Pedro",
    "idade": 21, 
    "cidade": "pirpirituba"}`; // => { nome: 'Pedro', idade: 21, cidade: 'pirpirituba' }

console.log(JSON.parse(pessoa1));
```
## JSON.stringify():

### JSON.stringify() converte um objeto Javascript em uma string Json:

```js
var pessoa2 = { "nome": "Maria", "idade": "21", "cidade": "Guarabira" }; // => {"nome":"Maria","idade":"21","cidade":"Guarabira"}

console.log(JSON.stringify(pessoa2));
```

# 3. Considerando a string "JavaScript é baseada em ECMA Script", quais métodos você usaria para:

## 3.1 Verificar se contém a palavra "Script":

### Utlizando a função indexOF():

```js
var string = "JavaScript é baseada em ECMA Script";

console.log(string.indexOf("Script")); // => 4

// Caso a saída seja != -1, significa que a palvra se encontra na string.
```
## 3.2 Remover a palavra "JavaScript" e gerar uma nova string:

### Utlizando a função slice():

```js
var string = "JavaScript é baseada em ECMA Script";

console.log(string.slice(10,35)); // =>  "é baseada em ECMA Script"
```

## 3.3 Substituir "baseada" por "tem origem":

### Utilizando a função replace():

```js
novaString = string.replace("baseada","tem origem");

console.log(novaString); // => "JavaScript é tem origem em ECMA Script"
```

# 4. Qual a vantagem de usar template strings (``) em vez de concatenação com + para criar strings complexas:

### Ao utilizarmos o + em situações em que existem diversas varíaveis que se tornam string, dificulta a leitura e organização do código em relação a formatação com a (``).
