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

* Possui as seguintes características:
 1. **Tamanhos de Arquivo e Sistema de Arquivos:** O ext4 suporta tamanhos de arquivos de até 16 terabytes e sistemas de arquivos de até 1 exabyte, permitindo um armazenamento muito maior em comparação com sistemas de arquivos anteriores.

2. **Journaling:** Assim como o ext3, o ext4 utiliza journaling para melhorar a confiabilidade do sistema de arquivos. O journaling registra alterações antes que elas sejam realmente aplicadas, ajudando a recuperar o sistema em caso de falhas.

3. **Alocação Tardia (Delayed Allocation):** O ext4 utiliza uma técnica chamada de alocação tardia, que atrasa a alocação de blocos de disco até que os dados sejam realmente gravados. Isso melhora o desempenho, especialmente em operações de escrita.

4. **Extents:** Ao invés de usar o método tradicional de blocos, o ext4 utiliza "extents" para representar blocos contíguos de arquivos. Isso reduz a fragmentação e melhora o desempenho de leitura e escrita.

5. **Backward Compatibility:** O ext4 mantém a compatibilidade retroativa com o ext3 e ext2. Isso significa que é possível montar sistemas de arquivos ext3 e ext2 como ext4, permitindo uma transição suave.

6. **Checagem de Integridade:** O ext4 tem mecanismos para verificar e corrigir a integridade dos dados, o que aumenta a confiabilidade do sistema de arquivos.

7. **Subdiretórios:** O ext4 suporta um número praticamente ilimitado de subdiretórios (até 64.000), ao contrário do limite de 32.000 no ext3.

8. **Multiblock Allocation:** O ext4 pode alocar múltiplos blocos de uma vez, o que melhora significativamente a velocidade de escrita.

* O resultado é um sistema de arquivos com um desenho melhorado, melhor desempenho, confiabilidade e recursos.

### 2. NTFS:
* É um sistema de arquivos desenvolvido pela Microsoft e utilizado principalmente em sistemas operacionais Windows. Ele foi introduzido em 1993 com o Windows NT 3.1 e tem sido o sistema de arquivos padrão para todas as versões do Windows desde então. Abaixo estão algumas das principais características do NTFS:

1. **Segurança e Permissões:** NTFS permite a definição de permissões detalhadas para arquivos e pastas, utilizando listas de controle de acesso (ACLs). Isso permite um controle refinado sobre quem pode acessar e modificar dados.

2. **Journaling:** Similar ao ext4, o NTFS utiliza journaling para registrar alterações antes que sejam aplicadas, ajudando a recuperar o sistema em caso de falhas.

3. **Compressão de Arquivos:** O NTFS suporta a compressão de arquivos e pastas, permitindo economizar espaço em disco sem a necessidade de ferramentas externas.

4. **Criptografia:** Com o NTFS, é possível criptografar arquivos e pastas para proteger dados sensíveis, usando o EFS (Encrypting File System).

5. **Tamanhos de Arquivo e Volume:** O NTFS suporta tamanhos de arquivos e volumes extremamente grandes, com um limite teórico de até 16 exabytes (embora implementações práticas sejam menores).

6. **Cotas de Disco:** Administradores podem definir cotas de disco para limitar a quantidade de espaço que cada usuário pode utilizar, ajudando a gerenciar o uso de armazenamento.

7. **Links Simbólicos e Pontos de Reanálise:** NTFS suporta links simbólicos, permitindo que arquivos e pastas apareçam em múltiplos locais no sistema de arquivos sem duplicação dos dados.

8. **Recuperação e Integridade de Dados:** NTFS tem mecanismos para verificar e corrigir a integridade dos dados, melhorando a confiabilidade do sistema de arquivos.

9. **Streams de Dados Alternativos:** NTFS permite associar múltiplos fluxos de dados a um único arquivo, uma característica útil para armazenar metadados adicionais.

10. **Auditoria:** É possível auditar o acesso a arquivos e pastas, permitindo que administradores rastreiem ações realizadas sobre arquivos específicos.

* Ele pode ser usado com CSV (Volumes Compartilhados Clusterizados) para fornecer volumes continuamente disponíveis que podem ser acessados simultaneamente de vários nós de um cluster de failover.

# Bibilografia:
[Visão geral do NTFS](https://learn.microsoft.com/pt-br/windows-server/storage/file-server/ntfs-overview)

[O que é o sistema de arquivos Ext4 – guia completo sobre Ext4](https://recoverit.wondershare.com.br/file-system/ext4-file-system.html)