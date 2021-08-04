# Aumentando capacidade do HD no Virtual Box com o Sistema Operacional já instalado

Aumentar área de armazenamento de um hd com o sistema operacional instalado
Aqui está o código a ser utilizado na ação de aumentar a capacidade de seu HD, ja com o Sistema operacional instalado.
Tem dúvida?, confira o video: 

#REQUISITOS#

1- Ter o caminho de instalação do VirtualBox. No meu caso foi: 
# C:\Program Files\Oracle\VirtualBox 

2- Ter o caminho da maquina virtual a ser alterada
# C:\Users\Everton\VirtualBox VMs\Win10\Win10.vdi 

3- Acessar o CMD do Windows

4- Entrar com o comando CD e colar o endereço que copiou no passo 1

5- Entrar com o comando
##vboxmanage modifyhd##

6- Coloque "aspas duplas", após ter digitado o item 5

7- Entre com a linha que copiou no passo 2, e coloque as aspas no final, que ficara:
C:\Program Files\Oracle\VirtualBox\vboxmanage modifyhd "C:\Users\Everton\VirtualBox VMs\Win10\Win10.vdi"

8- Digite no final do passo7:
Deixe um espaço e coloque --resize 30000
Obs.: Esse valor corresponde a 30GB.

9-Linha completa ficará:
C:\Program Files\Oracle\VirtualBox\vboxmanage modifyhd "C:\Users\Everton\VirtualBox VMs\Win10\Win10.vdi" --resize 30000

10- Pressione ###ENTER###
        
11- A saída deverá ser:
0% ...10%...20%...30%...40%...50%...60%...70%...80%...90%...100%

12- Acessa maquina virtual
13- Pressione CTRL + ESC, digite 'Ferramentas adimistrativas'
14- Entre em Gerenciamento do Computador
15- Entre em Gerenciamento de Disco
16- Clique com botao direito na Unidade a aumentar
17- Opção: Estender volume...avançar...defina um valor que se mostra e concluir.
        
Obs.: Entendo ser util acompanhar pelo vídeo.

Video explicativo: https://youtu.be/rLNIyRXP9u0
        
        Sucesso!!!
