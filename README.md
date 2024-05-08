# Trabalho 1: Impementação do WSClock
## Descrição:
> O trabalho consistirá de uma implementação do algoritmo de substituição de páginas wsclock. Vocês podem utilizar como base, a implementação do algoritmo "clock". Lembrando que este último foi implementado em classe e consta na seção de códigos(github)


# Trabalho 2: Pesquisa sobre
## Descrição:
> O trabalho consistirá da pesquisa de 2 sistemas de arquivos, sendo o ext3 ou ext4 obrigatórios. A seguir, é apresentada uma lista com possibilidades, mas sinta-se a vontade para outras possibilidades. 

## As técnicas são:
* HFS (Mac Os)
* EXT3 e EXT4 (Unix) - OBRIGATÓRIO
* NTFS (Windows)
* FAT16 e 32 (Windows)
* ExFat (Windows)

## Técnicas escolhidas

### 1. EXT4:
* Ext4 é a evolução do sistema de arquivos mais usado no Linux, o Ext3.

* o Ext4 é uma melhoria mais profunda sobre Ext3 do que o Ext3 foi sobre Ext2. O Ext3 foi principalmente sobre adicionar journaling ao Ext2, mas o Ext4 modifica estruturas de dados importantes do sistema de arquivos como aqueles projetados para armazenar os dados de arquivos.

* O resultado é um sistema de arquivos com um desenho melhorado, melhor desempenho, confiabilidade e recursos.

### 2. NTFS:
* Sistema de arquivos primário para versões recentes do Windows e do Windows Server, fornece um conjunto completo de recursos, incluindo descritores de segurança, criptografia, cotas de disco e metadados avançados. 

* Ele pode ser usado com CSV (Volumes Compartilhados Clusterizados) para fornecer volumes continuamente disponíveis que podem ser acessados simultaneamente de vários nós de um cluster de failover.

# Bibilografia:
[Visão geral do NTFS](https://learn.microsoft.com/pt-br/windows-server/storage/file-server/ntfs-overview)

[O que é o sistema de arquivos Ext4 – guia completo sobre Ext4](https://recoverit.wondershare.com.br/file-system/ext4-file-system.html)