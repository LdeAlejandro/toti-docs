


# Formulário de Cadastro com Tabela de Cidades

Este é um exemplo de um formulário de cadastro simples em HTML, incluindo uma tabela de cidades e estados.

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

    <!-- Campo de Nome -->
    Nome: <br><input type="text" name="name" maxlength="50" /><br>

    <!-- Campo de Telefone -->
    Telefone: <br><input type="tel" name="phone"/><br>

    <!-- Campo de Data de Nascimento -->
    Data de nascimento: <br><input type="date" name="birthdate"/><br>

    <!-- Campo de Doenças de Família -->
    Doenças de família: <br>
    <textarea name="doencasdefamilia"></textarea><br>
    <br>

    <!-- Caixa de Seleção (Checkbox) -->
    Fuma: <input type="checkbox" value="fuma" name="smoker"/><br>
    Bebe: <input type="checkbox" value="bebe" name="drinker"/><br>
    <br>

    <!-- Botões de Opção (Radiobutton) -->
    Sexo: <br>
    <input type="radio" value="femenino" name="sexo"/>feminino<br>
    <input type="radio" value="masculino" name="sexo"/>masculino<br>
    <br>

    <!-- Botões -->
    <input type="reset" value="clean" name="reset"/>
    <input type="submit" value="Enviar" name="submitform"/><br>

</form>

<br><br>

<!-- Tabela de Cidades e Estados -->
<table border="1">
    <tr><th>Estado</th><th>Cidade</th></tr>
    <tr><td>Pernambuco</td><td>Recife</td></tr>
    <tr><td>Paraíba</td><td>Santa Rita</td></tr>
</table>

</body>
</html>
```

## Explicação Detalhada das Tags e Atributos

### `<!DOCTYPE html>`
Define o tipo de documento como HTML5, garantindo que o navegador interprete corretamente o código HTML que se segue.

### `<html>`
Marca o início e o fim do documento HTML, encapsulando todo o conteúdo visível para o usuário.

### `<head>`
Contém metadados do documento, como informações sobre a codificação de caracteres e o título da página.

- `<meta charset="utf-8"/>`: Define o conjunto de caracteres como UTF-8, permitindo o uso de caracteres especiais e internacionais.
- `<title>Site = Toters WebSite</title>`: Define o título da página exibido na aba do navegador.

### `<body>`
Contém o conteúdo visível da página, como texto, imagens, formulários e tabelas.

#### Cabeçalho (`<h1>`)
- `<h1>Formulário de Cadastro</h1>`: Título principal da página.

#### Formulário (`<form>`)

`<form action="processa.php">`
Define um formulário que, quando enviado, envia os dados para o arquivo `processa.php` para processamento no servidor.

#### Campos de Entrada (`<input>`, `<textarea>`)

- `<input type="text" name="name" maxlength="50" />`: Campo de texto para inserir o nome do usuário, limitado a 50 caracteres.
- `<input type="tel" name="phone"/>`: Campo para inserir o número de telefone.
- `<input type="date" name="birthdate"/>`: Campo para inserir a data de nascimento.
- `<textarea name="doencasdefamilia"></textarea>`: Área de texto para inserir informações sobre doenças familiares.

#### Caixas de Seleção (`<input type="checkbox">`)

- `<input type="checkbox" value="fuma" name="smoker"/>`: Caixa de seleção para indicar se o usuário é fumante.
- `<input type="checkbox" value="bebe" name="drinker"/>`: Caixa de seleção para indicar se o usuário é bebedor.

#### Botões de Opção (`<input type="radio">`)

- `<input type="radio" value="femenino" name="sexo"/>`: Botão de rádio para selecionar o sexo feminino.
- `<input type="radio" value="masculino" name="sexo"/>`: Botão de rádio para selecionar o sexo masculino.

#### Botões (`<input type="reset">`, `<input type="submit">`)

- `<input type="reset" value="clean" name="reset"/>`: Botão para limpar todos os campos do formulário.
- `<input type="submit" value="Enviar" name="submitform"/>`: Botão para enviar os dados preenchidos no formulário para processamento.

#### Tabela (`<table>`)

- `<table border="1">`: Cria uma tabela com bordas de espessura 1.
- `<tr>`: Define uma linha na tabela.
- `<th>`: Define uma célula de cabeçalho em uma tabela.
- `<td>`: Define uma célula de dados em uma tabela.

##### Cabeçalho da Tabela
- `<tr><th>Estado</th><th>Cidade</th></tr>`: Cria a linha de cabeçalho da tabela com duas colunas: "Estado" e "Cidade".

##### Linhas da Tabela
- `<tr><td>Pernambuco</td><td>Recife</td></tr>`: Cria uma linha na tabela com os dados "Pernambuco" e "Recife".
- `<tr><td>Paraíba</td><td>Santa Rita</td></tr>`: Cria uma linha na tabela com os dados "Paraíba" e "Santa Rita".

### Resumo

Este código HTML cria uma página da web com um formulário de cadastro e uma tabela. O formulário permite aos usuários inserir informações como nome, telefone, data de nascimento, histórico de doenças familiares, hábitos de fumar e beber, e selecionar seu sexo. Além disso, a página inclui uma tabela que lista estados e suas respectivas cidades.
