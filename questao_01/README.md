# Questão 1

## Sobre o 'grep':

O 'grep' é um comando utilizado para encontrar ocorrências de padrões (strings) em um arquivo ou em um fluxo de dados recebido na entrada padrão. Está presente na maioria dos sistemas Unix-like (como Linux, FreeBSD, macOS, etc.). É utilizado com frequência por usuários desses sistemas operacionais e faz parte do dia-a-dia dos administradores de redes.


## Tarefa:

Crie o programa 'meu\_grep', que implementa as funcionalidades principais do 'grep'. Na linha de comando, seu programa deverá receber: 

- padrão (string) a ser procurado (obrigatório);
- arquivo texto (opcional) no qual o grep deve realizar a procura; caso o usuário não especifique o arquivo texto onde deve ser realizada a procura, o programa deverá capturar os dados a partir da entrada padrão (stdin);
- '-c' (opcional, em qualquer posição): indica que o programa deve exibir como saída somente a contagem das linhas que contém o padrão;
- '-i' (opcional, em qualquer posição): indica que o programa deve ignorar diferenças entre maiúsculas e minúsculas.
Como saída, o programa deverá mostrar as linhas do arquivo texto (ou da stdin) que contém o padrão procurado. Caso o usuário utilize a flag '-c', apresentar a quantidade de linhas que contém o padrão procurado ao invés exibir o conteúdo.


## Exemplo:

* Exemplo 1
Linha de execução no terminal(linux):
```shell
./meu_grep ida poema.txt
```
Saída:
```
Minh'alma, de sonhar-te, anda perdida.
Pois que tu és já toda a minha vida!
Não vejo nada assim enlouquecida...
A mesma história tantas vezes lida!...
```

* Exemplo 2
Linha de execução no terminal(linux):
```shell
./meu_grep -c ida poema.txt
```
Saída:
```
4
```

* Exemplo 3
Linha de execução no terminal(linux):
```shell
cat poema.txt | meu_grep -i meu
```
Saída:
```
Meus olhos andam cegos de te ver.
Não és sequer razão do meu viver
Passo no mundo, meu Amor, a ler
```
