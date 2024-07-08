# calculadora

const prompt = require('prompt-sync')({sigint: true})

let num1 = 0
let num2 = 0
let resultado

calculadora()

function calculadora() {
    fany = prompt('Digite um número:') 

        if(fany == Number) {
        
            let calculo = prompt(`
            1. subtração(-)
            2. adição (+)
            3. multiplicação (*)
            4· Divisão (/)
            5. Porcentagem `)

            let conta = prompt('escolha uma operação')

            resultado = parseFloat('Digite outro número:')
            switch(conta) {
                case 'subtração':
                case '-':
                    resultado = num1 - num2
                    console.log(`o resultado é ${resultado}`)
                    break
                case 'adição':
                case '+':
                    resultado = num1 + num2
                    console.log(`o resultado é ${resultado}`)
                    break
                case 'multiplicação':
                case '*':
                    resultado = num1 * num2
                    console.log(`o resultado é ${resultado}`)
                    break
                case 'divisão':
                case '/':
                    resultado = num1 / num2
                    console.log(`o resultado é ${resultado}`)
                    break 
                case 'porcentagem':
                case '%':
                    resultado = num1 % num2
                    console.log(`o resultado é ${resultado}`)

            } 
        }
}
