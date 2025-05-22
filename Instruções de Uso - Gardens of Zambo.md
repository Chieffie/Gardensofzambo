# Instruções de Uso - Gardens of Zambo

## Arquivos do Projeto

- **index.html**: Arquivo principal do site com a interface e funcionalidades
- **plantas.json**: Arquivo JSON com os links dos artigos do Blogger

## Como Funciona

O site agora permite que os usuários:

1. Selecionem uma região do Brasil
2. Visualizem cards com informações sobre plantas cultiváveis naquela região
3. Cliquem nos cards para acessar os artigos do Blogger correspondentes
4. Vejam a mensagem "Artigo em breve" para plantas que ainda não têm artigo

## Como Publicar o Site

Para publicar o site, você precisa:

1. Fazer upload dos arquivos `index.html` e `plantas.json` para o mesmo diretório no seu servidor web
2. Garantir que ambos os arquivos estejam na mesma pasta

## Como Adicionar Novos Artigos

Quando criar novos artigos no Blogger, você precisa:

1. Abrir o arquivo `plantas.json`
2. Adicionar uma nova entrada no formato:
   ```json
   {
     "nome": "Nome da Planta",
     "link": "URL do artigo no Blogger"
   }
   ```
3. Salvar o arquivo e fazer upload para o servidor

A mensagem "Artigo em breve" desaparecerá automaticamente quando um link for adicionado para aquela planta específica.

## Observações Importantes

- O sistema faz correspondência entre os nomes das plantas no JSON e no HTML, então certifique-se de que os nomes estejam escritos corretamente
- A correspondência é feita ignorando acentos e maiúsculas/minúsculas para maior flexibilidade
- O card inteiro é clicável, não apenas o link
- O design é responsivo e funciona bem em dispositivos móveis e desktop
