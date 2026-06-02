# Permissões aplicadas

## Ambiente utilizado
VM local Ubuntu, acedida via SSH com PuTTY.

## Utilizador e grupos
- Utilizador: vboxuser
- uid=1000, gid=1000
- Grupos: vboxuser, adm, cdrom, sudo, dip, plugdev, users, lxd, vboxsf

## Ficheiros criados
- publico.txt: ficheiro de texto de acesso público
- restrito.txt: ficheiro de texto com acesso limitado
- script.sh: ficheiro executável

## Permissões aplicadas
| Ficheiro     | Permissão | Justificação                                 |
|--------------|-----------|----------------------------------------------|
| publico.txt  | 644       | Dono escreve, grupo e outros só leem         |
| restrito.txt | 640       | Dono escreve, grupo lê, outros sem acesso    |
| script.sh    | u+x       | Apenas o dono pode executar o script         |

## Relação com o princípio do menor privilégio
Cada ficheiro tem apenas as permissões necessárias para a sua função.
O ficheiro restrito.txt bloqueia completamente o acesso a outros
utilizadores porque contém informação sensível.
O script.sh só é executável pelo dono para evitar que outros
utilizadores o executem sem controlo.
Atribuir permissões totais a todos (777) seria uma má prática
porque daria acesso desnecessário a utilizadores que não precisam.
