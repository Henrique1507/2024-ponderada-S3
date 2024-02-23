# Atividade Ponderada - Semana 03 - Henrique Ottoboni

## Introdução:

Criação de uma instância de máquina EC2 e acesso da máquina com SSH utilizando PuTTy.

## Objetivo:

O objetivo deste documento é mostrar de maneira simplificada e intuitiva a criação de uma instância EC2 e conectá-la utilizando SSH por meio do PuTTy, isto é, um software que permite criar conexões com servidores de maneira remota.

## Materiais:

Os materiais necessários para a realização desta atividade são: acesso à uma conta na AWS para a criação de uma instância EC2 e a instalação do software PuTTy.

## Método:

### 1. Criação do par de chaves

Nesta primeira etapa, após acessar a tela inicial e migrar para a EC2, devemos executar uma instância e iniciar sua configuração. Neste momento, o primeiro passo é criar um par de chaves para que possamos conectar com segurança à instância posteriormente. No exemplo abaixo, foi utilizado como chave "Atividade-ponderada-key", que será usada novamente após algumas etapas. Além disso, é importante selecionar o tipo ".ppk" para conseguir acessar o SSH por meio do puTTy.

<img src='./img/imagem 1.png'>

### 2. Adição do grupo de segurança

A fim de aumentar a segurança, foi adicionado um grupo de segurança chamado "PonderadaS3-sg". Após isso, pode criar a instância seguindo todas as outras configurações padrões.

<img src='./img/imagem 2.png'>

### 3. Instância criada

Após o término da configuração da criação da instância, podemos acessá-la na página inicial. Nela, é observado alguns pontos que serão essenciais, como o nome da instância, o endereço IP, o nome do grupo de segurança e o par de chaves criados e, por fim, a data de lançamento da instância.

<img src='./img/imagem 3.png'>
<img src='./img/imagem 4.png'>

### 4. Utilização do PuTTy

Após a instância criada e observado seus dados, abriremos o PuTTy no computador e logo adicionaremos o endereço IP logo no primeiro campo, que está em evidência. 

<img src='./img/imagem 5.png'>

Em seguida, devemos ir no campo "Auth" e selecionar por "Credentials", para que então possamos utilizar a chave de segurança criada. Para fazer isso, basta selecionar o primeiro campo "Browse..." e encontrar pela chave criada nas pastas do seu computador. Abaixo, a representação de como deve ser.

<img src='./img/imagem 6.png'>

 Vale destacar que essa é a última etapa, ou seja, o último método utilizado. Após isso, teremos o resultado que desejamos.

 