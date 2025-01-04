# ERC20
Token ERC20


En la linea

uint public totalSupply = 10000 * 10 ** 18;

Decidir cuantas unidades totales del token existirán, en esta ocasión vamos a dejarlo por default (si quieres agregar más no uses puntos ni comas, solo agrega o quita ceros)

Agregar el nombre de tu token entre las comillas en

string public name = "Nombre de token";
Ejemplo: string public name = "QABlockchain";

Agregar símbolo del token en mayúscula en

string public symbol = "SIMBOLO";
Ejemplo:
string public symbol = "QAB";


# Crear tu contrato
Ir a Remix
Click en contracts > Create new file (la hojita)
Ingresar nombre y enter
Pegar el código (recuerda editar las variables)

# Compilar tu código
Clickea ‘Compilar’ (tercera opción del menú)
Asegúrate de elegir la misma versión de Solidity que estamos usando en el código, en este caso 0.8.2

Click en ‘Compile’ 
Click en ‘Deploy’ (4ta opcion)
Seleccionar el enviroment » Injected Provider – Metamask «

Selecciona deploy
Se abrirá metamask y te mostrará el costo de la transacción en ETh de test. 
El costo que se muestra de gas por lo general es bastante similar al real en producción. 

Confirmar la transacción y quedará listada para procesarse 

# Hacer visible el contrato
Desplegar las opciones ‘Deployed Contracts’
En la opción ‘transfer’ peguemos nuestra dirección de metamask seguido de ‘,1’ 
El 1 puede ser 10, 100, 1000 o la cantidad que quieras menor al total de tokens que declaraste en el contrato y múltiplo de 10. 
Ejemplo: 0x6a0c2f0370cbE44C82ebfE368a8E2443d95E4d52,1

Seleccionamos la flecha de ‘transfer’ > ‘transact’ > confirmar la transacción en metamask

# Ver mis tokens en la blockchain
Ir a https://goerli.etherscan.io/
Pegar tu numero de wallet en el buscador
Ir a la pestaña ‘Erc20 Token Txns’
Click en la opción ‘Token’ y podrás ver en el menú la cantidad de token que enviaste.
