# Ejercicios de protocolos criptográficos

- Info: `code`

# Tareas a realizar

## 1\. Generad un archivo sharedDSA.pem que contenga los parametros. Mostrad los valores.

## 2\. Generad cada uno de vosotros una clave para los parámetros anteriores. La clave se almacenará en nombreDSAkey.pem y no es necesario protegerla por contraseña.

## 3\. "Extraed" la clave privada contenida en el archivo nombreDSAkey.pem a otro archivo que tenga por nombre nombreDSApriv.pem . Este archivo deberá estar protegido por contraseña. Mostrad sus valores.

## 4\. Extraed en nombreDSApub.pem la clave pública contenida en el archivo nombreDSAkey.pem . De nuevo nombreDSApub.pem no debe estar cifrado ni protegido. Mostrad sus valores.

## 5\. Calculad los valores hash del archivo con la clave pública nombreDSApub.pem usando dos funciones hash, sha256 y otra a elegir. Mostrad los valores por salida estándar y guardadlo en nombreDSApub.sha256 y nombreDSApub.[otro].

## 6\. Generad el valor HMAC del archivo sharedDSA.pem con clave '12345' mostrándolo por pantalla.

## 7\. Simulad el protocolo Estación a Estación. Para ello emplearemos como claves para firma/verificación las generadas en esta práctica, y para el protocolo DH emplead las claves asociadas a curvas elípticas de la práctica anterior. Por ejemplo, si mi clave privada está en javierECpriv.pem y la clave pública del otro usuario está en lobilloECpub.pem, el comando para generar la clave derivada será $> openssl pkeyutl -inkey javierECpriv.pem-peerkey lobilloECpub.pem -derive -out key.bin. El algoritmo simétrico a utilizar será AES-128
