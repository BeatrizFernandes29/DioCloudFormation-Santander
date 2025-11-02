# DioCloudFormation-Santander
Desafio implementando minha primeira stack- DIO

O AWS CloudFormation é um serviço da Amazon que permite criar e gerenciar recursos na nuvem automaticamente, usando um arquivo template (em formato YAML ou JSON).

Em vez de criar buckets, bancos de dados ou máquinas virtuais, você escreve um template e o CloudFormation constrói tudo para você automaticamente.

Esse conceito é conhecido como IaC — Infrastructure as Code (Infraestrutura como Código).

Isso traz padronização, automação e reprodutibilidade.

Exemplo de Stack (template.yaml)

Abaixo está um exemplo simples de template que cria um bucket S3 com versionamento habilitado:

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: "Minha primeira Stack AWS - Criação de um bucket S3"

Resources:
  MeuBucketS3:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: meu-primeiro-bucket-dio
      VersioningConfiguration:
        Status: Enabled

O passo a passo seria:

Acesse o Console AWS. Vá em CloudFormation → Create Stack → With new resources (standard). Faça upload do arquivo template.yaml. Dê um nome à Stack, como PrimeiraStackDIO. Clique em Create Stack e aguarde a criação do recurso.

Durante este desafio, aprend o conceito de Infraestrutura como Código (IaC); que o CloudFormation cria recursos automaticamente a partir de templates; que é possível automatizar e reproduzir ambientes facilmente.
E quoe dcumentar o aprendizado é essencial para o crescimento profissional.
