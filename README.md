# Calculadora-em-javascript
Uma calculadora em JavaScript é um aplicativo interativo que permite aos usuários realizar operações matemáticas básicas como adição, subtração, multiplicação e divisão diretamente no navegador. Ela pode ser criada usando HTML para a estrutura da interface, CSS para o estilo visual, e JavaScript para a lógica de funcionamento.

Aqui está uma descrição geral de como essa calculadora pode ser implementada:

HTML:

Estrutura: A interface da calculadora geralmente inclui um display para mostrar os números e os resultados das operações, além de botões para os dígitos (0-9) e operadores (+, -, *, /, =).
Botões: Cada botão é representado por um elemento <button> que, quando clicado, aciona uma função em JavaScript.
CSS:

Estilo: O CSS é utilizado para definir a aparência da calculadora, incluindo a disposição dos botões, o tamanho do display, as cores, e outros aspectos visuais.
Responsividade: O design pode ser ajustado para diferentes tamanhos de tela, garantindo que a calculadora funcione bem em dispositivos móveis e desktop.
JavaScript:

Lógica: O JavaScript é responsável por implementar a lógica de cálculo. Isso envolve capturar os cliques nos botões, atualizar o display, e realizar as operações matemáticas quando o usuário pressiona o botão de igual (=).
Funções: As funções principais incluem a adição de números ao display, a execução das operações matemáticas, e a limpeza do display para uma nova operação.
Eventos: O JavaScript escuta os eventos de clique nos botões e atualiza o estado da calculadora de acordo.
Exemplo simples de código JavaScript para a lógica de uma calculadora:

javascript
Copiar código
let display = document.getElementById('display');

function addNumber(num) {
    display.value += num;
}

function clearDisplay() {
    display.value = '';
}

function calculate() {
    try {
        display.value = eval(display.value);
    } catch (e) {
        display.value = 'Error';
    }
}
Neste exemplo, o display é atualizado com o número clicado (addNumber()), limpo (clearDisplay()), e o resultado é calculado usando a função eval() no JavaScript (calculate()).

Nota: O uso de eval() pode ser perigoso se não for manipulado corretamente, pois pode executar código arbitrário. Para implementações mais seguras, é recomendável evitar eval() e usar outras abordagens para calcular expressões matemáticas.








