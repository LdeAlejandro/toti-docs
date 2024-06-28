
Código da classe


# Formulário de Cadastro

Este é um exemplo de um formulário de cadastro simples em HTML.

## Estrutura do Documento HTML

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8"/>
    <title>Site = Toters WebSite</title>
</head>
<body>

<h1>Formulário de Cadastro</h1>

<form action="processa.php">

    Nome: <br><input type="text" name="name" maxlength="50" /><br>
    Telefone: <br><input type="tel" name="phone"/><br>
    Data de nascimento: <br><input type="date" name="birthdate"/><br>
    Doenças de família: <br>
    <textarea name="doencasdefamilia"></textarea><br>
    <br>
    Fuma: <input type="checkbox" value="fuma" name="smoker"/><br>
    Bebe: <input type="checkbox" value="bebe" name="drinker"/><br>
    <br>
    Sexo: <br>
    <input type="radio" value="femenino" name="sexo"/>feminino<br>
    <input type="radio" value="masculino" name="sexo"/>masculino<br>
    <br>
    <input type="reset" value="Limpar" name="reset"/>
    <input type="submit" value="Enviar" name="submitform"/><br>

</form>

</body>
</html>
```

## Explicação das Tags e Atributos

- `<!DOCTYPE html>`: Define o tipo de documento como HTML5.
- `<html>`: Marca o início e o fim do documento HTML.
- `<head>`: Contém metadados do documento.
  - `<meta charset="utf-8"/>`: Define o conjunto de caracteres como UTF-8.
  - `<title>Site = Toters WebSite</title>`: Define o título da página.
- `<body>`: Contém o conteúdo visível da página.
  - `<h1>Formulário de Cadastro</h1>`: Título principal da página.
  - `<form action="processa.php">`: Formulário que envia dados para `processa.php`.
    - `<input type="text" name="name" maxlength="50" />`: Campo de texto para nome.
    - `<input type="tel" name="phone"/>`: Campo de telefone.
    - `<input type="date" name="birthdate"/>`: Campo de data de nascimento.
    - `<textarea name="doencasdefamilia"></textarea>`: Área de texto para doenças familiares.
    - `<input type="checkbox" value="fuma" name="smoker"/>`: Caixa de seleção para fumante.
    - `<input type="checkbox" value="bebe" name="drinker"/>`: Caixa de seleção para bebedor.
    - `<input type="radio" value="femenino" name="sexo"/>`: Botão de rádio para sexo feminino.
    - `<input type="radio" value="masculino" name="sexo"/>`: Botão de rádio para sexo masculino.
    - `<input type="reset" value="Limpar" name="reset"/>`: Botão para limpar o formulário.
    - `<input type="submit" value="Enviar" name="submitform"/>`: Botão para enviar o formulário.

Este formulário é utilizado para coletar informações básicas de cadastro, como nome, telefone, data de nascimento, informações sobre doenças familiares, hábitos de fumar e beber, e seleção de sexo.
