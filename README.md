# Funcao-recursiva-exemplos

function resposta(array, end) {
    switch(true) {
        case end === array.length:
            return 0
        default:
            console.log(array[end]) //resposta 1 , 2, 3, 4, 5
            return resposta(array, end + 1 ) + arra[end] //resposta 15 soma de todos o números do Array        
    }
}

resposta([1,2,3,4,5], 0)

function resposta(count) {
    switch(true) {
        case count === 0:
            return 1
        default:
            console.log(count) // resposta 5, 4, 3, 2, 1
            return resposta(count - 1 ) * count // resposta 120
    }
}

resposta(5)
