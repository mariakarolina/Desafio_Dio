# Desafio_Dio
Este projeto demonstra uma arquitetura simples na AWS utilizando os serviços EC2, EBS, S3 Standard e AWS Lambda.


## Fluxo da Arquitetura

Usuário acessa a aplicação hospedada em uma instância EC2.

A EC2 está conectada a um EBS, que armazena dados de forma persistente.

A aplicação na EC2 envia arquivos para o S3 Standard.

O S3 dispara um evento que aciona a AWS Lambda.

A Lambda pode processar os arquivos (ex: redimensionar imagens, transformar dados ou enviar para outro bucket de arquivamento como Glacier).

## Serviços Utilizados

Amazon EC2 → Hospedagem da aplicação.

Amazon EBS → Armazenamento persistente da instância EC2.

Amazon S3 Standard → Armazenamento de arquivos enviados pela aplicação.

AWS Lambda → Função serverless que processa eventos do S3.
