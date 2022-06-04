# DIO-github-challenge
Desafio sobre git/github da trilha do bootcamp da plataforma DIO (Digital Innovation One).


### Alguns pontos que aprendi sobre Git/Github:
**⇒** **O que é Controle de Versão?** É um sistema com a finalidade de gerenciar diferentes versões de um documento.

**⇒** **O que é Git?** É um sistema de controle de versões distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

**⇒** **O que é GitHub?** É um serviço de web compartilhado para projetos que utilizam o Git para versionamento.

**⇒** **Características e Curiosidades sobre o Git:**

- O GIT foi criado em 2005 por Linus Torvals (que também criou o núcleo, ou kernel do LINUX) e atualmente vem sendo mantido pelo engenheiro de software japonês Junio Hamano.
- O GIT é um dos mais famosos sistemas de controle de versão de código aberto e milhões de projetos no mundo inteiro o utilizam para seu controle de versão.
- O GIT segue uma abordagem peer to peer (P2P), contrário de outros como o Subversion (SVN) que segue um modelo baseado em cliente-servidor.
- Permite aos devs ter uma infinidade de ramos de cód completamente independente. Criação, exclusão e fusão desses ramos é simples e não leva tempo.
- Todas as operações são atômicas. Isso significa que uma ação pode ter sucesso ou falhar (sem fazer nenhuma alteração). Isso é importante porque em alguns sistemas de controle de versão (como o CVS - Concurrent Version Systems) onde as operações não são atômicas, se uma operação de repositório é suspensa, ela pode deixar o repositório em um estado instável.
- No GIT tudo é armazenado dentro da pasta .git. Isso não é o mesmo em outros VCS, como SVN e CVS onde os metadados de arquivos são armazenados em pastas ocultas (por ex: .cvs, .svn etc).

➡️ **P2P é um formato de rede de computadores em que a principal característica é descentralização das funções convencionais de rede, onde o computador de cada usuário conectado acaba por realizar funções de servidor e de cliente ao mesmo tempo.**

**⇒** **Algumas informações sobre o GitHub:**

- **Repositório:** é um diretório onde os arquivos do seu projeto ficam armazenados. Ele pode ficar em um depósito do GitHub ou em seu computador. Você pode armazenar códigos, imagens, áudios, ou qualquer outra coisa relacionada ao projeto no diretório.
- **Branch:** é uma cópia do diretório. Você pode usar o *branch* para desenvolver isoladamente. Trabalhar em um *branch* não irá afetar o repositório central ou outros *branches*. Depois de finalizar o trabalho você pode combinar seu *branch* isolado com outros *branches* através de um *merge*. Para combinar o *branch* isolado ao repositório central utiliza-se o *Pull Request*.
- **Pull-Request:** Efetuar um *Pull Request* significa informar outros que você irá implementar as mudanças criadas no seu *branch* ao repositório master. Os colaboradores do repositório podem aceitar ou negar a *Pull Request*. Ao abrir um *Pull Request* você pode revisar e discutir seu trabalho com os colaboradores.



→ Para abrir o terminal do **Windows** é só digitar **CMD** na barra de pesquisa.

→ Depois de aberto podemos usar os comandos:

- **dir** → para listar as pastas do diretório atual;
- **cd** ***nomeDapasta*** → para entrar em outro diretório;
- **cd ..** → para voltar um diretório;
- **cls** → para limpar o terminal;
- **cd** ***começar a escrever o nome da pasta e clicar no TAB*** → Ele completa o nome da pasta pra você;
- **mkdir *nomeDaNovaPasta*** → cria uma pasta nova no diretório atual;
- **echo** → printa de volta no terminal um texto que vc passar;
- **echo** ***textoQualquer > nomeDoArquivoNovo.extensão*** → pega o texto digitado e **redireciona (>)** para um arquivo que vc está criando.



git init é um comando único que você usa durante a configuração inicial de um novo repositório. A execução desse comando cria um novo subdiretório .git no diretório de trabalho atual. Isso também cria um novo branch principal.


**→** Estados que o arquivo pode se encontrar:

- **Untracked:** O arquivo foi criado, mas o Git ainda não o está rastreando.
- **Unmodified:** É o estado onde o arquivo não sofreu alterações em relação a sua referência.
- **Modified:** É o estado onde o arquivo sofreu alterações em relação a sua referência.
- **Staged:** É o estado onde o arquivo já foi endereçado e aguarda ser transferido ao repositório.



//Para add o arquivo ao git:
git add nomeDoArquivo

//ou para add tds os arquivos modificados de uma vez:
git add .

//Depois que add o arquivo ele vai para o estado Modified

//Para commitar (salvar uma img dele no git):
git commit -m "msg para identificar o commit feito"




//O comando git remote lista as conexões remotas que você tem com outros repositórios:
git remote

//Com o git remote -v eu tenho a mesma função acima, mas mostrando tbm a URL de cada conexão
git remote -v

//Ao fazer o git push eu subo meu repositório local para o github, onde o -u é para trackear e não precisar mais digitar a linha de comando td novamente, 
//apenas git push, o origin é pra onde ele vai e o main é de onde ele vem.
//O nome origin é um nome default q é o nome do meu repositório remoto, eu posso substituir ele por outro.
git push -u origin main
