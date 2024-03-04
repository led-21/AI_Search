# Azure AI Search
O Azure AI Search é uma plataforma de recuperação de informações alimentada por IA que auxilia os desenvolvedores a criar experiências de pesquisa avançadas e aplicativos de IA generativos. Essa plataforma combina grandes modelos de linguagem com dados empresariais para oferecer funcionalidades de busca ricas e eficientes.

## Passo a passo atividades do laboratório
- Criar um recurso *Azure AI Search*;
- Criar um recurso *Azure AI services resource*;
- Criar uma *storage account*, alterar a configuração para permitir *Blob Anonymous Access*;
- Baixas e descompactar os arquivos no link: https://aka.ms/mslearn-coffee-reviews;
- Criar um *Container* no *storage account* e carregar os arquivos baixados anteriormente (Upload blob);
- No portal do Azure no recurso *Azure AI Search* na página do Overview, selecione Import data e configure conforme o tutorial link: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html;
- Criar um indexador;
- Consultar o índice;

## Resultado

Editor de consultas JSON

`
{
 "search": "sentiment:'positive'",
 "count": true
}
`

Resuldatos

`
  ...
  "@odata.count": 7, 
  "value": [
    {
      "@search.score": 0.47000363,
  ...
`



`
  ... "sentiment": "[\"positive\"]",
      "merged_content": "\n\nReview: The coffee tastings every Wednesday afternoon are so fun. Each month there is a new drink theme. You do need to book a spot in advance to attend. It is very worth it! I also love their local music. Fourth Coffee brings in rising artists every weekend. I like to head over there mid-afternoon on weekdays when it’s not too busy and get a slice of pie or their seasonal baked goods.  \nDate: August 13, 2018\nLocation: Chicago, Illinois  \n\nimage1.png\n ierican Coffee 114 10148/0034 \n\n\nimage2.png\n  \n\n\n",
      "text": [
        "ierican Coffee 114 10148/0034",
        ""
      ], ...
`
