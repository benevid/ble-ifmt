![](https://tva1.sinaimg.cn/large/006y8mN6gy1g73dk4h33oj30ss0g8jrr.jpg)

# Minicurso JEnPEx 2019

Este guia apresenta tudo que você precisa para começar a criar aplicativos móveis para a Internet das Coisas em JavaScript/HTML usando o Evothings Studio.  No entanto, existem outras ferramentas similares que você pode utilizar para desenvolver aplicações de forma similar:

- https://phonegap.com
- [https://thunkable.com](https://thunkable.com/)
- http://appinventor.mit.edu/

## Guia de Iniciante do Evothings Studio

# benevid@gmail.com

# 41 99258-2733 (whats)

O Evothings Studio é uma ferramenta de desenvolvimento para criar aplicativos móveis para a Internet das Coisas (IoT). Ele é baseado em tecnologias da Web e componentes de software de código aberto.

As ferramentas que você usa para desenvolver aplicativos com o Evothings Studio:

- **Evothings Viewer** - aplicativo móvel que executa todos os aplicativos escritos em HTML / JavaScript (instale-o nas lojas de aplicativos). Conecte-se do aplicativo Viewer ao Workbench e receba atualizações ao vivo de todos os aplicativos em que está trabalhando.
- **Evothings Workbench** - Use o Workbench para executar aplicativos no Evothings Viewer. Ele roda em seu laptop ou computador de mesa, próximo ao seu editor de código. O Workbench apresenta uma interface visual com o usuário, aplicativos de exemplo, uma barra de ativação para seus projetos de aplicativos, recarga automática ao vivo nas ferramentas de salvamento de arquivos, registro e avaliação de código. O Evothings Workbench vem com o download do Evothings Studio.
- **Seu editor de texto favorito ou editor de código IDE** (não incluído no download do Evothings Studio). Quando você pressiona salvar no editor, o Evothings Workbench notará o arquivo atualizado e acionará uma recarga do seu aplicativo em execução no Evothings Viewer. Isso permite um fluxo de trabalho de desenvolvimento rápido.

O Evothings Workbench vem com uma coleção de aplicativos de exemplo prontos para uso para vários dispositivos de IoT, por exemplo, beacons Eddystone e iBeacon, Arduino, TI SensorTag e muito mais.

### O que será preciso

Para começar, aqui está uma lista do que será necessário: 

- Computador laptop/desktop executando Windows, OS X ou Linux.
- Celular ou tablet executando iOS (iOS 7 ou posterior) ou Android (para usar o Bluetooth Low Energy, você precisa de um dispositivo com Bluetooth 4.0 ou posterior executando o Android 4.3 ou posterior).
- Download Evothings Studio - Instale o Evothings Workbench descompactando o pacote de download no seu laptop ou computador de mesa.
- Instale o Evothings Viewer - Faça o download na Apple App Store ou no Google Play.
- Para executar os aplicativos de exemplo que acompanham o Evothings Studio, você precisa do hardware usado por cada exemplo; Existem exemplos que funcionam imediatamente e sem hardware especial, como os exemplos do **Cordova Accelerometer** e **BLE Scan**.
- **Para criar aplicativos nativos**, você precisa do sistema de compilação **Apache Cordova**.

### Como editar código

O próximo passo é modificar o código de exemplo:

- Pressione o botão **COPY** no exemplo "Hello World". Isso fará uma cópia do aplicativo e aparecerá na guia "Meus aplicativos".
- Pressione **RUN** para iniciar o aplicativo no telefone ou tablet conectado. Pressionar **RUN** torna o aplicativo atualmente ativo. O aplicativo ativo é monitorado para alterações de código e, quando um arquivo é alterado, o aplicativo é recarregado automaticamente nos dispositivos conectados. É como se o **RUN** fosse pressionado automaticamente por você!
  Pressione o botão **CODE** no aplicativo "Hello World" em "Meus aplicativos". Isso abrirá o navegador de arquivos do sistema para os arquivos do aplicativo.
- Para ver a atualização ao vivo em ação, abra o arquivo index.html em um editor de texto. Você pode usar seu editor ou IDE favorito. Faça algumas alterações interessantes no código, por exemplo modifique o cabeçalho `h1` para dizer "Olá Evothings".
  Salve o arquivo (normalmente pressione **CTRL + S**). Feito! O aplicativo agora é recarregado automaticamente no Visualizador - as alterações são visíveis instantaneamente.

### Crie seu próprio projeto

Para criar seu próprio projeto de aplicativo móvel, você tem três opções:

- Clique no botão **NOVO**. Isso fornecerá um esqueleto de aplicativo em branco.
- Clique no botão **COPIAR** em um aplicativo de exemplo. Você pode modificar o aplicativo e continuar a partir daí.
- Arraste qualquer arquivo **HTML** para a janela Evothings Workbench.

Todos os métodos acima criarão uma entrada na guia "**Meus aplicativos**". Você pode reorganizar as entradas do aplicativo usando arrastar e soltar. Feche-os usando o ícone **Fechar (x)**. Isso não removerá os arquivos no disco.

> ☕︎ Quando você cria um aplicativo usando **NOVO** ou **COPIAR**, os arquivos do aplicativo são salvos em uma pasta no disco. Você pode especificar a pasta em uma caixa de diálogo. Se você deseja mover o aplicativo para outra pasta, exclua o item do aplicativo em "Meus aplicativos" (não excluirá a pasta do aplicativo). Mova a pasta do aplicativo para o novo local. Arraste index.html do navegador de arquivos do sistema para "Meus aplicativos".

#### Criar Aplicativo do zero ou adicionar um existente

- Criar uma pasta com os arquivos do projeto (arquivos HTML / CSS / JavaScript / media).
  É necessário que haja pelo menos um arquivo HTML no projeto - usado como ponto de entrada do aplicativo. 

- Arrastar o arquivo HTML principal, por exemplo o `index.html`, na lista de aplicativos no Evothings Workbench.
- Agora, basta pressionar **RUN** no aplicativo para iniciá-lo no Visualizador. 

> ☕︎ Observe que você pode conectar vários telefones celulares e tablets ao Evothings Workbench. Quando você salva qualquer arquivo no projeto (ou pressiona RUN), o aplicativo é recarregado em todos eles!

Um projeto de aplicativo do Evothings é apenas uma pasta com seus arquivos HTML e JavaScript. Assim como qualquer site. E assim que tudo é alterado, o Workbench o envia a todos os espectadores conectados, assim!

### Configurações do ambiente de trabalho

No menu "Mais", você encontrará a opção de menu "Configurações". Isso abre uma caixa de diálogo na qual é possível alterar o tamanho da fonte usada na janela Ferramentas e o número de níveis de diretório percorridos pelo observador de arquivos recarregado. Você também pode alterar o caminho padrão para a pasta usada pelos botões **NOVO** e **COPIAR**.

> ☕︎ A configuração do endereço do servidor de recarga é destinada aos desenvolvedores do Evothings Studio. Na maioria dos casos, você não deve alterar esse valor. O valor padrão é "https://deploy.evothings.com". O servidor de recarga lida com a comunicação entre o Evothings Workbench e os telefones e tablets conectados.

![Apache_Cordova1](https://evomedia.evothings.com/2015/02/Apache_Cordova1.png)

O Apache Cordova é um sistema de construção (build) para criar aplicativos nativos desenvolvidos em HTML/JavaScript. Você pode usar o Evothings Studio sem o Cordova, mas se quiser criar aplicativos nativos, é necessário.

> ☕︎ É útil saber que o próprio Evothings Viewer é um aplicativo Cordova, desenvolvido usando o Evothings Studio.

Os plug-ins Cordova são módulos de código que fornecem funcionalidade nativa do dispositivo, como Bluetooth Low Energy e variação do iBeacon. O Evothings Viewer vem com vários plugins [pré-instalados](https://evothings.com/doc/studio/mobile-app.html#SupportedPlugins). 

Os plugins possuem duas partes, uma implementação de código nativo (geralmente escrita em Objective-C ou Swift no iOS e em Java no Android) e uma biblioteca JavaScript (compartilhada entre plataformas). É possível usar o Evothings Studio sem o Cordova, mas se você deseja criar aplicativos nativos, ele deve ser utilizado.

Um projeto do Evothings é apenas uma pasta com arquivos HTML / JavaScript e outro conteúdo da web. Um projeto do Cordova possui uma estrutura de pastas especial e os arquivos JavaScript / web entram na pasta "www". 

Você pode usar o Cordova apenas, sem usar o Evothings Studio. Mas o fluxo de trabalho será muito mais rápido se você usar o Evothings. Abaixo, os dois fluxos de trabalho.

**Fluxo de trabalho Cordova**

1. Edite seu código (HTML / JS) e salve
2. Compilar o aplicativo (cordova build ios / android)
3. Implantar o aplicativo em um dispositivo (adb install -r caminho para o arquivo apk)
4. Inicie o aplicativo no dispositivo
5. Repita as etapas acima para cada alteração de código

**Fluxo de trabalho de Evothings**

1. Edite seu código (HTML / JS) e salve

2. O aplicativo é recarregado instantaneamente no (s) dispositivo (s)

### Visão geral do download do Evothings Studio

Evothings Studio tem incluso os seguintes itens:

- Aplicativo de desktop do Evothings Workbench
- Aplicativos de exemplo

O Evothings Workbench é executado no mecanismo `nw.js` (que inclui WebKit e node.js). O binário `nw.js` está incluído no download. Todos os pacotes de download (Windows / OS X / Linux) são basicamente idênticos, exceto o binário node-webkit.

Aqui está uma visão geral de alguns dos arquivos e pastas no pacote de download descompactado:

```ASN.1
- examples - aplicativos de exemplo
- hyper - código JavaScript para o Workbench
-- server - código que se comunica com o servidor proxy que encaminha as recargas para o Viewer
-- settings
--- settings.js - configurações que você pode modificar
-- ui - código da interface do usuário
- node_modules - módulos usados pelo node-webkit
- package.json - Configurações do aplicativo Workbench
```



O Evothings Studio oferece várias ferramentas e itens úteis:

- Desenvolva em vários dispositivos móveis simultaneamente - teste seu aplicativo em telefones e tablets iOS e Android ao mesmo tempo
- Execute um aplicativo em todos os dispositivos conectados com um clique
- Ao salvar um arquivo, todos os dispositivos conectados recarregam o aplicativo em execução - você pode ver o resultado instantaneamente
- Liberdade para usar qualquer editor (a atualização ao vivo funciona com todos os editores que salvam dados em arquivos HTML/JS/CSS/mídia, também editores HTML e editores de imagem)
- Comece rapidamente com seus próprios aplicativos, copiando o código dos aplicativos de exemplo (código para exemplos incluídos no download)
- Envie facilmente dados de registro de dispositivos conectados
- Avalie o código JavaScript interativamente em dispositivos conectados, útil para desenvolvimento e depuração
- Crie aplicativos nativos usando o Apache Cordova - não são necessárias ferramentas proprietárias, inclua os plugins do Cordova que você gosta
- Use recarga ao vivo, registro e avaliação de código interativa com qualquer aplicativo Cordova - isso facilita o desenvolvimento e a depuração de aplicativos Cordova
- O [código fonte](https://evothings.com/doc/studio/evothings-studio-overview.html#SourceCode) completo está disponível no GitHub (licença de código aberto Apache)

## Evothings BLE

Este guia mostra como usar a API do Evothings BLE para conectar-se a dispositivos Bluetooth Low Energy a partir do JavaScript. Observe que este guia se aplica ao Evothings Viewer 1.5 ou posterior e ao plug-in Cordova BLE versão 2.0.0 ou posterior (incluído no Evothings Viewer).

Orientamos você nas etapas para detectar e conectar-se a um dispositivo BLE. 

> ☕︎ Você pode usar este guia para basicamente qualquer dispositivo BLE.


O suporte nativo para Bluetooth Low Energy no Android e iOS é fornecido pelo plug-in Cordova BLE. Este plug-in está incluído no Evothings Viewer, que facilita o início do desenvolvimento de um aplicativo BLE em JavaScript. Quando o aplicativo está pronto para teste e implantação, o sistema de compilação Cordova é usado para criar um aplicativo personalizado com o código do aplicativo e o plug-in BLE. 

> ☕︎ Este aplicativo pode ser publicado nas lojas de aplicativos.

### Etapas para conectar-se a um dispositivo BLE

Para conectar-se a um dispositivo BLE e começar a ler/gravar dados, tem-se as seguintes etapas:

1. 🕵🏻‍♂️ Procurar pelo dispositivo 
2. 📡 Conectar-se ao dispositivo
3. 📝 Ler e Gravar Características

> ☕︎ Uma característica é como um comando ou função, é um local que você lê ou escreve para buscar dados ou controlar o dispositivo (ligar ou desligar um LED ou um motor, por exemplo). **Serviços** são coleções de características, agrupam comandos/funções relacionados.

O que você precisa saber para programar um dispositivo BLE são os **UUIDs** dos serviços e **características** que você deseja usar. Essas informações geralmente são encontradas na documentação do fabricante do dispositivo. 

> ☕︎ Os UUIDs serão colocados no código ao fazer chamadas para as funções da biblioteca BLE. 

![img](https://i2.wp.com/randomnerdtutorials.com/wp-content/uploads/2018/06/GATT-BLE-ESP32.png?w=813&ssl=1)

O nível superior da hierarquia é um perfil, composto por um ou mais serviços. Normalmente, um dispositivo BLE contém mais de um serviço. Todo serviço contém pelo menos uma característica ou também pode fazer referência a outros serviços. Um serviço é simplesmente uma coleção de informações, como leituras de sensores, por exemplo. Existem serviços predefinidos para vários tipos de dados definidos pelo SIG (Bluetooth Special Interest Group), como: 

- Nível da bateria
- Pressão arterial
- Freqüência cardíaca
- Escala de peso, etc.

A **característica** sempre pertence a um serviço e é onde os dados reais estão contidos na hierarquia (valor). A característica sempre tem dois atributos: declaração da característica (que fornece metadados sobre os dados) e o valor da característica.

Além disso, o valor da característica pode ser seguido por **descritores**, que expandem ainda mais os metadados contidos na declaração da característica. 

As **propriedades** descrevem como o valor da característica pode ser interagido. Basicamente, contém as operações e procedimentos que podem ser usados com a característica:

- Difusão
- Ler
- Escreva sem resposta
- Escreva
- Notificar
- Indicar
- Gravações assinadas autenticadas
- Propriedades estendidas

Cada serviço, característica e descritor possui um UUID (Universally Unique Identifier). Um UUID é um número exclusivo de 128 bits (16 bytes). Por exemplo:

```
55072829-bc9e-4c53-938a-74a6d4c78776
```

Existem UUIDs reduzidos para todos os tipos, serviços e perfis especificados no SIG (Bluetooth Special Interest Group). Em resumo, o UUID é usado para identificar informações exclusivamente. Por exemplo, ele pode identificar um serviço específico fornecido por um dispositivo Bluetooth.

### Como falar com um dispositivo BLE - serviços e características

Um dispositivo BLE expõe sua interface de comunicação através de serviços e características. Um **serviço** pode ter uma ou mais **características**. Cada **característica** também pode ter um ou mais descritores (os descritores tendem a ser acessados com menos frequência pelo código do aplicativo).

```markdown
A[Serviço] -> B(Característica)
D(Característica) --> C{Descritores}
```

Por exemplo: um **termômetro** habilitado para BLE geralmente possui um serviço de temperatura com uma característica que permite ler a temperatura.

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g73e0xelfjj30bt05vmx9.jpg)

Cada **serviço** e **característica** tem um ID **universalmente exclusivo** (UUID), que são utilizados para configurar a comunicação com o dispositivo BLE a partir do JavaScript. Os UUIDs geralmente são encontrados na documentação do dispositivo fornecida pelo fabricante.

Cada dispositivos BLE pode ter serviços e características diferentes, mas o princípio geral é o mesmo. Alguns dispositivos têm opções para configurá-lo, outros podem não precisar de nenhuma configuração específica. Em alguns dispositivos você lê principalmente dados (como um termômetro), em outros, você grava dados neles (como máquinas controladas remotamente).

Veja um exemplo do **O ESP32** do curso possui os seguintes UUIDs:

```
SERVICE_UUID        "6E400001-B5A3-F393-E0A9-E50E24DCCA9E"
CHARACTERISTIC_UUID_RX "6E400002-B5A3-F393-E0A9-E50E24DCCA9E"
CHARACTERISTIC_UUID_TX "6E400003-B5A3-F393-E0A9-E50E24DCCA9E"
```

Esses UUIDs são usados no código de exemplo mostrado abaixo. Use os UUIDs para os serviços e as características do dispositivo com o qual você está trabalhando no seu código de aplicativo real.

### Debugando no Evothings Studio

Nos exemplos de código abaixo, a função`console.log( )` é usada para imprimir dados de depuração. Para gerar instruções de log no Evothings Workbench, é possível mapear a função `console.log` para `hyper.log`, da seguinte maneira:

```
// Redirect console.log to Evothings Workbench.
if (window.hyper && window.hyper.log) { console.log = hyper.log }
```

Os dados do log são enviados na janela do console no Evothings Workbench. Clique no botão "Console" no ambiente de trabalho para abrir esta janela.

## Criando Aplicações

### Buscar dispositivos BLE

Aqui está um exemplo de código completo. Observe que o arquivo `cordova.js` está incluído no plug-in BLE, esse arquivo não faz parte do código do aplicativo, é fornecido como plug-in no Evothings Viewer.

Abaixo o Código-fonte do arquivo `index.html` e `app.js` (arraste esse arquivo para o Evothings Workbench e clique em RUN para iniciar no Evothings Viewer):

**HTML:** `index.js`

```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, user-scalable=no,
		shrink-to-fit=no, initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0" />

	<title>Buscar BLE</title>

	<style>
		@import 'ui/css/evothings-app.css';

		p.deviceAddress {
			margin: 5px 0px 10px 10px;
			font-size: xx-small;
			font-weight:bold;
		}

		p.deviceName {
			margin: 5px 0px 0px 10px;
			font-weight: bold
		}
		p.deviceRssi{
			color:rebeccapurple;
			padding: 2px;
			text-align: center;
		}

		div.deviceContainer {
			border-radius: 10px;
			border: 1px solid;
			border-color: #CCCCCC;
			overflow: hidden;
			margin: 10px 0px;
		}
	</style>

	<script>
	// Redirect console.log to Evothings Workbench.
	if (window.hyper && window.hyper.log) { console.log = hyper.log }
	</script>
	
</head>

<body ontouchstart=""><!-- ontouchstart="" enables low-delay CSS transitions. -->

	<header>
		<button class="back" onclick="history.back()">
			<img src="ui/images/arrow-left.svg" />
		</button>

		<img class="logotype" src="ui/images/logo.svg" alt="Evothings" />
	</header>

	<h1>Buscador BLE</h1>

	<div id="startView">
		<button class="red wide" onclick="app.startScan()"> Scan </button>
	</div>

	<div id="scanResultView" style="display: none;">
	
	</div>

	<span id="message" style="display: none;">
	</span>

	<script src="cordova.js"></script>
	<script src="libs/evothings/evothings.js"></script>
	<script src="libs/evothings/ui/ui.js"></script>
	<script src="libs/jquery/jquery.js"></script>
	<!-- TODO: Add libraries that you need -->
	<script src="app.js"></script>
</body>
</html>
```



**Javascript:** `app.js`

```javascript
// Iniciar a busca quando o plugin for carregado

document.addEventListener(
    'deviceready',
    function(){ evothings.scriptsLoaded(app.initialize)},
    false
);

var app = {};
var analog_enabled;


app.initialize = function () {
    app.connected = false;
    app.analog_enabled = false;
    app.showMessage('');
}

app.startScan = function(){
    app.disconnect(); 
    app.showMessage('');
    console.log('Scanning started...');
    //lista para dispositivos
    app.devices = {};
    var img = "https://darrenkearney.me/wp-content/uploads/2015/07/hacking_typing1.gif";
    var htmlString = 
    '<img src='+img+' style="display:inline; vertical-align:middle"> ' +
    '<p style="display:inline">   Scanning...</p>';

    $('#scanResultView').append($(htmlString));
    $('#scanResultView').show();
    
    evothings.ble.startScan(onScanSuccess,onScanFailure);

    function onScanSuccess(device) {
        if(device.name != null){
            app.devices[device.address] = device;

            //var service = device.advertisementData.;
          
            console.log('Found:'+ JSON.stringify(device));
            
            
            var htmlString =
				'<div class="deviceContainer">' +
				'<p class="deviceName">' + device.name + '</p>' +
                '<p class="deviceAddress">' + device.address + '</p>' +
                '<p class="deviceRssi">' + device.rssi + '</p>' +
				'</div>';

			$('#scanResultView').append( $( htmlString ) );
        }
    }
    function onScanFailure(errorCode) {
        // Show an error message to the user
		app.disconnect('Failed to scan for devices.');

		// Write debug information to console.
		console.log('Error ' + errorCode);
    }
}

app.disconnect = function(errorMessage){
    if (errorMessage)
	{
		console.log(errorMessage);
	}
    
    // Pare a busca
	evothings.ble.stopScan();
    $('#scanResultView').hide();
	$('#scanResultView').empty();
}

app.showMessage = function(message){
    document.querySelector('#message').innerHTML = message;
    $('#message').show();
    //$('#message').hide();
}
```



## Conectando a um dispositivo BLE

Aqui um segundo exemplo de código completo. Abaixo o Código-fonte do arquivo `index.html` e `app.js` (arraste esse arquivo para o Evothings Workbench e clique em RUN para iniciar no Evothings Viewer):

**HTML:** `index.html`

```HTML
<!DOCTYPE html>
<!--
	
	Baseado no BLE example, com algumas atualizações e correções no código para trabalhar com o código de exemplo do ESP32 para ligar o led padrão na porta 25.

-->
<html>
<head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, user-scalable=no,
		shrink-to-fit=no, initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0" />
	<title>ESP32 BLE</title>

	<style>
		@import 'ui/css/evothings-app.css';
	</style>

	<script>
	// Redirect console.log to Evothings Workbench.
	if (window.hyper && window.hyper.log) { console.log = hyper.log }
	</script>

</head>

<body ontouchstart="">
	
  <header>
		<button class="back" onclick="history.back()">
			<img src="ui/images/arrow-left.svg" />
		</button>
		<img class="logotype" src="ui/images/logo.svg" alt="Evothings" />
	</header>
	
	<img class="evo-image" src="https://cdn.apk-cloud.com/detail/image/io.dabbleapp-w250.png"/>
	<h1>ESP32 BLE</h1>
	<button id="find" class="blue">Find Device</button>
	<p><strong>Status:</strong> <span id="message">Idle</span></p>
	<button id="on" class="green">LED ON</button>
	<button id="off" class="red">LED OFF</button>
	
	<!--
	Incluir o cordova.js automaticamente inclui a biblioteca JavaScript para o plugin Cordova BLE.
	-->
	<script src="cordova.js"></script>
	
	<!--
	Inclui o código da aplicação
	-->
	<script src="app.js"></script>
</body>
</html>

```



**Javascript:** `app.js`

```javascript
// JavaScript code for the Arduino BLE example app.
;(function()
{


var SERVICE_UUID =        		'6E400001-B5A3-F393-E0A9-E50E24DCCA9E'
var CHARACTERISTIC_UUID_RX = 	'6E400002-B5A3-F393-E0A9-E50E24DCCA9E'
var CHARACTERISTIC_UUID_TX = 	'6E400003-B5A3-F393-E0A9-E50E24DCCA9E'


/**
 * The BLE plugin is loaded asynchronously so the ble
 * variable is set in the onDeviceReady handler.
 */
var ble = null;

// Connected device.
var mDevice = null;

var mPollingTimer = null;

var characteristicRead = null;
var characteristicWrite = null;

function btEnable(){
	document.getElementById("on").disabled = false;
	document.getElementById("on").className = 'green';
	document.getElementById("off").disabled = false;
	document.getElementById("off").className = 'red';
}
function btDisable(){
	document.getElementById("on").disabled = true;
	document.getElementById("on").className = 'stone';
	document.getElementById("off").disabled = true;
	document.getElementById("off").className = 'stone';
}
function initialize()
{
	btDisable();

	document.getElementById('find').addEventListener(
		'click',
		findDevice,
		false)
	document.getElementById('on').addEventListener(
		'click',
		on,
		false)
	document.getElementById('off').addEventListener(
		'click',
		off,
		false)

	showMessage('Ready');
	
}

function findDevice()
{
	showMessage('...Finding Device');

	disconnectDevice()

	// Used for debugging/testing.
	scanForDevice();
	return
}

function scanForDevice(){
	showMessage('Scanning device...');

	evothings.ble.startScan(
		onDeviceFound,
		onScanError
	);

	function onDeviceFound(device){
		console.log('Found device: ' + device.name);
		
		if (device.advertisementData.kCBAdvDataLocalName == 'ESP32-SI01'){
			console.log('Found: ' + device.name);

			evothings.ble.stopScan();

			MakeConnection(device);
		}
	}

	function onScanError(){
		console.log('Found device: ' + device.name);
	}
}

function MakeConnection(device){
	showMessage('Connecting to: ' + device.name);
	
	// Save device.
	mDevice = device;
	
	//Biblioteca desatualizada no GTEkViwer
	setTimeout(
		evothings.ble.connectToDevice(
			device,
			onConnected,
			onDisconnected,
			onConnectError
		),
		500
	)

	function onConnected(device){
		console.log('Connected to: ' + device.name);
		getServices(device);
	}

	function onDisconnected(device){
		console.log('Disconnected from: ' + device.name);
	}
	function onConnectError(device){
		console.log('Connect error: ' + device.name);
	}

}

function getServices(device){
	console.log('Getting Services');
	var service = evothings.ble.getService(device, SERVICE_UUID);
	characteristicRead = evothings.ble.getCharacteristic(service,CHARACTERISTIC_UUID_TX);
	characteristicWrite = evothings.ble.getCharacteristic(service,CHARACTERISTIC_UUID_RX);

	if (characteristicRead && characteristicWrite){
		console.log('RX/TX services found.');
		showMessage('READY!');
		btEnable();
	}else{
		showMessage('ERROR: RX/TX services not found!');
		console.log('RX/TX services ERROR.');
	}
}

function disconnectDevice()
{
	evothings.ble.stopScan();
	clearInterval(mPollingTimer);
	if (mDevice) { 
		console.log('Disconnected: ' + mDevice.name);
		evothings.ble.close(mDevice) ;
	}
	mDevice = null;
	btDisable();
	//showMessage('Disconnected');
	
}

function on()
{
	showMessage('ON:');
	writeValue(new TextEncoder("utf-8").encode("1")); 
}

function off()
{
	showMessage('OFF:');
	writeValue(new TextEncoder("utf-8").encode("0"));
}

function writeValue(value){
	evothings.ble.writeCharacteristic(
		mDevice,
		characteristicWrite,
		new Int8Array(value),
		onActivated,
		onActivatedError);
	
	function onActivated()
	{
		console.log('ESP is'+(value==1)?'ON':"OFF");
	}
	
	function onActivatedError(error)
	{
		console.log('ESP32 error: ' + error);
	}
}

function showMessage(text)
{
	document.querySelector('#message').innerHTML = text
	console.log(text)
}

// Start scanning for devices when the plugin has loaded.
document.addEventListener('deviceready', initialize, false)

})(); // End of closure.
```



Código do ESP32

```java
/*
    Based on Neil Kolban example for IDF: https://github.com/nkolban/esp32-snippets/blob/master/cpp_utils/tests/BLE%20Tests/SampleWrite.cpp
    Ported to Arduino ESP32 by Evandro Copercini
*/
#include <BLEDevice.h>
#include <BLEServer.h>
#include <BLEUtils.h>
#include <BLE2902.h>

#include <iostream>
#include <string.h>

// See the following for generating UUIDs:
// https://www.uuidgenerator.net/

#define SERVICE_UUID        "6E400001-B5A3-F393-E0A9-E50E24DCCA9E"
#define CHARACTERISTIC_UUID_RX "6E400002-B5A3-F393-E0A9-E50E24DCCA9E"
#define CHARACTERISTIC_UUID_TX "6E400003-B5A3-F393-E0A9-E50E24DCCA9E"

BLEServer *pServer = NULL;
BLECharacteristic * pTxCharacteristic;

//Variável para controlar o LED
const int LED = 25;

//Variaves BLE
bool _BLEClientConnected = false;
bool oldDeviceConnected = false;
uint8_t txValue = 0;
uint8_t rxValue = 0;


class MyCallbacks: public BLECharacteristicCallbacks {
    void onWrite(BLECharacteristic *pCharacteristic) {
      
      std::string value = pCharacteristic->getValue();
      
      // put your main code here, to run repeatedly:
      if(value.length() == 1){
        if(value.find("1") != -1){
          digitalWrite(LED, HIGH); // ligar led
        }else{
          digitalWrite(LED, LOW); // desligar led
        }
      }
      if (value.length() > 0) {
        Serial.println("*********");
        Serial.print("New value: ");
        
        for (int i = 0; i < value.length(); i++){
          Serial.print(value[i]);
        }
        Serial.println();
        Serial.println("*********");
      }
    }
};



class MyServerCallbacks : public BLEServerCallbacks {
    void onConnect(BLEServer* pServer) {
      _BLEClientConnected = true;
      Serial.println("Client Connected");
    };

    void onDisconnect(BLEServer* pServer) {
      _BLEClientConnected = false;
      Serial.println("Client Disconnected");
    }
};

void InitBLE(){
  BLEDevice::init("ESP32-SI01");
  //BLE Server
  pServer = BLEDevice::createServer();
  pServer->setCallbacks(new MyServerCallbacks());
  
  //BLE Service
  BLEService *pService = pServer->createService(SERVICE_UUID);
  BLECharacteristic *pCharacteristic = pService->createCharacteristic(
                                         CHARACTERISTIC_UUID_RX,
                                         BLECharacteristic::PROPERTY_READ |
                                         BLECharacteristic::PROPERTY_WRITE
                                       );
  pCharacteristic->setCallbacks(new MyCallbacks());
  pCharacteristic->setValue("LED");
  
  //BLE Characteristic
  pTxCharacteristic = pService->createCharacteristic(
										CHARACTERISTIC_UUID_TX,
										BLECharacteristic::PROPERTY_NOTIFY
									);
  pTxCharacteristic->addDescriptor(new BLE2902());
  pService->start();
  BLEAdvertising *pAdvertising = pServer->getAdvertising();
  pAdvertising->start();
}

void setup() {
  Serial.begin(115200);
  pinMode(LED, OUTPUT);
  //Chama a configuração inicial do display
  InitBLE();
}

void loop() {
  delay(500);
  if (_BLEClientConnected) {
        pTxCharacteristic->setValue(&txValue, 1);
        pTxCharacteristic->notify();
        txValue++;
		    delay(10); // bluetooth stack will go into congestion, if too many packets are sent
        showInDisplay();
	}
  
  // disconnecting
    if (!_BLEClientConnected && oldDeviceConnected) {
        delay(500); // give the bluetooth stack the chance to get things ready
        pServer->startAdvertising(); // restart advertising
        Serial.println("start advertising");
        oldDeviceConnected = _BLEClientConnected;
    }
    // connecting
    if (_BLEClientConnected && !oldDeviceConnected) {
		// do stuff here on connecting
        oldDeviceConnected = _BLEClientConnected;
    }
}

```



## Extras - informações sobre as funções



#### Procurando por nome e serviço UUID

O primeiro passo ao se comunicar com qualquer dispositivo BLE é estabelecer uma conexão com ele e, para isso, primeiro você precisa encontrar o dispositivo. Esta etapa é chamada de escaneamento. Ao procurar dispositivos, você terá todos os dispositivos BLE dentro do alcance. Isso significa que você deve descobrir de alguma forma a qual dispositivo você deseja se conectar.

Para determinar a identidade de um dispositivo usando o escaneamento, você pode usar vários métodos. Duas maneiras úteis são usar o nome do dispositivo e/ou os UUIDs de serviço anunciados do dispositivo.

Aqui está como encontrar a TI SensorTag CC2650 pelo nome:

```javascript
// Start scanning. Two callback functions are specified.
evothings.ble.startScan(
    onDeviceFound,
    onScanError);

// This function is called when a device is detected, here
// we check if we found the device we are looking for.
function onDeviceFound(device)
{
    if (device.advertisementData.kCBAdvDataLocalName == 'CC2650 SensorTag')
    {
        console.log('Found the TI SensorTag!');
    }
}

// Function called when a scan error occurs.
function onScanError(error)
{
    console.log('Scan error: ' + error);
}
```

Em comparação, veja como encontrar o dispositivo pelo UUID do serviço anunciado :

```javascript
evothings.ble.startScan(
    onDeviceFound,
    onScanError);

// Here we check for a specific service UUID advertised by the device.
function onDeviceFound(device)
{
    // kCBAdvDataServiceUUIDs is an array of strings with service UUIDs.
    var advertisedServiceUUIDs = device.advertisementData.kCBAdvDataServiceUUIDs;
    if (advertisedServiceUUIDs.indexOf('0000aa10-0000-1000-8000-00805f9b34fb') > -1)
    {
        console.log('Found the TI SensorTag!');
    }
}
```

Você também pode especificar o UUID de serviço no parâmetro `options` para startScan. Isso instruirá o sistema BLE nativo a relatar apenas dispositivos que anunciam o UUID de serviço fornecido:

```javascript
// The callback function onDeviceFound will be called only for devices
// that advertise the given service UUID.
evothings.ble.startScan(
    onDeviceFound,
    onScanError,
    { serviceUUIDs: ['0000aa10-0000-1000-8000-00805f9b34fb'] });

function onDeviceFound(device)
{
    console.log('Found the TI SensorTag!');
}
```



### Seleção do disposito através de uma lista

Para selecionar a qual dispositivo se conectar é importante exibir uma lista com os dispositivos e seus nomes. Dessa forma, o usuário do aplicativo pode selecione manualmente um dispositivo. 

> ☕︎ A lista pode ser construída dinamicamente durante o escanemanto, sendo atualizada e classificada por informações como a distância ou valor do RSSI.

### Seleção do dispositivo pelos dados do anúncio

Os UUIDs de serviço anunciado (**kCBAdvDataServiceUUIDs**) usados acima fazem parte dos dados do anúncio do BLE. Este é um bloco de bytes que é transmitido por um dispositivo BLE quando está no modo de anúncio. É importante consultar a documentação dos dados do anúncio para obter uma lista dos campos disponíveis (esses campos podem estar indefinidos ou vazios, dependendo do dispositivo BLE).

Em alguns casos um dispositivo não pode ser identificado exclusivamente por seu nome e/ou UUIDs de serviço anunciados. Dependendo do dispositivo, pode haver outros dados no anúncio que possam ser usados para identificá-lo. Os sinalizadores de Eddystone, por exemplo, transmitem IDs e URLs como parte dos dados do anúncio.

Aqui está como gerar uma representação imprimível da estrutura de dados do anúncio:

```javascript
function onDeviceFound(device)
{
    console.log('Found device:' + JSON.stringify(device.advertisementData));
}
You can also print the entire device structure:

function onDeviceFound(device)
{
    console.log('Found device:' + JSON.stringify(device));
}
```

### Conectando-se a um dispositivo

Quando o dispositivo for encontrado, o próximo passo é conectar-se a ele. Normalmente, a verificação está agora parada e a função de conexão é chamada. Aqui está um exemplo:

```javascript
evothings.ble.startScan(
    onDeviceFound,
    onScanError);

// This function is called when a device is detected, here
// we check if we found the device we are looking for.
function onDeviceFound(device)
{
    if (device.advertisementData.kCBAdvDataLocalName == 'CC2650 SensorTag')
    {
        // Stop scanning.
        evothings.ble.stopScan();

        // Connect.
        evothings.ble.connectToDevice(
            device,
            onConnected,
            onDisconnected,
            onConnectError);
    }
}

// Called when device is connected.
function onConnected(device)
{
    console.log('Connected to device');
}

// Called if device disconnects.
function onDisconnected(device)
{
    console.log('Disconnected from device');
}

// Called when a connect error occurs.
function onConnectError(error)
{
    console.log('Connect error: ' + error);
}
```

Por padrão, a função `evothings.ble.connectToDevice` lê todos os serviços, características e descritores do dispositivo. Opcionalmente, você pode especificar os serviços a serem lidos (a leitura apenas dos serviços necessários pode melhorar o desempenho):

```javascript
evothings.ble.connectToDevice(
    device,
    onConnected,
    onDisconnected,
    onConnectError)
    { serviceUUIDs: ['f000aa70-0451-4000-b000-000000000000'] })
```

### Lendo e gravando características

As características são como comandos ou funções, elas podem ser lidas para obter dados ou escritas para controlar algum aspecto de um dispositivo. Por exemplo, no TI SensorTag, você liga e desliga um sensor gravando em uma característica. Quando o sensor está ligado, você pode ler dados de outra característica. Ambas as características fazem parte do mesmo serviço.

Use as funções `evothings.ble.getService` e `evothings.ble.getCharacteristic` para obter a característica que você deseja ler e escrever. Para ler e escrever descritores, use a função `evothings.ble.getDescriptor` para fazer com que o descritor escreva/leia.

Aqui está um exemplo de como gravar e ler uma característica:

```javascript
// UUID of service.
var BLE_SERVICE = 'f000aa70-0451-4000-b000-000000000000'

// UUID of config characteristic (write 1 to turn sensor ON, 0 to turn OFF).
var BLE_CONFIG = 'f000aa72-0451-4000-b000-000000000000'

// UUID of data characteristic.
var BLE_DATA = 'f000aa71-0451-4000-b000-000000000000'

// Get service and characteristics.
var service = evothings.ble.getService(device, BLE_SERVICE)
var configCharacteristic = evothings.ble.getCharacteristic(service, BLE_CONFIG)
var dataCharacteristic = evothings.ble.getCharacteristic(service, BLE_DATA)

// Write a charateristic.
evothings.ble.writeCharacteristic(
    device,
    configCharacteristic,
    new Uint8Array([1]), //new TextEncoder("utf-8").encode("1")
    onCharacteristicActivated,
    onCharacteristicActivatedError)

function onCharacteristicActivated()
{
    console.log('Characteristic is ON')

    // Enable notifications from the Luxometer.
    evothings.ble.readCharacteristic(
        device,
        dataCharacteristic,
        onCharacteristicRead,
        onCharacteristicReadError)
}

function onCharacteristicActivatedError(error)
{
    console.log('Characteristic activate error: ' + error)
}

function onCharacteristicRead(data)
{
    // Get raw sensor value (data buffer has little endian format).
    var raw = new DataView(data).getUint16(0, true)
    console.log('Raw Characteristic value: ' + raw)
}

function onCharacteristicReadError(error)
{
    console.log('Read Characteristic error: ' + error)
}
```



### Usando notificações para ler dados

É comum que um aplicativo precise ler continuamente dados de um dispositivo BLE. Os exemplos incluem a **leitura** de um sensor e o **envio** de dados para a nuvem ou o uso do acelerômetro de um dispositivo sensor para controlar um jogo no celular.

As **notificações** são uma maneira eficiente de ler dados continuamente de um dispositivo BLE. O processo é semelhante à leitura de dados, a principal diferença é que a função de retorno de chamada será chamada repetidamente até que a notificação seja desativada.

Aqui está um exemplo de código de como habilitar e manipular notificações:

```javascript
function onCharacteristicActivated()
{
    console.log('Characteristic is ON')

    // Enable notifications from the Luxometer.
    evothings.ble.enableNotification(
        device,
        dataCharacteristic,
        onCharacteristicNotification,
        onCharacteristicNotificationError)
}

// Called repeatedly until disableNotification is called.
function onCharacteristicNotification(data)
{
    console.log('Characteristic value: ' + data)
}

function onCharacteristicNotificationError(error)
{
    console.log('Characteristic notification error: ' + error)
}
```



## Aplicações de Exemplo

- Localizar Objetos BLE - Criar uma aplicação para ler a intensidade do RSSI e conforme reduz a distância mais o led pisca na tela (blink) do aplicativo.
- https://evothings.com/how-to-connect-your-phone-to-your-esp8266-module/ (ESP8266 WiFi)
- https://evothings.com/diy-arduino-beacons/ (Fazer com ESP32I)
- Pensar em uma aplicação apenas para trocar dados entre celulares
  - Beacon Chat
- https://evothings.com/arduino-ble-quick-walk-through/

## Problemas com Codificação

Ao escrever a característica o valor passado não estava sendo recebido com a codificação correta pelo ESP. Abaixo são descritas duas formas, uma que funciona para a versão do GTekViewer, que roda no iOS, e outra para o Evothings Viewer, que roda no android.

Para Android:

```javascript
writeValue(new TextEncoder("utf-8").encode("0"));
```

Para iOS:

```javascript
app.toUTF8Array = function(str) {
    var utf8 = [];
    for (var i=0; i < str.length; i++) {
        var charcode = str.charCodeAt(i);
        if (charcode < 0x80) utf8.push(charcode);
        else if (charcode < 0x800) {
            utf8.push(0xc0 | (charcode >> 6), 
                      0x80 | (charcode & 0x3f));
        }
        else if (charcode < 0xd800 || charcode >= 0xe000) {
            utf8.push(0xe0 | (charcode >> 12), 
                      0x80 | ((charcode>>6) & 0x3f), 
                      0x80 | (charcode & 0x3f));
        }
        // surrogate pair
        else {
            i++;
            charcode = ((charcode&0x3ff)<<10)|(str.charCodeAt(i)&0x3ff)
            utf8.push(0xf0 | (charcode >>18), 
                      0x80 | ((charcode>>12) & 0x3f), 
                      0x80 | ((charcode>>6) & 0x3f), 
                      0x80 | (charcode & 0x3f));
        }
    }
    return utf8;
};

var data = app.toUTF8Array("1");
    app.device && app.device.writeDataArray(new Uint8Array([data]), '6E400002-B5A3-F393-E0A9-E50E24DCCA9E');
```

## Referências

https://evothings.com/doc/build/build-overview.html

https://evothings.com/doc/build/cordova-guide.html#SummaryOfBuildSteps

https://evothings.com/doc/starter-guides/cordova-starter-guide.html