# reclamaNet
Este programa vai testar a sua conexão com a internet, gerar um log dos resultados e mandar um tweet para a sua operadora
reclamando da velocidade recebida.

## Configuração
A configuração é feita em um arquivo JSON
Neste arquivo você encontra as seguintes configurações
* twitter
 * twitterToken: O token de acesso ao twitter para o seu app
 * twitterConsumerKey: Sua Consumer Key (API Key)
 * twitterTokenSecret: Seu Access Token Secret
 * TwitterConsumerSecret: Seu Consumer Secret (API Secret)
* tweetTo: Para quem você quer enviar o tweet, é necessário colocar o @
* internetSpeed: A velocidade do seu plano de internet (sem o Mb/s)
* tweetThresholds: Aqui é onde esta a lista de mensagens que serão enviadas quando você não estiver recebendo a velocidade contratada
 * {tweetTo} - Mostrará aquilo que você cadastrou em tweetTo .
 * {internetSpeed} - Mostrará aquilo que você cadastrou como velocidade contratada.
 * {downloadResult} - Mostrará a velocidade que foi constatada no teste

## Como usar
> python reclamaNet.py

para rodar em  background:

> python reclamaNet.py > /dev/null &

## Instalando
> pip install -r requirements.txt


