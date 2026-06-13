# AWS FREE TIER ACCOUNT

Inicie com a conta free tier, alguns serviços serão disponíveis apenas 12 meses

## Principais erro ao usar AWS

❌ Ignorar Alertas de Cobrança
👉 Risco de cobranças acidentais. Sempre configure um orçamento de custos com alertas por e-mail.

❌ Usar Instâncias EC2 ou RDS Grandes
👉 Utilize apenas tipos t2.micro ou outros elegíveis ao Free Tier.

❌ Implantar Usando o Usuário Root
👉 Crie um usuário IAM para as atividades do dia a dia com permissões limitadas.

❌ Esquecer de Parar/Encerrar Recursos
👉 EC2, RDS e até volumes EBS podem gerar cobranças se permanecerem em execução.

❌ Armazenar Arquivos Grandes no S3 sem Limpeza
👉 O Free Tier inclui 5 GB — monitore regularmente o uso do S3.

❌ Não Receber o E-mail de Ativação
👉 Sua conta não estará pronta até que você receba a confirmação da AWS.

❌ Escolher um Plano de Suporte Pago
👉 Selecione Suporte Básico ( Gratuito ) durante o cadastro.

❌ Não Monitorar o Uso
👉 Utilize o Painel de Cobrança ( Billing Dashboard ) para acompanhar o consumo mensal.

## BUDGETS

Sempre adicione orçamento de custos > Para isso pesquise "Billing" no painel da AWS > No painel Billing e costs home > Budgets, selecione:

    - Use a template ( simplified )
    - Coloque o nome do template
    - Coloque os emails das pessoas que irão receber
    - Clique em criar o budget

Ao passar do limite será enviado uma mensagem para o email do custo já atingido

# TIPOS DE USUÁRIOS

`Root User:` Pode criar usuários, apagar arquivos do sistema, instalar serviços e modificar qualquer configuração. Deve inserir um Email na criação.

`IAM User:` usuários criados para uso diário, com permissões específicas e mais seguras. Deve inserir email.

Por padrão, uma conta AWS permite até 5.000 usuários IAM. Esse limite pode ser consultado e, em alguns casos, solicitado para aumento através do Service Quotas.

Para criar um novo usuário: 

    - Acesse IAM resources
    - Na aba esquerda Acess Management > Users > Create user coloque:
        - Coloque um nome
        - Caso o usuário necessite de acesso ao console marque para ele ter permissão ao console da AWS, caso seja uma API não marque essa opção, pois irá ser usado Access Keys (Access Key ID e Secret Access Key) para API's
        - Caso deseja controlar mais específicamente o usuário marque o serviço Identity Center
        - Pode gerar uma senha ou customizar a senha
        - Caso deseje que o usuário mude a senha marque a opção de troca de senha

    - No Painel de Permissões( Set Permissions )