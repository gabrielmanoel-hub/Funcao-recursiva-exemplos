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





function main(array, x, y, cor) {
   remove(array, x, y, cor)
    if(x === array.length) {
        return 
    } else {
        main(array, x + 1, y, cor) 
    }
}

function remove(array, x, y, cor) {
    if(array[x - 1][y] === 1) {
        array[x - 1][y] = cor
        console.log(array[x - 1])
    }
}
main([[1,1,1], [1,1,0],[1,0,1], [0,1]], 1, 1, 2)
// Resposta
[ 1, 2, 1 ]
[ 1, 2, 0 ]
[ 0, 2 ]
