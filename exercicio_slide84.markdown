# Casos de teste
> Um formulario de cadastro de usuario requer nome, cpf, mail e uma senha. Ao final existe um botao 'salvar', quais testes devem ser usados de acordo com os requisistos presente no slide?

## Testes usados
> Uso do processo de modelagem de teste de software (slide 97)
1. Partição em equivalencia
2. Análise do valor limite
3. Teste com base em experiência

## Teste exploratório
1. dois usuários ter o mesmo cpf
2. dois usuários ter o mesmo e-mail

## Casos validos
* c1 - cpf = 11
* c2 - cpf [0...9]
* c3 - mail com [a..z&0...8]@[a..z&0...8].com.[a..z&0...8]
* c4 - senha > 5 and senha < 11
* c5 - senha [a..z&0...8&!...)]
* c6 - nome > 1
* c7 - nome != null
* c8 - nome não é apenas [&...8]

### Casos inválidos
* c9 - cpf > 11
* c10 - cpf < 11
* c11 - cpf[a...z]
* c12 - cpf[!...)]
* c13 - e-mail sem @
* c14 - @[!...)].[!...)]
* c15 - @['edu'].['edu']
* c16 - ['null']@['null'].['null']
* c17 - senha < 6
* c18 - senha > 10
* c19 - senha só com [0...9]
* c20 - senha só com [a...z]
* c21 - senha só com [!...)]
* c22 - nome só com [!...)]
* c23 - nome ['null']

## Resultados esperados
1. Caso validado - exibir mensagem "Usuário cadastrado com sucesso"
2. Caso invalidado - exibir mensagem informando o erro e pedindo pro usuário corrigir os dados

## Metricas
1. Nº aprovado divido pelo Nº planejado
2. Em caso de erro, avisar o usuário e não cadastrar

### Slide 93 - Monitoramento do planejamento
1. % trabalho preparado
2. % resultados negativos
3. % resultados positivos
4. Densidade dos defeitos
5. Resultado de retestes
6. Custo dos testes
7. Relação Defeito-Ocorrência
8. Categoria dos defeitos