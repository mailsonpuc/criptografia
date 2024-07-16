### Criptografa arquivos com aes.

#### criptografa com aes
```bash
openssl enc -aes-256-cbc  -pbkdf2  -salt -in arquivo.txt -out arquivo_criptografado2.enc

```

#### decriptografa
```bash
openssl enc -aes-256-cbc  -pbkdf2 -d -in arquivo_criptografado2.enc -out arquivo_descriptografado2.txt
```

| comando       | explicação                                                                                       |
| ----          | ---                                                                                              |
|-aes-256-cbc   |Especifica o algoritmo AES com uma chave de 256 bits no modo CBC.                                 |
|-pbkdf2        | funções usadas para reduzir a vulnerabilidade a ataques de força bruta.                          |
| -salt         | Adiciona um salt ao processo de criptografia, o que torna os ataques de dicionário mais difíceis.|
|-in arquivo.txt|  Especifica o arquivo de entrada.                                                                |
|-out arquivo_criptografado.enc|Especifica o nome do arquivo de saída criptografado.                               |

---
#### Criptografa com ccrypt
```bash
ccrypt arquivo.txt
```

#### descriptografa 
```bash
ccrypt -d arquivo.txt.cpt
```
