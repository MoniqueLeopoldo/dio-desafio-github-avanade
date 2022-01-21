**GIT**

**GIT** não tem interface gráfica, ele é um CE Line Interface (linha de comando), diferente do Grafic Usuer Interface.

**Windows - SHA1** (Secure Hash Algorithm) – (Algoritmo de Hash seguro), é um conjunto de funções Hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA) A encriptação gera conjunto de caracteres identificador de 40 dígitos. (É único e serve como identificação), toda vez que eu mudar algo gera novos dígitos.

- Objetivos fundamentais: Responsáveis pelo versionamento dos códigosBlobs (onde os arquivos ficam guardados, contém meta dados dentro dele dos arquivos), (tipo, tamanho, barra contrário com 0 e o conteúdo do arquivo), (tem o SHA1 dos arquivos).

**Trees** (Armazenam blobs, também contém meta dados, e guarda o nome do arquivo), (apontam os caminhos), (tem o SHA1 dela). Elas apontam para arvores e bolhas.

**Commits** (Junta tudo). Aponta para uma árvore, para um parente, aponta para um último antes dele, autor, mensagem, carimbo de tempo (data e hora de criação). Também tem SHA1 dele. (Único para cada autor). Sistema distribuído seguro Guarda a mesma versão em todas as máquinas.**

**Comandos:**

**“-a” mostra arquivos ocultos.**

**“ls” mostra os arquivos que estão dentro da pasta.**

**“dir” lista o todas as pastas (diretórios) dentro do terminal.**

**“cltr + l” limpa os comando que digitamos.**

**“cd + nome da pasta” entra dentro da pastas.**

**“cd ..” sobe um nível acima.**

**“mkdir” cria pasta.**

**“del + nome da pasta” apagar tudo que está dentro da pasta.**

**“rmdir” apaga a pasta.**

**“letra inicial + TAB” ele reconhece que existe um pasta com a inicia dentro dela e auto preenche .**

**“>” (para jogar informação dentro de alguma pasta) se a pasta não existir ele cria. (colocar .txt no final do nome da pasta).**

**“echo > nome do aquivo.md**

**” cria arquivo. (não rastreáveis, não visíveis)**

**“mv nome da pastas.md ./nome da pasta para onde queremos mover/” mover pastas.**

**“git init” iniciar o GIT**

**“git commit” criar um commit. **

**“git commit –m “digitar a mensagem que esse commit irá carregar”” **

**criar um commit com mensagem (melhor). **

**Retorna com o início o SHA1 e mais algumas informações**

**![img](https://lh3.googleusercontent.com/GFMiDPpreXpidwUBDQyHn6p6sq673siQtZ1mptjSeTl72WxC1GGbzfCQVAspgKCtQPEFASfKrKW2dqs2scW_-FVvda5mprQjjtrU_PvJ9c051GWGkrbxk3Q9pS0Ul-vI424FIb4B)**

**“git status” mostrar o status dos arquivos que estão dentro dele.**

**“git add” iniciar o versionamento (adiciona o arquivo para ser comitado.), alterou o arquivo para status stargign.**

**“git add \*” iniciar o versionamento (adiciona o arquivo para ser comitado.), alterou todos os arquivos (que estavam na área de trabalho) para status stargign. **

**“git add/rm” para mover o arquivo para untraked.**

**“git clone (endereço URL copiado)” clonar um repositório do GitHub **

**“git config --global user.email (e-mail)” cadastrar e-mail.**

**“git config --global user.name (nome)” cadastrar nome.**

**“git config --global --unset user.email” apagar o e-mail cadastrado.**

**“git config --global --unset user.name (nome)” apagar o nome cadastrado.**

**![img](https://lh6.googleusercontent.com/67Uk2XW2yE1yIYR5WviTJPR1A4VYeaeauY-R9zBPQIeW2_pRniHwk2-1qbH_GtjYBQvFMhks2VFXMKiOJ6HcE5u-1d5OAQgLlcFEdQNumeMSakQHjkpk2tVq3bxMTUjw7evsqCTV)**

**“git remote add origin (links do github”) para criar um repositório remoto.**

**“git remote -v” passa a lista de servidores remotos.**

**“git push origin master” vai empurrar o meu git do servidor local para o servidor remoto.Username: MoniqueLeopoldo Senha:Moo&F.....**

**![img](https://lh3.googleusercontent.com/4wVQfQJLtZhhtXXyUnJ4eMv4IkPCfIFWXpJ7OBOxF26OCv8B5QFPHkgk1NFUiJrddwTup4R7L6r0aXNEYTQ3pCUsg5yTdxRetC88WBJ1gtJg3MQv3uacWJ4PrzokS8IRQqGigzpg)  **

****Ciclo de vida dos arquivos dentro do GITGIT INIT (criar a pastas .git e inicializa um repositório) ****

**Untraked ou TrackedUntraked** (não temos ciência deles) Cria o arquivo Git e o prepara para edição Tracked (rastreados de fato de GIT, temos ciência deles) 

**Unmodified –** Arquivo que ainda não foi modificado 

**Modified –** Arquivo Unmodified que sofreram modificações****

**Staged –** Arquivos que estão se preparando para fazer parte de um outro tipo de agrupamentoQuando damos a eles informações eles passam a ser um commit e o commit retorna todos esses arquivos para Unmodified aguardando novas informações

**Unmodified –** Se temos esse arquivo e deletamos ele antes de fazer qualquer alteração ele vai para Untraked Servidor Remote Repository (meu GITHUB) Ambiente de desenvolvimento Working directory (repositório de trabalho, pasta receitas) 🡩 arquivos ficam transitando 🡫 Staging area (os arquivos ficam rodando entre essa área e a working)

**Local Repository** (quando fazemos um commit ele passa a integrar meu repositório local e pode ser empurrado para um repositório remoto)

**1 –** Quando você adiciona um arquivo que era untraked (não modificado) e dá um GIT eg ele é movido para o Staging e um modificado também vai para o staging.

**2 –** O arquivo também transita entre a staging área e o local repositor quando você commita eles, porque o local repositor é feito somente de commits que você fez entrar em cena. Caso você não comita eles, você não consegue manda-lós para um repositório remoto. 

**Conflitos no GitHub**: Para alguém contribuir com o meu código, o arquivo inicial é clonado na máquina da pessoa.Quando alguém editar a mesma linha do arquivo que estou editando e empurra primeiro para o GitHub, o site vai me informar isso, porque o código que está no GitHub é o mais atual (porque o meu commit informa a data). Então é preciso baixar o conteúdo atual que está no servidor remoto, juntar com as suas alterações dar o push novamente no remoto. Esse é o conflito Marsh, quando o GitHub tentar juntar esses dois arquivos, então ele te dá a opção de abrir o arquivo e corrigir manualmente a linha e push novamente no servidor remoto.

**Erro Marsh:**

**![img](https://lh5.googleusercontent.com/Qc30akVdMsH0MEAxdoeByirnzkMJ10UA_8DmjkYRz8Avo7dBNKfjbdzc_miBoKZ4QdM8iJP3uu2X09faAV7jfAzacphUAERzNKZ7Ocm1N5gnF_CEm3Pp7WrLFX60w95gmFX_FFoz)**

**Puxar o GitHub “git pull origin master” vai puxar o que está no meu GitHub para o servidor local.**

**A alteração diferente fica abaixo dos símbolos ============Mensagem pós alteração:**

**![img](https://lh3.googleusercontent.com/5jMz8o2jzS8BLY4il5Q_d-gyqIyVXg07_RHMVgRwRoFSCg2td22coKnzkkyt4-O34DRUkdTehXNQO7nAp7kAJkyqtFFa9jyVCCbXPmSwVtVdBOK9qE0T1jgeU7Gu8odAJW5NidzP)**



**Como baixar (clonar) um repositório do servidor remoto GitHub para o repositório local GitCopiar a URL na opção “Code”**

![img](https://lh6.googleusercontent.com/hobgT3iloQUn0vil2gxV6V37kKu1gZ2o4idDZ5V0X4oE_Zu_BD3UXakWGpV6330oBL3Z_zz6ucBJZ9_EpRtO6Y0aNocVEb1SwLCELvHIgTI_vljLhyxeXrPGLM1v1LSEwQwMfTAq)

**E no Git:Dentro da pastas desejada inserir “git clone (endereço URL copiado)**

![img](https://lh4.googleusercontent.com/uhWqusH7bFrNf3i4qkmsVh9mTidbc15YohCVeGbkM6NJxhUVAqV8bcB37BYswvaK_JmOTKxgdFjgdxP4iLOZK5wZCUiT-rUMLHBNmsnf1MDVXJ0HpmvKUuS6hqRu26uDt5Q9G04q)

**Abrindo a pasta (“cd”) baixada e verificando seu repositório (“ls”):**

![img](https://lh3.googleusercontent.com/i4Ti6OzB1dM7t4GpC6KR_-RGmhA308OzWPqBjawKPa8lyHa2ND9kp3x58z_-tN8R5a8LwULSOnTPVfSb2DbeUMxUjRK8RiTHR6jfAgIvTCSAbwhhqjz8Gcr6iY3LogwhNppHwCyt)

**Verificando o repositório oculto “ls –a”:**

![img](https://lh5.googleusercontent.com/caRtLoOwry4ddRkMX9oLIcNIBV95z9vB65u_YVovewMhe59c-tMNk8W8n-3_JoSfVFV0GYRRf8KIjL3VhamRT_N4zzOlX3RgupY5X2pFXtOL7MOKm7XexbyAqvbhcDZNFtmbSo_m)

** Passos de envio... 1- git add . ou -a // 2- git commit -m (para criar arquivo com comentário) // 3- git push origin main // 
