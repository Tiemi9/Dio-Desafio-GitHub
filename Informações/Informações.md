# Git & GitHub
O git é um software que permite armazenar e versionar os projetos criando um histórico do trabalho do começo ao fim, desenvolvido por Linus Torvalds, criador do sistema operacional Linux.
O gitHub é uma plataforma web que permite armazenamto remoto dos projetos, tambem versionados, este permite que varios desenvolvedores possam trabalhar em um mesmo projeto simultaneamente, além de indentificar qual desenvolvedor é respnsavel por implementar cada parte do código.

## Termos mais usados
- Repositório: local onde ficam armazenados os arquivos, suas cópias e/ou verões;
- Branch: são os ramos, cópias dos códigos que serão manipuladas sem afetar o código-fonte;
- Merge: agregadar as atualizações ao código-fonte após realizar um trabalho em um brnach, isso ocore no repositório local;
- Push request: envio das modificações após o merge para o repositório central para verificar conflitos entre o trabalho de demais desenvolvedores;
- Pull request: usado quando há mudanças no ramo principal do repositório e é necessario puxar para sua máquina para fundir com o código local.

## Entendendo um pouco mais
SHA1 (Secure Hash Algorithm): conjunto de funções hash criptografadas que gera um conjunto de 40 caractéres, esse é modificado a cada alteração realizada no arquivo, mesmo sendo uma vírgula, se a alteração for desfeita, o SHA1 volta a ser o mesmo;
### Entenda:
- Blobs: contém metadados (tipo, tamanho, \0, conteúdo)
- Trees: armazena Blobs (tipo, tamanho, \0, blobs, sha1, nome do arquivo)
- Commit: engloba tudo (tipo, tamanho, \0, trees, sha1, nome do arquivo, parentes, autor, mensagem)

Blobs, trees e commits teem seu próprio SHA1, por isso ao alterar um arquivo todos terão alteração em seu SHA1.
