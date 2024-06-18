# cifra-de-cesar-simples

```
def crifra():
    key = int(input('digite o numero da chave (entre 1 e 31) >>>'))
    texto = input('Digite o texto que deseja criptografar >>>')
    new_text = ''
    for letra in texto:
        if letra == ' ':
            new_text += ' '
        else:
            new_text += chr(ord(letra) + key)
    
    return new_text

def descifra(texto_cifrado):
    key = int(input('digite o numero da chave (entre 1 e 31) >>>'))
    new_text = ''
    
    for letra in texto_cifrado:
        if letra == ' ':
            new_text += ' '
        else:
            new_text += chr(ord(letra) - key)
    
    return new_text

text = crifra()
print(f'texto cifrado >>> {text}')
print('texto decifrado >>>', descifra(text))
```
