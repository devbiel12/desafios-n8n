Atue como um especialista em N8N.

Crie uma automação para automatizar envio de notificações de chamado no celular e e-mail.

Público:
Equipe de Infra Coorporativa

Ferramentas envolvidas:
Whatsapp, SAP Interno, E-mail

Fluxo:
1. Webhook que recebe os dados de ocorrências que forem abertas para TI INFRA
2. Valida se aquele chamado está como situação "ABERTO"
3. Envia e-mail e Whatsapp no grupo para dizer que chegou um novo chamado, junto com o link da Ocorrência.

Regras:
- Não pode utilizar chamados já criados como parâmetros para falar que um novo chamado foi criado
- Integração deve ser enviado no e-mail de infraestrutura
- Ignorar registros sem e-mail válido

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
Devem ser usados os seguintes nodes:
- 1: WebHook para validar a entrada de dados do SAP
- 2: EditField para pegar o estado do chamado, quem criou ele, SLA e descrição do chamado.
- 3: IF para validar se aquele chamado consta como "ABERTO" ou se houve somente uma modificação no chamado
- 4: Caso esteja "Aberto", colocar um "Send an Email" enviar para e-mail de infraestrutura e no grupo de Whatsapp com os profissionais da área.
- 4: Adicionar um http request para pegar os dados do Uzapi e enviar a mensagem de acordo com as informações do EditField.