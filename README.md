# Microservice de envio de email

Bem-vindo ao Microservice de Envio de Email! Este microservice desenvolvido em Spring Boot oferece uma solução confiável e eficiente para enviar emails, combinando o poder do RabbitMQ como serviço de mensageria e o Log4j2 como serviço de logging.

Com este microservice, você pode enviar emails de forma descomplicada e escalável, integrando-se facilmente aos principais provedores de email, como o Gmail, por meio do protocolo SMTP. A abordagem simplificada permite que você se comunique com seus usuários, clientes ou fornecedores sem dificuldades.

O RabbitMQ garante a entrega assíncrona e confiável de mensagens, tornando o envio de emails mais robusto e resiliente, mesmo em situações de alto volume. Enquanto isso, o Log4j2 fornece um sistema de logging abrangente, permitindo que você acompanhe as atividades do microservice e solucione problemas de forma eficaz.

Antes de começar a usar o microservice, verifique se você tem os seguintes pré-requisitos instalados em seu ambiente de desenvolvimento:

- Java 8 ou superior: Linguagem de programação utilizada pelo microservice.
- Maven: Ferramenta de automação de compilação e gerenciamento de dependências.
- RabbitMQ: Serviço de mensageria para garantir a entrega assíncrona e confiável de mensagens.
- Log4j2: Biblioteca de logging para registrar e monitorar eventos no microservice.

Siga as instruções fornecidas para configurar e executar o microservice, e aproveite a facilidade de envio de emails com a confiabilidade do RabbitMQ e o registro detalhado das atividades com o Log4j2. Esteja preparado para levar a comunicação por email a um novo patamar com este poderoso microservice.

## Configuração
1. Clone este repositório em sua máquina local:
```
git clone https://github.com/seu-usuario/ms-email.git
```
2. Abra o arquivo application.properties e ajuste as configurações conforme necessário, incluindo as configurações do Gmail, do RabbitMQ e do Log4j2.

## Executando o Microservice
1. Abra um terminal e navegue até o diretório raiz do projeto.
2. Execute o seguinte comando para construir o projeto:
```
-- mvn clean install
```
3. Em seguida, execute o seguinte comando para iniciar o microservice:
```
-- mvn spring-boot:run
```
O microservice será iniciado e estará pronto para receber solicitações de envio de emails.

## Utilizando o Microservice
Você pode enviar solicitações de envio de emails para o microservice através de uma API REST. A seguinte rota é exposta:
```
{POST} http://localhost:8081/sending-email
```
O corpo da solicitação deve conter as informações necessárias para enviar o email, como o destinatário, o remetente, o assunto e o corpo do email.

## Spring Logging com Log4j2
O Log4j2 já está configurado no microservice para registrar informações de log. Os logs são gravados em um arquivo de log no diretório configurado. Você pode ajustar as configurações de logging no arquivo log4j2-spring.xml.

## Contribuindo
Sinta-se à vontade para contribuir para este projeto abrindo issues e pull requests. Sua contribuição é muito bem-vinda!

## Licença
Este microservice é distribuído sob a licença MIT. Consulte o arquivo LICENSE para obter mais informações.
