# Desenvolvedor Magento

> Seguir o roteiro conforme descrito

## Roteiro da Prova

### 1. Instalação do Magento

- Faça download do magento: https://magento.com/tech-resources/download `(utilize a versão 1.9.4.x)`  

#### 1.2. Instalar módulo Pagar.me

O arquivo do módulo se encontra na raiz desse projeto: `pagarme-magento.zip`

##### Configurações:

>>>
**Modo**: Teste  
**Chave de API**: ak_test_qJFclo9K2JZvmRGjplBC6mgCGuHdDa  
**Chave de criptografia**: ek_test_kMvFsBVfltaVYj9HzPG4Q8HANpzQgM  
>>>

#### 1.3. Instalar módulo Correios

O arquivo do módulo se encontra na raiz desse projeto: `correios-master.zip`

##### Configurações:

>>>
**Serviços**: 
- 04510 - PAC SEM CONTRATO
- 04014 - SEDEX SEM CONTRATO
>>>

### 2. Desenvolvimento / Configuração Backend

- Configurar para que vendas não possam ser realizadas por convidados `(Allow Guest Checkout)`
- Configurar para que seja exibido Tax/Vat Number (CPF)
- Configurar para que sejam obrigatórios os campos de data de nascimento, gênero e Tax/Vat
- Configurar para que sejam exibidas 4 linhas de endereço que correspondem a: `Rua`, `Número`, `Complemento` e `Bairro`
- Configurar para que o país padrão seja o Brasil e **permitir** compras apenas para o brasil
- Configurar a Origem do Envio
- Adicionar Estados Brasileiros (http://mariosam.com.br/magento/sql-estados/)
- Cadastrar 3 produtos simples com estoque, pelo menos 1 foto 
- Customizar a listagem de pedidos para exibir os itens de pedido no grid e permitir filtragem dos mesmos

### 3. Desenvolvimento / Configuração Frontend

> `NÃO` é necessário **IMPLEMENTAR** as mascaras nos campos de CEP, CPF, Telefone e etc;  
> Quando for realizar o pedido favor formatar os campos pois o gateway do Pagar.me faz validações   
> (Ex.: em vez de digitar CPF como 12345678901 digitar como 123.456.789-01, aniversário 20022017 digitar como 20/02/2017)

- Fazer o Pedido utilizando o método de Boleto Bancário do Módulo Pagar.me
- Realizar uma compra com 2 itens e frete para 30110-017
- Criar novo módulo Destaque com link no menu da homepage e gerar nova rota no frontend para exibir um texto(oportunidade única) e um produto especifico

