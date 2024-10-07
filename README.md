Problème rencontré lors de la création d'un serveur MySQL Azure

Commande utilisée :

az mysql server create --resource-group myResourceGroup --name mdbserver --admin-user myadmin --admin-password MyPassword123! --sku-name B_Gen5_2

Erreur reçue :

Azure Database for MySQL - Single Server is scheduled for retirement (https://go.microsoft.com/fwlink/?linkid=2216041) by September 16, 2024. Migrate (https://go.microsoft.com/fwlink/?linkid=2202255) to Azure Database for MySQL- Flexible Server now.
Checking the existence of the resource group 'myResourceGroup'...
Resource group 'myResourceGroup' exists ? : True 
Creating mysql Server 'mdbserver' in group 'myResourceGroup'...
Your server 'mdbserver' is using sku 'B_Gen5_2' (Paid Tier). Please refer to https://aka.ms/mysql-pricing for pricing details
(InvalidElasticServerType) The provided server type value 'Azure Database for MySQL - Single Server' is invalid.
Code: InvalidElasticServerType
Message: The provided server type value 'Azure Database for MySQL - Single Server' is invalid.

Solutions essayées :

Changement de l'SKU : J'ai essayé plusieurs SKU, y compris B_Gen5_1, B_Gen5_2, et d'autres SKU disponibles.
Changement de l'emplacement : J'ai tenté de créer le serveur dans différentes régions (comme westeurope et eastus), mais j'ai rencontré le même problème à chaque fois.
Vérification des limites d'abonnement Azure : J'ai confirmé que mon abonnement n'avait pas atteint ses limites de ressources. 
