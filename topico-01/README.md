# Tópico 1 - Preparação do ambiente Linux

## Ambiente utilizado
VM local com Ubuntu, acedida através do terminal da máquina virtual.

## Objetivo desta atividade
Preparar o ambiente Linux e organizar a primeira evidência técnica,
criando a estrutura de pastas que será usada ao longo do módulo.

## Estrutura criada
linux-seguranca-cloud/
├── topico-01/
│   ├── evidencias/
│   ├── comandos-topico-01.txt
│   └── README.md
└── produto-final/

## Comandos executados
- uname -a → identifica o kernel e a arquitetura
- lsb_release -a → identifica a distribuição Ubuntu e versão
- whoami → mostra o utilizador autenticado
- hostname → mostra o nome da máquina
- mkdir -p → cria a estrutura de diretórios
- find ... | sort → confirma visualmente a estrutura criada

## Diferença entre VM, VPS e infraestrutura em nuvem
- VM local: máquina virtual que corre no teu próprio computador.
  Controlo total, sem custos, sem internet obrigatória.
- VPS: servidor virtual alugado a um fornecedor. Acessível remotamente
  via SSH. Tem IP público e corre 24 horas.
- Infraestrutura em nuvem: conjunto de serviços geridos (AWS, Azure,
  GCP). Escalável, pago por uso, sem gestão de hardware físico.

## Dificuldades encontradas
Nenhuma dificuldade relevante neste tópico.

## Próximos passos
- Ter a VM Ubuntu operacional para o próximo tópico.
- Familiarizar com navegação no terminal (cd, ls, cat, nano).
