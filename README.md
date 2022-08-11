# Arquitetura Geral

## Objetivo e Foco

A arquitetura do PingCast.com foi pensada e desenvolvida com foco em entregar valor de maneira iterativa e incremental o quanto antes possivel, com foco nisso pensamos em uma solução que permitisse o desenvolvimento das partes do projeto em simultâneo pelas equipes, reduzindo a interrupções, dependencias e desacordo entre as equipes. Para atender esse objetivo dividimos o sistema em serviços, que são subsistemas capazes de resolver problemas especificos e se comunicar com outros serviços desde que um não necessite do outro para funcionar enquanto na fase de desenvolvimento do projeto.

Além dos serviços terão os artefatos que devem ser documentos com finalidade de apoiar e orientar o desenvovimento de um serviço.

## Serviços

| Serviço    | Descrição |
| :------------- |:----------|
| PingCast API    | Uma aplicação que fornece uma interface para a web por meio do protocolo https com finalidade de disponibilizar diversos recursos como consulta de informações, processamento de dados e etc, essa interface terá niveis de acesso controlado por credenciais e token de autênticação. |
| PingCast Client        | Aplicação web(Front-end) fornecerá uma interface grafica em que o possa interagir pelo seu navegador ao acessar a url da mesma.     |
| PingCast Database        | Serviço responsavel pelos bancos de dados do sistema    |
| PingCast Infra        | Serviço reponsavel pela infraestrutura do sistema com finalidade de manter os demais serviços em nuvem com auta disponibilidade e saudaveis e algumas outras funcioalidade como sistema de armazenamento de arquivos. |
