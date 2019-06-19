<img src="../../src/images/benner_rgb.png" align="right"/>

# Parametrizações - Reembolso online

1.  **[Introdução](#introdução)**
2.  **[Tipo de Reembolso](#tipo-de-reembolso)**
3.  **[Tipo de reembolso online](#tipo-de-reembolso-online)**
4.  **[Parametrização geral](#parametrização-geral)**
5.  **[Contratos](#contratos)**

## Introdução

Para que o reembolso online funcione no **Portal** é necessário qua a tarefa *"Reembolso online"* esteja associada ao papel de Beneficiário ou ao papel de realizará a parametrização.

## Tipo de Reembolso

> Processamento de contas > Tabelas > Tipos de reembolso

Ao iniciar a inclus"ao de um novo tipo de reembolso, os seguintes campos serão apresentados para a parametrização:

* **Descrição:** nome do reembolso que será apresentado no portal;
* **Tipos:**
  * **Consultas:** permite ao beneficiário preencher os campos CPF/CNPJ do prestador, nome do prestador, evento, nome do profissional, data do atendimento, sigla do conselho do profisisonal, número da inscrição no conselho, estado, valor total pago, número da nota fiscal;
  * **Atendimento médico/odontológico:** permite ao beneficiário preencher os campos CPF/CNPJ do prestador, nome do prestador, data do atendimento, data da emissão da nota fiscal/recibo, nome do profissional, sigla do conselho do profissional, número da inscrição no conselho, estado, valor total pago, número da nota fiscal/recibo;
  * **Medicamento:** permite ao beneficiário preencher os campos CPF/CNPJ do prestador, nome do prestador, data do atendimento, data da emissao da nota fiscal/recibo, valor total pago, número da nota fiscal/recibo;
    * Para o tipo *medicamento*, existe a possibilidade de habilitar para o beneficiário preencher uma lista de medicamentos. Para realizar uma inserção na lista, é necessário que o beneficiário informe o *evento*, *quantidade* e *valor total*.
    * Para este tipo de reembolso é possível informar o grau medicamento na parametrização.
* **Valor mínimo (S/N; Informar valor):** não permite que o beneficiário solicite um reembolso com valor menor que o mínimo informado;
* **Exige autorização (S/N):** é adicionado o campo obrigatório *autorização*, não permitindo que o beneficiário solicite um reembolso sem informar uma autorização existente no sistema saúde;
* **Exige prescrição (S/N):** é adicionado o campo obrigatório *prescrição*, não permitindo que o beneficiário solicite  um reembolso sem informar uma prescrição existente no sistema saúde;
* **Tipo de PEG:** quando o reembolso é criado no saúde, será do tipo informado na parametrização;
* **Evento padrão:** quando, na solicitação, não são preenchidas as informações referentes ao evento, será utilizado o evento parametrizado para a criação da guia;

![001](src/images/001.png)

## Tipo de reembolso online 

> Processamento de contas > Tabelas > Parametrização reembolso online

Ao iniciar a inclusão de uma nova parametrização de reembolso online, os seguintes campo serão apresentados para parametrização:

* **Tipo de reembolso:** tipo de reembolso online (carga: Tipos de reembolso);
* **Situação:** define-se se o reembolso está ativo ou não;
* **Mensagem informativa ao usuário:**
  * **Passo 1, 2 e 3:** é possível parametrizar a mensagem informativa principal e uma mensagem secundária para o beneficiário, quando estiver no passo correspondente;
* **Análise sem documentação física (S/N. Em qual a fase é permitida):** permite a análise da solicitação sem documentação física, sendo possível escolher até qual fase será permitida, sendo elas: *conferência*, *verificação* e *pronto*;
* **Prazo para apresentação da documentação física:** prazo para o beneficiário apresentar a documentação física;
* **Motivo glosa de cancelamento da documentação física:** glosa padrão para cancelamento da documentação física.

## Parametrização geral

> Adm > Parametros gerais > Processamento de contas > Reembolso online (aba)

No caminho informado deve ser apresentado os seguintes campos para parametrização:

* **Orientações gerais - Dados bancários:** mensagem padrão alertando beneficiário sobre os dados bancários:
  * **Mensagem principal e secundária:** escolha da operadora;
* **Orientações gerais - Dados bancários incompletos:** mensagem padrão alertando beneficiário sobre os dados bancários:
  * **Mensagem principal e secundária:** escolha da operadora;
* **Validar data emissão nota expirada (S/N; Quantidade de dias para a validação):** define o prazo de dias para o beneficiário enviar a solicitação de reembolso a partir da data de emissão da nota;

## Contratos

> Beneficiários > Contratos > Tipo de reembolso

Ao incluir um novo registro na carga, é habilitado aos beneficiários do contrato a realizar o tipo de reembolso escolhido.