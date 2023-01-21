# Terraform Azure Remote Dependency Module

Este é um módulo Terraform que permite criar recursos na nuvem Azure de forma independente e escalável, utilizando dependências remotas para gerenciar a ordem de criação e destruição dos recursos.

## Arquivos incluídos

- main.tf: arquivo principal do módulo, onde são declaradas as dependências remotas e chamadas às outras configurações.
- vm.tf: configurações para criar uma máquina virtual na Azure.
- variables.tf: arquivo para declarar variáveis usadas em todas as configurações.
- outputs.tf: arquivo para declarar saídas disponíveis após a criação dos recursos.
- network.tf: configurações para criar uma rede virtual e regra de firewall na Azure.
- locals.tf: arquivo para declarar variáveis locais usadas em uma ou mais configurações.

## Como usar

1. Copie os arquivos para o diretório do seu projeto Terraform.
2. Defina as variáveis necessárias no arquivo variables.tf.
3. Execute o comando terraform init para baixar as dependências remotas.
4. Execute o comando terraform plan para verificar as alterações que serão feitas na sua conta Azure.
5. Execute o comando terraform apply para criar os recursos na Azure.

## Notas

- Certifique-se de ter uma chave de assinatura válida da Azure configurada antes de executar os comandos Terraform.
- Verifique se as regras de firewall configuradas no arquivo network.tf atendem às suas necessidades de segurança.
- As saídas disponíveis após a criação dos recursos podem ser vistas usando o comando terraform output.
