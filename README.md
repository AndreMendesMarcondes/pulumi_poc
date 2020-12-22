# Pulumi


Pulumi é uma infraestrutura de código aberto como ferramenta de código para criar, implantar e gerenciar infraestrutura em nuvem. Pulumi trabalha com infraestrutura tradicional, como VMs, redes e bancos de dados, além de arquiteturas modernas, incluindo contêineres, clusters Kubernetes e funções sem servidor.

Essa POC é um projeto AZURE

## Instalação

Siga o tutorial [instalação](https://www.pulumi.com/docs/get-started/azure/begin/)para instalar o Pulumi.

Para utilizar o Pulumi precisa ter o Azure CLI (command line interface) vinculado à uma conta no Azure.

Para instalar o Azure CLI siga esse [tutorial](https://docs.microsoft.com/pt-br/cli/azure/install-azure-cli)

**Importante** tem que ter uma assinatura **ATIVA** no Azure

## Revisão

Vamos revisar alguns dos arquivos do projeto:

- **Pulumi.yaml** define o projeto.
- **Pulumi.dev.yaml** contém valores de configuração para a pilha que inicializamos.
- **Program.cs** com um ponto de entrada simples.
- **MyStack.cs** é o programa Pulumi que define nossos recursos de pilha. 

## Rodar o projeto

Para rodar o projeto abra o terminal na pasta do mesmo e execute:
```
pulumi up
```

Verifique na sua conta Azure se foi criado uma conta storage com o prefixo pulumi.

Para destruir os resources criados por essa stack execute 

```
pulumi destroy
```

## Comandos

Para verificar todos os comandos disponíveis de automação de infra que o Pulumi dispões para o AZURE, acesso o linl [commandos pulumi](https://www.pulumi.com/docs/reference/pkg/azure/)
