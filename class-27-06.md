


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
- 

### Explicação dos Tipos de Entrada (`type`)

1. **`type="text"`**: 
   - **Descrição**: Cria um campo de texto simples onde os usuários podem inserir texto livre.
   - **Exemplo**: `<input type="text" name="name" maxlength="50" />`

2. **`type="tel"`**:
   - **Descrição**: Campo de entrada otimizado para números de telefone.
   - **Exemplo**: `<input type="tel" name="phone"/>`

3. **`type="date"`**:
   - **Descrição**: Permite aos usuários selecionar uma data de um calendário interativo.
   - **Exemplo**: `<input type="date" name="birthdate"/>`

4. **`<textarea>`**:
   - **Descrição**: Cria uma área de texto multi-linha onde os usuários podem inserir texto extenso.
   - **Exemplo**: `<textarea name="doencasdefamilia"></textarea>`

5. **`type="checkbox"`**:
   - **Descrição**: Cria uma caixa de seleção que pode ser marcada ou desmarcada independentemente de outras caixas de seleção.
   - **Exemplo**: 
     ```html
     Fuma: <input type="checkbox" value="fuma" name="smoker"/><br>
     Bebe: <input type="checkbox" value="bebe" name="drinker"/><br>
     ```

6. **`type="radio"`**:
   - **Descrição**: Cria um botão de opção que permite aos usuários selecionar uma opção de um conjunto de opções mutuamente exclusivas.
   - **Atributos**: Deve ter o atributo `name` com o mesmo valor para todos os botões de rádio que pertencem ao mesmo grupo.
   - **Exemplo**: 
     ```html
     Sexo: <br>
     <input type="radio" value="femenino" name="sexo"/>feminino<br>
     <input type="radio" value="masculino" name="sexo"/>masculino<br>
     ```

7. **`type="reset"`**:
   - **Descrição**: Cria um botão que limpa os campos do formulário, restaurando os valores padrão.
   - **Exemplo**: `<input type="reset" value="Limpar" name="reset"/>`

8. **`type="submit"`**:
   - **Descrição**: Cria um botão que envia os dados do formulário para o servidor para processamento.
   - **Exemplo**: `<input type="submit" value="Enviar" name="submitform"/>`


Cada tipo de entrada (`type`) no código HTML serve a um propósito específico no formulário de cadastro:

- **Campos de Entrada**: `text`, `tel`, `date`
- **Área de Texto**: `textarea`
- **Caixas de Seleção**: `checkbox`
- **Botões de Opção**: `radio`
- **Botões**: `reset`, `submit`

Esses elementos formam a estrutura básica para coletar informações do usuário de forma interativa em um site ou aplicação web.

### Resumo

Este código HTML cria uma página da web com um formulário de cadastro e uma tabela. O formulário permite aos usuários inserir informações como nome, telefone, data de nascimento, histórico de doenças familiares, hábitos de fumar e beber, e selecionar seu sexo. Além disso, a página inclui uma tabela que lista estados e suas respectivas cidades.
