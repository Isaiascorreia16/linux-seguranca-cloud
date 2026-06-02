# Acesso remoto e chaves SSH

## Diferença entre autenticação por palavra-passe e autenticação por chave

Autenticação por palavra-passe: o utilizador envia a password pela
rede. Pode ser interceptada ou descoberta por força bruta.

Autenticação por chave SSH: usa um par de chaves criptográficas.
A chave privada nunca sai do computador do utilizador. O servidor
tem apenas a chave pública. É mais seguro porque nenhum segredo
viaja pela rede.

## Chave pública
Ficheiro: ~/.ssh/id_ed25519.pub
Algoritmo: ED25519
Pode ser partilhada e copiada para servidores remotos.
Permissões: rw-r--r-- (644) — qualquer utilizador pode ler.

## Chave privada
Ficheiro: ~/.ssh/id_ed25519
Nunca deve ser partilhada ou copiada para outros sistemas.
Permissões: rw------- (600) — apenas o dono tem acesso.
O SSH recusa-se a usar a chave privada se as permissões
estiverem abertas.

## Cuidados de segurança
- Nunca partilhar a chave privada.
- Nunca copiar id_ed25519 para outro sistema.
- Proteger a chave privada com uma passphrase em ambientes reais.
- Verificar sempre as permissões da pasta ~/.ssh.

## Evidência segura
As chaves foram geradas com ssh-keygen usando o algoritmo ED25519.
O fingerprint da chave pública é:
SHA256:ouHFDLw1QtEralNyrLWc8yFbibdv+KC9ie7+lwh6Xog
O conteúdo da chave privada não é incluído por razões de segurança.
