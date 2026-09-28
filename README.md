# alertas-demandas-rh-power-automate
Automação com Power Automate para apoiar o acompanhamento de demandas de RH, com alertas por e-mail nas faixas de 7, 15 e 30 dias.

# Alertas automáticos para acompanhamento de demandas de RH

Desenvolvi esta automação com Power Automate para apoiar o acompanhamento de solicitações de departamento pessoal, como pedidos de férias.

O objetivo é dar visibilidade às demandas que precisam de atenção e ajudar a equipe a evitar o acúmulo de pendências.

## Como funciona

O fluxo executa uma verificação diária, consulta as solicitações registradas e calcula o tempo decorrido desde a abertura de cada uma.

Os alertas são organizados em três faixas:

- **7 dias:** primeiro aviso de atenção.
- **15 dias:** reforço para acompanhamento.
- **30 dias:** nível máximo de atenção definido para o processo.

Esses períodos são critérios de acompanhamento do projeto.

## Controle dos avisos

A automação registra a última faixa de alerta enviada para cada solicitação. Esse controle evita repetir o mesmo aviso nas verificações seguintes.

A análise começa pela faixa de 30 dias, depois passa por 15 e 7 dias. Assim, quando uma solicitação já está na faixa mais alta, o fluxo envia o alerta correspondente, sem disparar os avisos anteriores na mesma execução.

## Tecnologias utilizadas

- **Power Automate:** verificação diária, cálculo do tempo e regras de envio.
- **SharePoint:** consulta das solicitações e registro do último aviso.
- **Outlook:** envio dos alertas por e-mail.

## Minha participação

Desenvolvi a lógica de acompanhamento, as condições para cada faixa de prazo, os e-mails de notificação e o controle dos avisos enviados.

## Próximo ajuste

Adicionar a verificação da situação da solicitação antes do envio, para que apenas demandas ainda elegíveis ao acompanhamento recebam os alertas.

## Sobre esta apresentação

Este repositório apresenta uma descrição do projeto para portfólio. Não disponibiliza dados pessoais, arquivos de produção ou configurações internas.

## Autora

Letícia Santana  
Desenvolvimento de soluções com Microsoft Power Platform.
