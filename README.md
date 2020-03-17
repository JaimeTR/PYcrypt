# PYcrypt

- PYcrypt es un crypter polimórfico 'python backdoors' escrito en python por JaimeTR. La salida es completamente indetectable.

- PYcrypt puede inyectar archivos maliciosos de python en un archivo normal con sistema de subprocesos múltiples.

- Ejecútelo con los permisos de superusuario.

- La salida de PYcrypt es completamente indetectable.

Módulo de encriptación

![Alt text](https://image.ibb.co/jO9mdd/Encryption_Module.png "Encryption Module ")


# Uso :

 - sudo  ./PYcrypt.py --file=backdoor.py --output=output_backdoor.py # encrypt backdoor.py and output file is output_backdoor.py
 - sudo ./PYcrypt.py --file=shell.py # encrypt shell.py and default output file  is backdoor.py but you can edit it in source code
 - sudo ./PYcrypt.py --help # PYcrypt help
 - sudo ./PYcrypt.py --backdoor-file=payload.py --file=test.py --output=hacked.py # inject payload.py with  test.py into hacked.py with multi-threading system

 # Como funciona?

 * Encryption module :

 - PYcrypt add some junkcode .
 - PYcrypt use a python internal module 'py_compile' who compile the code into bytecode to a .pyc file .
 - PYcrypt convert .pyc file into normal .py file .
 - And in this way we can obfuscate the code
 - The md5sum will change too

* Injection  module :

- it inject a malicious python file  into a normal file with multi-threading system .


## Sistemas Operativos recomendados para iniciar:
- Kali Linux
- Cyborg
- Parrot
- BackTrack
- Backbox
- Dracos

### Donar!
AYUDAME A SEGUIR TRABAJANDO [Donar](https://www.paypal.me/jaimetarazona).

### PAYPAL

[https://www.paypal.me/jaimetarazona](https://www.paypal.me/jaimetarazona).


### GRACIAS

JaimeTR hecho con ❤️
