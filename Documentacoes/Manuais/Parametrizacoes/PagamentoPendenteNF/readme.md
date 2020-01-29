<img src="../../src/images/benner_rgb.png" align="right"/>

# Pagamento Pendente de Nota fiscal

1. **[Introdução](#introdução)**
2. **[AG](#ag)**  
  2.1 **[Pagamento](#pagamento)**  
  2.2 **[Caso 1](#caso-1)**  
  2.3 **[Caso 2](#caso-2)**  
  2.4 **[Caso 3](#caso-3)**
3. **[Portal](#portal)**  
  3.1 **[Sincronização](#sincronização)**
4. **[Como funciona](#como-funciona)**

## Introdução

Para o funcionamento da rotina de pagamento pendente de nota fiscal, será necessário seguir as seguintes parametrizações.

# AG

## Pagamento

Para que o pagamento pendente de nota fiscal seja exibido no portal, deve se enquadrar em uma das situações a seguir.

### Caso 1

"Tipo documentos fiscais" deve ser "Nota fiscal"

O Documento fiscal não deve possuir nota

O valor do pagamento deve ser maior que 0

O pagamento deve estar fechado

![001](src/images/001.png)

![002](src/images/002.png)

### Caso 2

"Tipo documentos fiscais" deve ser "Nota fiscal"

O documento deve possuir Nota fiscal com status "Indeferido"

O valor do pagamento deve ser maior que 0

O pagamento deve estar fechado

![005](src/images/005.png)

![006](src/images/006.png)

### Caso 3

"Tipo documentos fiscais" deve ser "Nota fiscal"

O documento deve possuir Nota fiscal com status "Em Análise"

O valor do pagamento deve ser maior que 0

O pagamento deve estar fechado

O Status da conciliação deve ser "Não conciliado"

![003](src/images/003.png)

![004](src/images/004.png)

# Portal

## Sincronização

> Painel de Sincronização > Gerenciador de Sincronizações > Pagamentos Pendentes de Nota Fiscal

A sincronização será realizada buscando pagamentos pendentes de nota fiscal que se enquadram em algum dos casos citados anteriormente.

![007](src/images/007.png)

## Como funciona

Ao vincular uma nota fiscal ao pagamento, será enviado o número da nota, série da nota, Data de emissão, valor, anexo e caso tenha sido incluído itens na nota, os mesmos também serão enviados. Todas as informações serão vínculadas ao registro de pagamento.

Pagamento pendente de NF.
![008](src/images/008.png)

![009](src/images/009.png)

Anexado nota fiscal ao pagamento.
![010](src/images/010.png)

![011](src/images/011.png)

Incluído item na nota fiscal.
![012](src/images/012.png)

![013](src/images/013.png)

![014](src/images/014.png)

Nota indeferida.
![015](src/images/015.png)

Sincronização executada.
![016](src/images/016.png)

![017](src/images/017.png)
