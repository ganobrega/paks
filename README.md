<p align="center"><img src="/docs/assets/images/paks-icon-flat.svg" alt="Icon" width="200"></p>

# PAKS

Serviço de Comunicação Anônima P2P PAKS é um projeto de comunicação anônima baseada em BlockChain e React.

**Introdução do PAKS**:

Bom, nestes últimos meses estive pensando em: "Oque posso fazer para facilitar a vida de uma pessoa no trabalho? ou até mesmo no cotidiano dela?", foi assim que começei a procurar coisas que ainda não existiam e que dificultavam o dia-dia de um programador.

Quando estou trabalhando em um projeto que preciso testar em algum aparelho, e esse aparelho não possui meu e-mail, facebook, whatsapp, etc. Como eu posso enviar algo para mim mesmo sem precisar entrar em conta, colocar senha e não guardar histórico?

**Exemplos**:

  * Compartilhar fotos, vídeos, textos e outras coisas de um dispositivo que não possui seu e-mail ou aplicativos de mensagem configurados com a sua conta ou de outras pessoas.

  * Fazer teste de links, arquivos em um aparelho de alguma empresa/startup que não possui número de telefone ou aplicativos instalados para comunicação.


No primeiro momento utilizei o QR CODE, porém toda vez eu preciso entrar em um gerador para colocar um texto ou um link e resgatar no dispositivo com a câmera, mas e se o dispositivo for um Computador?

Foi assim que tive a idéia de criar um Serviço totalmente grátis de comunicação BlockChain.

**Oque é BlockChain?**:

O BlockChain (também conhecido como “o protocolo da confiança”) é uma tecnologia que visa a descentralização como medida de segurança. São bases de registros e dados distribuídos e compartilhados que têm a função de criar um índice global para todas as transações que ocorrem em um determinado mercado.

**Como irá funcionar?**:
Cada computador que se conectar em uma mesma sala irá possuir um "pedaço" do servidor, assim a sala nunca será desligada, somente se todos os usuários sairem dela, dando lugar para outra pessoa abrir uma comunicação com o mesmo código da sala, porém com uma segurança diferente.


## Configuração do Projeto ##

Aqui estão alguns passos a passos para configurar o projeto antes de você começar o desenvolvimento!

Leia com atenção e utilize as dicas que daremos aqui.

1. #### Baixar o Projeto ####

  - ##### Não possui o projeto? #####
    -  Se você não possui o projeto em sua máquina, faça um **clone** dele, utilizando o comando abaixo:

    `git clone <url_do_repositorio>`

  -  ##### Já possui o projeto? #####
    - Se você já possui o projeto em sua máquina, mantenha sempre seu projeto atualizado com a sua **branch**, utilizando o comando abaixo:

    `git pull origin <branch>`

1. #### Instalação ####


  Após clonar o projeto, a estrutura de pastas estará parecida com o exemplo abaixo.

```
PAKS
├── images
├── public
├── source
├── package.json
└── README.md
└── ...
```

  Repare que temos um `package.json` em nosso diretório principal, onde temos algumas dependências de desenvolvimento, exemplo: **WebPack**

  1. **Instale todas as dependências**:

    * Remover pasta `node_modules`:

      `npm prune`

    * Instalar dependências

      `npm install`


  1. **Iniciando Projeto**:

      1. Após fazer a instalação das dependências, inicie o webpack com o comando:

      `webpack -d --watch`

      1. Após compilar o projeto, execute o express com o comando:

      `npm start`



## Escopo ##

  1. ##### Recursos
    * Criptografia.
    * Conectar através de QR CODE / Link / Código e uma senha de 4 dígitos.
    * Conectar até 10 dispositivos.
    * Enviar arquivos, mensagens, vídeos e tudo que é possível.
    * Não armazenar histórico.
    * Acessar via comando no terminal (Aplicativo para terminal).
    * Bloquear IP/MAC por 20 minutos para a sala após 3 tentativas de acesso.
      * Se o mesmo IP tentar acessar a mesma sala com a senha errada, mostrar um captcha de segurança contra BOT.
    * Não ser necessário informar nenhum tipo de dado (Telefone, e-mail, entre outros).
    * Servidor deleta sozinho após ficar vazio.

  1. ##### Futuros Recursos:
    * Possibilidade de acessar varias salas diferentes
    * Mandar mensagem para os integrantes individualmente, dentro da sala