# Fonte de Tensão ajustável(3v - 12v)

## Objetivo:
Construir uma fonte capaz de transformar a corrente alternada de tensão média de **127V** para a corrente de **12V** contínua.

## Tabela dos componentes:
| Componentes | Quantidade | Valor unitário R$ |
|-------------|  :---:  |----------|
| Capacitor Eletrolítico (470uF) 35V       | 0 | 0,00 |
| Diodo 1N4004                             | 0 | 0,00 |
| Diodo Zener (13V)                        | 0 | 0,00 |
| Potenciômetro Linear 5k                  | 0 | 0,00 |
| Resistor 2.2K                            | 0 | 0,00 |
| Resistor 3k                              | 0 | 0,00 |
| Transistor NPN-2N2222                    | 0 | 0,00 |
| Led vermelho                             | 0 | 0,00 |
| Resistor 1.5k                            | 0 | 0,00 |
| | Total: | 9,39 |

## Componentes:

* **Transformador**: é o primeiro componente, que transforma os 127v da ddp proveninete da tomada para valores menores desejados para o projeto. O transformador escolhido é capaz de abaixar a tensão alternada de 110 volts para 12 volts com 24v de pico, mas não altera as propriedades da tensão e da corrente, mantendo ambas alternadas.
* **Ponte de diodo**: é o segundo momento do circuito em que faz a corrente deixar de ser alternada, mas mantém a corrente pulsada, pois faz os ciclos da corrente passarem para o circuito sempre de maneira positiva.
* **Capacitor**: é o terceiro componente (em paralelo com todo o restante do circuito), que armazena a carga durante os ciclos da corrente alternada, liberando corrente quando a tensão interna é maior que a tensão vinda da fonte. Descarrega quando ocorre a inversão de ciclo. Como demonstrado nos cálculos da próxima seção, para alcançar o valor de riple de 10% (2,4V pois o pico é de 24V), a capacitância calculada deve ser de 347uF, portanto, optamos por pegar o capacitor de 470uF pela folga e compatibilidade con valores comerciais.
* **Resistores**: estão presentes por todo o circuito para limitar a corrente e evitar a queima dos dispositivos. Os resistores estão associados em série com vários componentes, tais como: o LED, o Diodo Zener, o potenciômetro e na saída final (para fins de medição).
* **LED**: é o próximo item em paralelo ao capacitor, que permite mostrar a passagem da corrente, ou seja, mostrar que a fonte está operante.
*  **Diodo Zener**: é o quarto período do circuito que regula a tensão máxima. Ele mantém a tensão dos seus terminais fixa numa tensão constante, no caso, em 13v, quando a tensão fornecida a ele é maior que a constante. Além disso, se oferecida uma ddp insuficiente para alcançar a constante, o diodo não conduz e não interfere no circuito.
*  **Potenciometro**: é o quinto momento do circuito, que consiste num resistor variável que permitirá o controle do valor da tensão resultante entre 3 e 12 volts.
*  **Transistor**: é a parte final do circuito, que amplifica a corrente pequena que chega na sua base para o desejado de no máximo 100mA. 

## Cálculo do capacitor

![CodeCogsEqn (1)]()


![CodeCogsEqn (3)]()


## Cálculo do resistor do LED

![CodeCogsEqn (4)]()



## Imagem da fonte no simulador
![image](https://github.com/LuisHenriique/Fonte-de-tens-o-ajust-vel/assets/96901986/f8ab45dc-2c73-48d5-b631-f2873c16ce75)
Link da fonte: [https://tinyurl.com/23abu5a5](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcDoBYDsAmdA2dBOdMMADhzEnxAGZIQkE6EBTAWmICgB3GzOsHHUwIc4QVG6861EqhDDRMuZEnU+Y6QkwaJPNdNk0tNQyp45U-cThIkdZkBYNybdpbse2Tc3G9OTXHV97DgATEGCBOhwReSx5EFDmADMAQwBXABsAFzCQWyF4yPFtJLSs3PCCuO1g91KUjJy8usMY0WxtBvLm81jOx1jUEjoHaoH8EviHdpBhukm6eYkBbQovS35IL30Esqbs1kzmcIhRqFgwSXW7ZeJIOWWHG5rwbbd1Z-fX+7kBlQATm8NnBgbcRlB6PBrt8JlNtF8NhDFnMIc8KH94sRDP9rhjUfxSI80XicVi+IUEaTifwKQSJAAvcB0gZgOnUGx7RoVVgM5gAO2YAI4QLZoNQAmZ4rRbzgHDA6DkbIhuzZkzmoIgjFBMHw+G18EN8AgACVmABnACW5uyqX5AGNmCLmRDWZgVZ95NCeGLKS6-YDkBypEHFKYpRwAA5iSXuASx9TUSEqAAq3h0TnTSwu2lYMHI1AQlhkJEwevQkDASBg6FrIwQ6BIxCwZYwFz1+FUhiiRjW4gche07mH-ntIBRyxR-wu8Co1FQ0HW1D17SLkzOsErHAAbvJYj2FFnwI5+ARkxcEBwAB4RdBJxjofJ4egUObyOSRgD2Vuylu3n+vN5MD+VAqAoHAqGEbQQJAABzflQmuOkJVEX0aE5Z5kMlZUlklTD1Q5OwwHnORCIkbJwGoXB0KIqjRBQyEIFYd00HwYZsTYzAcBsdV83wYiINQCC8G2CVHwoOh9gqa4SJoyjqLI55l2g7DUEsOY8OuNTcNQ7T6WePS7mQkkfQ5HTKPELQ7CUyz3VDeg7OeBBgys+yGMw10sS0ANrm8n5nI6aZfODVUAteJzgwYqsQv8H1yDDJUwvcZ54pDaLFE+DhYPHeEcv4fAEQkIA)
## PCB da fonte
![image]()
## Pasta do projeto do EAGLE




## Vídeo no YouTube
.....

### Alunos:
* Luis Henrique Ponciano dos Santos
* Dante Brito
* Gabriel de Araujo
* Pedro Bizon
