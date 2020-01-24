<img src="../../src/images/benner_rgb.png" align="right"/>

# Extrato de coparticipação - Requisitos

1. **[Introdução](#introdução)**
2. **[AG](#ag)**  
  2.1. **[Fatura(AG)](#Fatura-(AG))**  
  2.2. **[Documento (AG)](#documento-(AG))**  
  2.3. **[Demais parâmetros](#demais-parâmetros)**
3. **[MG](#mg)**  
  3.1. **[Fatura (MG)](#Fatura-(MG))**  
  3.2. **[Documento (MG)](#documento-(MG))**
4. **[Portal](#portal)**  
  4.1 **[Parametrização](#parametrização)**  
  4.2 **[Sincronização](#sincronização)**

## Introdução

Para que o extrato de coparticipação seja exibido no portal, será necessário seguir os requisitos abaixo.

# AG

## Fatura (AG)

> Beneficiários > Beneficiários > Conta Financeira > Faturas

* **Fatura:** Para que o extrato de coparticipação seja exibido no portal é necessário que:
  * O tipo de faturamento da fatura seja "Autogestão".
  * Possua lançamento com "Tipo de lançamento financeiro" Participação Financeira.
  * Possua Módulo com "Tipo" Utilização.

![001](src/images/001.png)

![002](src/images/002.png)

![003](src/images/003.png)

## Documento (AG)

> Beneficiários > Beneficiários > Conta Financeira > Documentos

* **Documento:** Para que o extrato de coparticipação seja exibido no portal é necessário que:

  * A "Natureza" do documento seja Crédito.
  * O documento não esteja cancelado.
  * Possua fatura com os requisitos citados anteriormente.

    ![004](src/images/004.png)

    ![005](src/images/005.png)

    ![006](src/images/006.png)

## Demais parâmetros

> Processamento de Contas > Peg > GUIA

"Eventos de guias" de reembolso onde a guia possui AbatePF marcado, não serão exibidas nos detalhes da coparticipação.

![010](src/images/010.png)

![011](src/images/011.png)

A importação das informações de coparticipação pode ser realizada com base na competência do documento ou pela data de vencimento. Definido pelo parâmetro a seguir.

> Adm > Parâmetros Gerais > Portal Serviços > Principal > Busca Histórico de coparticipação por

![012](src/images/012.png)

# MG

## Fatura (MG)

> Beneficiários > Beneficiários > Conta Financeira > Faturas

* **Fatura:** Para que o extrato de coparticipação seja exibido no portal é necessário que:
  * O tipo de faturamento da fatura seja "Pré-Pagamento".
  * Possua lançamento com "Tipo de lançamento financeiro" Participação Financeira.
  * Possua Módulo com "Tipo" Utilização.

![013](src/images/013.png)

![014](src/images/014.png)

![015](src/images/015.png)

## Documento (MG)

> Beneficiários > Beneficiários > Conta Financeira > Documentos

* **Documento:** Para que o extrato de coparticipação seja exibido no portal é necessário que:

  * A "Natureza" do documento seja Crédito.
  * Possua fatura com os requisitos citados anteriormente.

    ![017](src/images/017.png)

# Portal

## Parametrização

> Portal > Gestor - Portal Serviços > Preferências > Parâmetros Gerais > Período

No campo "Sincronizar Extratos de Coparticipacao por:" deve ser inserido o período desejado para importação de extratos de coparticipação, a parametrização pode ser feita por Período (Dias) ou por Competência (Mês).

![007](src/images/007.png)

![008](src/images/008.png)

## Sincronização

> Portal > Gestor - Portal Serviços > Painel de Sincronização > Gerenciador de Sincronizações

Para que os dados sejam apresentados no portal é necessário executar a sincronização "Extratos de Coparticipação".

![009](src/images/009.png)
