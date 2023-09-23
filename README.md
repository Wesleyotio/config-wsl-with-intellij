# Configurando WSL2 com Intellij

Neste breve tutorial faremos uma configuração para instalação da IDE [Intellij](https://www.jetbrains.com) no WSL2 usando o [Ubuntu-20.04](https://ubuntu.com/wsl), caso nunca tenha feito a instalação desta distro no seu WSL2 minha sugestão é começar [Configurando o WSL com o Ubuntu](https://github.com/Wesleyotio/config-wsl-with-ubuntu-zsh).

Depois de ter realizado a configuração mencionada estaremos prontos para dar inicio a esta, importante também enfatizar que esse tutorial foi inspirado pelo video [instalando o Intellij dentro do wsl2](https://www.youtube.com/watch?v=v-e8MRhNkmU) do canal [CodaRAM](https://www.youtube.com/@codaram).

# Índice

- [Configurando WSL2 com Intellij](#configurando-wsl2-com-intellij)
- [Índice](#índice)
- [Instalando uma interface gráfica no WSL](#instalando-uma-interface-gráfica-no-wsl)
- [Instalando a IDE pelo JetBrains Toolbox App](#instalando-a-ide-pelo-jetbrains-toolbox-app)

# Instalando uma interface gráfica no WSL

Sim, meu camarada é possível instalar uma interface gráfica para seu WSL2, fazemos isto rodando o comando.

```sh
sudo apt install nautilus -y
```
# Instalando a IDE pelo JetBrains Toolbox App

Basicamente vamos baixar o [toolbox APP](https://www.jetbrains.com/toolbox-app/) e fazer a instalação no WSL2, o interessante aqui é que você pode ter todas a ferramentas deles dentro do WSl, mas neste caso estamos focados no [JAVA](https://www.java.com), com já citado a ferramenta vai ficar instalada dentro do WSL então baixe o arquivo da extensão **.tar.gz** usando sua interface do windows encontre o diretório da distro.

![Image](tela-diretorio-1.png)  

Dentro do diretório da distro jogue onde quiser o arquivo, lembre que depois de descompactado e instalado ele não terá mais utilidade.

```sh
sudo tar -xzf <nome-do-arquivo>.tar.gz -C /opt
```

Feito isso agora temos o arquivo descompactado na pasta `/opt` navegue até esta pasta e encontre o diretório **com mesmo nome do arquivo** descompactado

```sh
cd /opt

cd <nome-do-arquivo>
```

Neste diretório roda o comando para iniciar a instalação de fato do tool box

```sh
./jetbrains-toolbox
```
Se tudo estiver saindo como o esperado teremos a seguinte tela
![Image]()  