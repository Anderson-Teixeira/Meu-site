<html>
<body>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
            window.addEventListener("onEmbeddedMessagingReady", e => {
            // Envio de dados para o Salesforce
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"IdContato" : "003Dy00000vmv09IAA"});
            // Exemplo de como preencher mais de uma variável
            // ({"IdContato" : "8675309", "Order_Number" : "11098324"});
        });
        
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DDy0000008qC3',
				'TesteGitPagesQA',
				'https://sieg--qa.sandbox.my.site.com/ESWTesteGitPagesQA1718299314061',
				{
					scrt2URL: 'https://sieg--qa.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://sieg--qa.sandbox.my.site.com/ESWTesteGitPagesQA1718299314061/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</body>
</html>
