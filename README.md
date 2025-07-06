# Git e Github

<img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" width="50"/>

`Git é um sistema de controle de versão distribuído open-source criado por Linus Torvalds em 2005 para gerenciar o desenvolvimento do kernel Linux.`

```mermaid
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit
   checkout main
   merge develop
   commit
   commit
```

<img src="https://github.com/user-attachments/assets/dfbd3220-149a-41fb-b694-0cfa36d14ae8" width="50"/>

`GitHub é uma plataforma de hospedagem de código-fonte e colaboração baseada em Git, criada por Tom Preston-Werner, Chris Wanstrath, PJ Hyett e Scott Chacon em 2008. Atualmente, tem como proprietária a empresa Microsoft.`

Ao integrar Git e Github é possível combinar as funcionalidades de versionamento, compartilhamento de projetos e colaboração entre pessoas:

```mermaid
flowchart LR
    A["Repositório Local"]
    B["Repositório Remoto"]
    B --> |git pull| A
    A --> |git push| B
```

**Aplicações**
- Gerenciar projetos
- Atuar colaborativamente
- Integrar Github e Colab
- Criar páginas estáticas


**[Github Pages](https://pages.github.com/)**

Permite a criação de sites estáticos integrados a um repositório.

**Templates**

[Bootstrap Portfolio](https://bootstrapmade.com/bootstrap-portfolio-templates/) |
[Jekyll Themes](http://jekyllthemes.org/) |
[Github Themes](https://pages.github.com/themes/)

