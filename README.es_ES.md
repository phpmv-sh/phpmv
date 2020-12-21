# Administrador de versiones de PHP

Traducciones: [English](README.md) - [Castellano](README.es_ES.md)

## Acerca de
phpvm es un administrador de versiones para [PHP](https://www.php.net/downloads.php), dise�ado para ser instalado por 
usuario e invocado por shell, basado en el proyecto [nvm](https://github.com/nvm-sh/nvm). `phpvm` funciona en cualquier
shell compatible con POSIX (sh, dash, ksh, zsh, bash), en particular en estas plataformas: unix, macOS y windows WSL.

<a id="installation-and-update"></a>
<a id="install-script"></a>
## Instalaci�n y actualizaci�n

### Script de instalaci�n y actualizaci�n
Para **instalar** o **actualizar** phpvm, debe ejecutar �l [script de instalaci�n][2]. Para hacer eso, puede descargar 
y ejecutar el script manualmente, o us� el siguiente comando cURL o Wget:
```sh
curl -o- https://raw.githubusercontent.com/phpvm/phpvm.sh/master/install.sh | intento
```
```sh
wget -qO- https://raw.githubusercontent.com/phpvm/phpvm.sh/master/install.sh | intento
```

## Uso
Para instalar una versi�n espec�fica de nodo:
```sh
phpvm install 5.6 # o 7.1, 7.2, 7.3, 7.4, 8.0
```
Para instalar extensiones en una versi�n activa de PHP:
```sh
phpvm agregar xml mbstring pdo # lista de extensiones separadas por espacios
```
Y luego, en cualquier shell nuevo, simplemente use la versi�n instalada:
```sh
phpvm usa 5.6 # o 7.1, 7.2, 7.3, 7.4, 8.0
```

[1]: https://github.com/phpvm/phpvm.sh.git
[2]: https://github.com/phpvm/phpvm.sh/blob/master/install.sh
