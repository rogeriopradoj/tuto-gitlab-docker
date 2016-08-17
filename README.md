# tuto-gitlab-tutorial

GitLab Community Edition in Docker tutorial

Seguindo mistura de três tutoriais:
- https://blog.sixeyed.com/run-gitlab-on-a-usb-stick-with-docker/
- http://docs.gitlab.com/omnibus/docker/README.html
- https://blog.jscrambler.com/migrating-your-gitlab-infrastructure-into-docker/

## Passos

### Instalação

1. Cria docker-compose.yml (ajusta bem portas, volumes e variáveis de ambiente)
2. Roda `docker-compose up -d` para baixar a imagem e subir o container
3. Acessa no browser http://localhost:8050/

### Atualização da versão do GitLab CE

1. Roda `docker stop gitlab` para parar o container
2. Atualiza tag da imagem no arquivo docker-compose.yml
3. Roda `docker-compose pull` para trazer a nova versão da imagem
4. Roda `docker-compose up -d` para subir o container
5. Acessa no browser http://localhost:8050/