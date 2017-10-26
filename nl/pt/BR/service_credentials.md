---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-01"

---

{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# Incluindo uma nova credencial de serviço
{: #service_credentials}

É possível gerar um novo conjunto de credenciais de serviço para casos em que se queira conectar manualmente um consumidor externo a um serviço do Bluemix. Por exemplo, se você estiver tentando ligar um app AWS a um serviço do Watson, será necessário gerar uma nova credencial de serviço que possa ser usada para ligar esses dois serviços.

Os serviços do Cloud Foundry podem gerar uma chave de serviço, também conhecida como uma credencial de serviço. As credenciais de serviço são específicas do serviço e variam com base em como cada serviço define as credenciais que precisam ser geradas. Uma credencial de serviço pode conter um nome de usuário, uma senha, um nome de host, uma porta e uma URL. No entanto, o conteúdo de cada credencial de serviço é exclusivo para o serviço que a gera. Alguns serviços podem gerar dados adicionais que requerem que parâmetros sejam passados. Por exemplo, um serviço pode requerer que você insira um parâmetro de idioma para configurar o idioma padrão retornado na chave de serviço que é gerada. 

Conclua as etapas a seguir para incluir uma nova credencial de serviço:

1. Na página de detalhes de serviço, selecione a guia Credenciais de serviço e clique em **Nova credencial + **.
2. No diálogo Incluir nova credencial, forneça um **Nome**.
3. Opcionalmente, é possível fornecer parâmetros adicionais como um objeto JSON válido contendo parâmetros de configuração específicos do serviço, fornecidos sequencialmente ou em um arquivo.

  **Nota**. A maioria dos serviços não requer parâmetros adicionais e para serviços que o requerem, cada serviço define sua própria lista exclusiva de parâmetros. Para obter uma lista de parâmetros de configuração suportados, veja a documentação para a oferta de serviços específica.
4. Clique em **Incluir** para gerar a nova credencial de serviço.
