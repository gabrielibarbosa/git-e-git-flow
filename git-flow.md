# Git Flow

## O que é o Git Flow?
Git Flow é uma estratégia de branching (ramificação) para gerenciamento de versões de software que utiliza Git. Ele foi criado por Vincent Driessen em 2010 e se tornou bastante popular por fornecer um conjunto estruturado de regras para como branches devem ser criados e mesclados. Git Flow ajuda a organizar o desenvolvimento de software e a manter um fluxo de trabalho mais ordenado e previsível.

[Link da documentação git](https://git-scm.com/docs/gitworkflows)

## Vantagens do Git Flow
- É um fluxo de trabalho que preza por organização e praticidade.
- Torna o processo de desenvolvimento mais intuitivo.
- Resolve problemas e bugs no código de maneira instantânea.
- Facilita a colaboração entre a equipe e o acesso ao progresso individual.

## Branches Principais
### main (ou master)
**Propósito:** Esta branch contém o código que está pronto para produção. Todo o código aqui deve estar estável e pronto para ser lançado.  
**Uso:** É a base para todas as versões de produção do software. Alterações diretamente nesta branch devem ser evitadas.

### develop
**Propósito:** Esta branch é usada para o desenvolvimento contínuo. Ela contém as últimas alterações que foram integradas e são consideradas prontas para a próxima versão.  
**Uso:** É onde os novos recursos e correções são integrados antes de serem preparados para uma nova versão de produção.

## Branches de Suporte

### Feature
**Propósito:** Criadas para desenvolver novas funcionalidades ou recursos específicos. Geralmente são baseadas na branch develop.  
**Nomeação:** Tipicamente nomeadas como `feature/nome-do-recurso`.  
**Uso:** Após a conclusão do desenvolvimento de uma nova funcionalidade, estas branches são mescladas de volta para a branch develop.

### Hotfix
**Propósito:** Usadas para corrigir problemas críticos que surgem em produção. Elas são criadas a partir da branch main.  
**Nomeação:** Tipicamente nomeadas como `hotfix/x.y.z`.  
**Uso:** Após a correção do problema, estas branches são mescladas tanto na branch main quanto na branch develop para garantir que a correção esteja disponível tanto na versão atual quanto na próxima.

### Release
**Propósito:** Usadas para preparar uma nova versão de produção. Elas permitem que o código seja estabilizado e testado antes de ser mesclado na branch main e develop.  
**Nomeação:** Tipicamente nomeadas como `release/x.y.z`, onde x.y.z é o número d  
**Uso:** Correções de bugs, documentação e outras atividades de preparação para o lançamento são realizadas aqui. Após o lançamento, a branch de release é mesclada na branch main e também na develop para garantir que quaisquer correções sejam aplicadas à próxima versão