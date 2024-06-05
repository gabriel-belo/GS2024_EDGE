# GS2024_EDGE
Projeto de EDGE para a Global Solution 2024

<table>
  <tr>
    <th> Nome </th>
    <th> RM </th>
  </tr>
  <tr>
    <td> Gabriel Belo </td>
    <td> 551669 </td>
  </tr>
  <tr>
    <td>Gustavo Pierre</td>
    <td>558928</td>
  </tr>
  <td> Gabriel Galerani </td>
  <td> 557421 </td>
</table>


<h1>Link Para o projeto</h1>
https://www.tinkercad.com/things/iRVuRnD8kkv-copy-of-prototipo-de-monitoramento-de-qualidade-de-agua/editel?tenant=circuits


<h1>Foto do sistema:</h1>
<img src="https://github.com/gabriel-belo/GS2024_EDGE/assets/126474319/06aa14d8-ca34-4ceb-b544-d78c9c64fc0b"/>


<h1>Materiais:</h1>
<ul>
  <li>Arduin Uno</li>
  <li>Breadboard</li>
  <li>LCD 16x2</li>
  <li>Resistor</li>
  <li>3x Potenciômetro</li>
  <li>TMP 36</li>
</ul>


O sistema é desenvolvido com um Arduino Uno visando o monitoramento das águas. Para a coleta de dados foram utilizados três sensores o TMP 32 e dois Potenciômetros que simulam um sensor de pH e o outro um sensor de oxigênio dissolvido na água, o TMP 32 coleta dados da temperatura da água e os Potenciômetros do pH e do oxigênio na água. Para informar o estado do ambiente utilizamos o LCD apresentando os dados em tempo real e um alerta de acordo com o estado em que cada dado se apresenta, sendo eles alto, médio e baixo para temperatura e oxigênio dissolvido na água e para o pH os parâmetros são ácido, neutro e básico. O código inicia com a importação da biblioteca LiquidCrystal. Então no void setup temos a inicialização da comunicação serial e configuração das colunas e linhas do LCD e printamos no monitor serial uma mensagem de início. 
O void loop inicia com a definição do pino analógico de um dos Potenciômetros que simula o sensor de pH em seguida vem os cálculos que transformam os dados do Potenciômetro para valores de pH, então temos o sensor de temperatura e alguns cálculos para fazer a transformação para celsius, e por último a leitura do pino A2 do segundo Potenciômetro que a partir de alguns cálculos gerá os dados de oxigênio dissolvido. Depois temos a impressão no monitor serial e no LCD.
