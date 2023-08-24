# camunda-cglib-keycloak

Ambiente de desenvolvimento para VSCode com estrutura de "docker-compose" contendo:
  - Postgres 14 (para database local, *com extensões PostGis & OGR_FDW ativas*)
  - Camunda 7.18 SpringBoot, configurado para carregar JSON nativamente via gerador de Bean/Classe em CGLib;
  - keycloak 21.1.2

## Instruções de instalação do ambiente dev java em vscode virtualizado

*from [Leandro Boeing Vieira - dev.to - **Spring Boot Development Environment with Docker and VS Code** (2021 May/03)](https://dev.to/lepsistemas/spring-boot-development-environment-with-docker-and-vs-code-42mg)*:
> # The new Era
> So, no need for a JDK installed on your machine. But you'll need VS Code and Docker, of course. After you install them, open your VS Code. In the Extensions menu, search for "Remote - Containers" and install it:
> ![imagem](https://res.cloudinary.com/practicaldev/image/fetch/s--miSqN-1J--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8mjrr7to0n7dmg4wu0ng.png)

(...)

> Now, in your VS Code, open the Command Palette (usually Ctrl or Command + Shift + P) and type ">Remote-Containers: Open Folder in Container", select it and choose the location of your extracted Spring Boot application:
> ![imagem](https://res.cloudinary.com/practicaldev/image/fetch/s--ttaPTAXJ--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1a8cyi47weqo56oqijoa.png)

### Nesta etapa, selecione entre na pasta [/camunda-cglib-keycloak/camunda/](https://github.com/P-D-MVV/camunda-cglib/blob/master/camunda/)
#### (a Pasta correta tem um arquivo chamado: ***` Dockerfile `***, sem extensão).
Finalmente, dentro dessa pasta aperte o botão [selecionar pasta] no diálogo de abrir)
E pronto! Ambiente configurado. Basta agora selecionar o arquivo java principal ( ***Application.java*** ) da aplicação spring na aba de arquivos, e iniciar com RUN ou DEBUG

![imagem](https://res.cloudinary.com/practicaldev/image/fetch/s--KUa6UhlV--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8r0ww7un8gkfykugrxgu.png)
