# Boas práticas de commit

O conventional commits é uma metodologia com intuito de nos auxiliar a estruturar melhor as mensagens dos commits, e também manter o histórico de mudanças organizado e legível para as pessoas do time.

## Principais Flags Utilizadas
- **feat:** sinaliza o desenvolvimento de uma nova feature, como a criação de um novo serviço, funcionalidade ou regra de negócio.  
  Exemplo: `git commit -m “feat: Criando função que retorna usuários”`

- **test:** sinaliza quando são criados cenários de testes, como testes unitários ou de integração.  
  Exemplo: `git commit -m “test: Criando teste unitário da função user()”`

- **refactor:** sinaliza refatoração de código, como alteração de lógica.  
  Exemplo: `git commit -m “refactor: Alterando lógica de apresentação da tabela”`

- **docs:** sinaliza mudanças na documentação do projeto, como README.md ou Swagger.  
  Exemplo: `git commit -m “docs: Alterando informações de deploy no readme”`

- **fix:** sinaliza correções de erros ou bugs.  
  Exemplo: `git commit -m “fix: Corrigindo função que carrega dashboard”`

## Como Fazer um Bom Commit
- Começar com um verbo no infinitivo. Escreva mensagens no presente, como se estivesse descrevendo o que o commit faz.  
  Exemplos:
  - Adicionar nova funcionalidade de login.
  - Corrigir bug na página de cadastro.
  - Implementar teste automatizado para a função X.

- Seu commit precisa responder à pergunta: "quando aplicado, esse commit irá?"

- Resuma a mudança em 50 caracteres ou menos na linha de assunto. Se precisar, adicione uma descrição mais detalhada no corpo da mensagem.

- Se o commit estiver relacionado a uma issue ou tarefa, mencione-a. Por exemplo:
  - "Corrigir erro #42"
  - "Resolver problema com autenticação"