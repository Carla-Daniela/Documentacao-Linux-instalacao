<img style="width:70px; height:70px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" /><img style="width:70px; height:70px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/oracle/oracle-original.svg" />
                    
# Documentação sobre a instalação do Oracle Linux versão 8.7

<h2>Instalações</h2>

<ul>
<h4><li>Instale o VirtualBox para criar uma máquina virtual: https://www.virtualbox.org/</li></h4>
<h4><li>Instale a Iso do oracle linux 8.7: https://yum.oracle.com/oracle-linux-isos.html</li></h4>
</ul>

<h2>Configurando a máquina</h2>
<ul>
<h4><li>1. Abra o virtualbox selecione a opção máquina > novo</li></h4>
<h4><li>2. Escolha o nome que desejar para a sua máquina e no tipo coloque LINUX</li></h4>
<h4><li>3. Defina quantos MB e quantas CPUs terá sua máquina: pode ser 4MB e 1 CPU por padrão</li></h4>
<h4><li>4. Selecione criar um disco rígido virtual agora e coloque 30GB de memória, deixe a caixa pré-alocar desmarcada</li></h4>
<h4><li>5. Finalize</li></h4>
<h4><li>6. Entre nas configurações da sua máquina</li></h4>
<h4><li>7. Selecione Armazenamento > Controladora IDE > vazio > em drive óptico selecione o ícone do disco > escolher uma imagem > selecione a Iso 8.7 que baixamos</li></h4>
<h4><li>8. Vá em rede e troque a placa de Nat por modo bridge</li></h4>
<h4><li>9. Habilite uma segunda placa de rede e coloque como interna</li></h4>
<h4><li>10. Inicie a máquina</li></h4>
</ul>

<h2>Configurando o ambiente</h2>
<ul>
<h4><li>1. Selecione Install Oracle Linux 8.7</li></h4>
<h4><li>2. Selecione o idioma e next, por padrão é recomendado o inglês, pois é o mais utilizado em ambiente de desenvolvimento</li></h4>
<h4><li>3. Selecione installation destination > selecione o disco de 30GB > done </li></h4>
<h4><li>4. Selecione Network & Host Name > ative a placa de rede enp0s3 > done </li></h4>
<h4><li>5. Selecione caso desejar, selecione o keyboard e configure para português > done</li></h4>
<h4><li>6. Selecione Root Password e escolha um senha para seu usuário root > done</li></h4>
<h4><li>7. Selecione Create User e escolha um nome e uma senha para o usuário comum > done</li></h4>
<h4><li>8. Finalize a configuração em Begin installation</li>
</ul>

<h2>Desativando interface gráfica</h2>
<ul>
<h4>Após a instalação entre com seu usuário e execute no terminal esses comandos:</h4>
<h4><li>systemctl set-default multi-user.target</li></h4>
<h4><li>systemctl reboot</li></h4>
</ul>

## Pronto para uso! 
