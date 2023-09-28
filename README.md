# Bubble Sort em Ruby
Este é um exemplo simples de implementação do algoritmo de ordenação Bubble Sort em Ruby.

## [O que é o Bubble Sort?](https://www.youtube.com/watch?v=8Kp-8OGwphY)
## Como funciona
O algoritmo Bubble Sort funciona comparando cada elemento do array com o próximo e trocando-os de lugar se estiverem fora de ordem. Este processo é repetido até que não seja mais necessário trocar nenhum elemento de lugar, o que indica que o array está ordenado.

Neste código, o loop do continua até que a variável swapped permaneça false, o que significa que nenhum elemento foi trocado na última passagem pelo array, indicando que o array está ordenado.

## Para utlizá-lo:
1. Clone este repositório para sua máquina local usando o comando git clone.
2. Navegue até a pasta do projeto no seu terminal.
3. Execute o programa com o comando ruby bubble_sort.rb.
4. Quando solicitado, insira o array que você deseja ordenar.

## Como usar
Para usar este código, você precisa passar um array para a função bubble_sort. A função irá retornar o array ordenado.
```
array_desordenado = [4, 3, 2, 1]
array_ordenado = bubble_sort(array_desordenado)
puts array_ordenado # Saída: [1, 2, 3, 4]
```
## Código

```
def bubble_sort(array)
    loop do
        swapped = false
        (array.length - 1).times do |i|
            if array[i] > array[i + 1]
                array[i], array[i + 1] = array[i + 1], array[i]
                swapped = true
            end
        end
        break if not swapped
    end
    array
end
```




## License
This project is licensed under the MIT License - see the [LICENSE.md] file for details.

## This is an assignment from [The Odin Project](https://www.theodinproject.com/lessons/foundations-git-basics)
