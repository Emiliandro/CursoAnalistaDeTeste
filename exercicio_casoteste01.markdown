#Caso de teste
> https://hvacnhurry.com/auth/
> Crie caso de teste para a ação de registro da e-commerce informada.

## Pre-condição
1. acessar https://hvacnhurry.com/auth/
2. Ter conexão (internet)

## Procedimentos
1. Clique no botão login
2. Clique no botão cadastro
3. Preencha os dados
4. Registre

## Casos validos
1. senha > 6
2. senha == confirmacao_senha
3. senha[0...9a...z!...)]

## Casos inválidos
1. mail != null
2. senha != null
3. ['null']@['null'].['null']

## Teste exploratório
1. dois usuários não podem ter o mesmo número
2. [0...9a...z!...)]@['edu'].['edu'] é valido

## Resultados esperados
1. Caso validado - border-shadow vermelho nos inputs seguido de um redirecionamento para a home
2. Caso invalidado - exibir mensagem informando o erro
>> senha curta, minimo 6 caracteres
>> e-mail já existe
>> e-mail mal formatado

## Senhas testadas
'''
___________
8888888
iiiiiiiiiiiii
'''