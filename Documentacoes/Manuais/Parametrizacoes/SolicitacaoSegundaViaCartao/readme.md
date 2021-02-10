<img src="../../src/images/benner_rgb.png" align="right"/>

# Solicitação 2ª via cartão

1. **[Introdução](#introdução)**
2. **[Motivos para emissão](#Motivos-para-emissão)**
3. **[Sincronizações](#Sincronizações)**
4. **[Solicitando 2ª via de carteirinha pelo portal](#Solicitando-2ª-via-de-carteirinha-pelo-portal)**
5. **[Atendimento de solicitações](#Atendimento-de-solicitações)**

## Introdução

Neste manual será abordado de forma simples as parametrizações necessárias para a utilização da funcionalidade de solicitação 2ª via de carteirinha.

## Motivos para emissão

> Beneficiários > Tabelas > Motivos para o cartão

Para a exibição dos motivos de solicitação de 2ª via de cartão no portal, primeiramenre será necessário criar um motivo de cartão com o flag "Visualiza na web" no sistema Saúde.

Caso o "tipo de solicitação cartão" seja "Furto/Roubo", será exibido um campo para anexo de arquivos no momento da solicitação de 2ª via.

![001](src/images/001.png)

> Beneficiários > Contratos > Motivos de emissão do cartão

O motivo criado anteriormente deverá ser vinculado aos contratos que poderão solicitar o mesmo.

![002](src/images/002.png)

## Sincronizações

> Gestor - Portal Serviços > Painel de Sincronização > Gerenciador de Sincronizações > Contratos motivo cartão

Para que os motivos sejam exibidos no portal, é necessário executar a sincronização "Contratos motivo cartão".

![003](src/images/003.png)

> Gestor - Portal Serviços > Painel de Sincronização > Gerenciador de Sincronizações > Solicitação de Segunda Via Carteirinha

A sincronização "Solicitação de Segunda Via Carteirinha" realizará o envio de solicitações com status "Solicitada" para análise no sistema saúde.

![004](src/images/010.png)

> Gestor - Portal Serviços > Painel de Sincronização > Gerenciador de Sincronizações > Situação de Segunda Via Carteirinha

Para que o status das solicitações de 2ª via da carteirinha sejam atualizadas, será necessário executar a sincronização "Situação de Segunda Via Carteirinha".

![005](src/images/011.png)

## Solicitando 2ª via de carteirinha pelo portal

> Beneficiário > Carteirinha >  Solicitar 2ª via

A página "Solicitação de 2ª via da carteirinha" permite ao beneficiário solicitar sua 2ª via de cartão indicando o motivo e o beneficiário a ter o cartão emitido. Caso o motivo seja furto/roubo, um novo campo será exibido para o anexo do BO.

![006](src/images/004.png)

> Beneficiário > Carteirinha > Histórico 2ª via

O beneficiário poderá acompanhar o status de sua solicitação através da funcionalidade "Histórico 2ª via". O status da solicitação somente será atualizado após a execução da sincronização "Situação de Segunda Via Carteirinha".

![007](src/images/005.png)

## Atendimento de solicitações

> Beneficiários > WEB > WEB:Movimentação de Beneficiários > Monitor de Análise/Pendência

A liberação/recusa da solicitação de 2ª via é feita por meio da aprovação ou recusa das mensagens de pendência. Caso todas mensagens tenham sido aprovadas, a solicitação também é aprovada, caso alguma pendência tenha sido negada, a solicitação também será negada.

![008](src/images/006.png)

![009](src/images/007.png)

![010](src/images/008.png)

![011](src/images/009.png)

![012](src/images/012.png)
