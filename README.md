# Learning HTTP Fundamentals

> Notes regarding course about HTTP Fundamentals, HTTPS and REST services.

## O que é HTTP

* HTTP: Sigla/Abreviação para Hypertext Transfer Protocol.
* Independente de plataforma de desenvolvimento.
* O HTTP é um protocolo que define um conjunto de regras que faz essa relaçao Cliente - Servidor acontecer. Logo, o protocolo HTTP segue o modelo `Client - Server`.
* Relação Navegador - Internet - Servidor. (Cliente - Servidor)

### Relação Cliente - Servidor

* O Servidor devolveu uma resposta? Meu navegador tem que tratar isso.
* Ou seja, o HTTP estabelece as regras que existirão entre os dois lados.
* RFC2616 define as regras/especificação do HTTP.
* O Navegador é quem "faz o papel do Cliente".
* Quem fornece o conteúdo é o Servidor.
* O `Client` inicia a comunicação e o `Server` responde.
* O modelo Cliente-Servidor tenta centralizar o trabalho no servidor, mas isso também pode gerar gargalos.

### Diferentes protocolos

* No protocolo P2P (Peer to peer, muito utilizado em Torrents) o Cliente assume um pouco a responsabilidade do Servidor, dividindo as tarefas.
* Existem vários protocolos em TI (Ex: SMTP, FTP, P2P...), no entanto, HTTP é o mais popular dentre eles.

### Exemplo de arquitetura

`Client (Navegador)` <-- HTTP --> `Servidor Java (Tomcat)` <-- SQL --> `Banco (MySQL)`

* Há arquiteturas muito mais complexas, mas a grande maioria usa o protocolo HTTP no topo.
* O protocolo HTTP garante a conectividade. Isso quer dizer que o protocolo HTTP funciona em todos os lugares, sem ter problemas com firewalls e outras regras de segurança.

## HTTPS

* Versão segura do HTTP.
* HTTP Comum adicionado de uma camada de segurança/criptografia que antes era `SSL`, mas posteriormente passou a ser também `TLS`.
* SSL/TLS: Secure Sockets Layer / Transport Layer Security

### Identidade

* Identidade Confirmada - Certificado Digital (Tem a Chave Publica para criptografar os dados) e o Servidor tem a Chave Privada, dessa maneira intermediarios não conseguem descriptografar.
* Chrome Dev Tools tem uma aba para verificação da Segurança e certificado.
* Certificados Digitais provam a identidade, mas tem validade. Ex. de autoridade certificadora: COMODO.
* Autoridades Certificadores garantem que os certificados que estão sendo utilizados podem ser confiados, através de uma assinatura digital.
* Então, HTTPS começa com criptografia assimétrica (mais lenta) para depois mudar para criptografia simétrica (mais rápida).
* A chave simétrica será gerada no início da comunicação e será reaproveitada nas requisições seguintes






