# Entrega 02 : exercício de programação de um `ls -l .`

Faça um programa em C que lista todas as entradas do diretório atual ("."), e, para cada uma,
apresenta um conjunto de metadados.

Use chamadas de sistema e funções das bibliotecas básicas em C.

Teste com o diretório guarda-roupa que compõe este repositório.

Apresente os metadados conforme seu RA, dada a tabela abaixo. Confira a legenda.

Fique livre para decidir como formatar os dados, especialmente as datas e horários.
Use alguma biblioteca de formatação se quiser.


RA        | Tipo | Perm | Tam. | ID   | Hora
----------|------|------|------|------|------
151153401 |  X   |  U   |  A   |  N   |  C
151153418 |  X   |  U   |  A   |  N   |  M
151153426 |  X   |  U   |  A   |  D   |  C
161150101 |  X   |  U   |  A   |  D   |  M
161150179 |  X   |  U   |  H   |  N   |  C
161150594 |  X   |  U   |  H   |  N   |  M
161152317 |  X   |  U   |  H   |  D   |  C
171150491 |  X   |  U   |  H   |  D   |  M
171150708 |  X   |  G   |  A   |  N   |  C
171150716 |  X   |  G   |  A   |  N   |  M
171150971 |  X   |  G   |  A   |  D   |  C
171151046 |  X   |  G   |  A   |  D   |  M
171151364 |  X   |  G   |  H   |  N   |  C
171152581 |  X   |  G   |  H   |  N   |  M
171152689 |  X   |  G   |  H   |  D   |  C
171153022 |  X   |  G   |  H   |  D   |  M
171153081 |  X   |  O   |  A   |  N   |  C
171153278 |  X   |  O   |  A   |  N   |  M
171153571 |  X   |  O   |  A   |  D   |  C
171153669 |  X   |  O   |  A   |  D   |  M
171153731 |  X   |  O   |  H   |  N   |  C
171153782 |  X   |  O   |  H   |  N   |  M
181150247 |  X   |  O   |  H   |  D   |  C
191150096 |  X   |  O   |  H   |  D   |  M

Legenda:
* Tipo : Tipo de arquivo (normal|diretório|link simbólico)
* Perm : Permissões
    * U : Permissões de usuário + Nome de usuáro
    * G : Permissões de grupo + Nome do grupo
    * O : Permissões de outros + Bits especiais
* Tam. : Tamanhos
    * A : Tamanho do arquivo
    * H : Número de _hard links_
* ID    : Identificadores
    * N : Inode
    * D : Device
* Hora : Horário
    * C : Horário de criação
    * M : Horário da última modificação
