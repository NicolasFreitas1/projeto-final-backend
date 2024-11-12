## Executando

Para executar o projeto:

1. Modifique o arquivo `.env.template` para `.env` e preencha as variáveis de ambiente, ou defina diretamente pelo terminal.
3. Rode o comando `docker compose up -d` na raiz do projeto.


## Tecnologias Utilizadas

* Spring Boot
* Spring Data JPA
* PostgreSQL
* Docker


## Recursos
1. Imagens: Imagens associadas a uma galeria, incluindo metadados como título, descrição e data de upload.
2. Usuários: Perfil de cada usuário, contendo informações básicas.
3. Galerias: Galerias criadas por cada usuário, podendo conter várias imagens.


## Regras de Negócio
* Cadastro Único: Cada e-mail pode estar associado a um único usuário; usuários devem verificar a disponibilidade do e-mail no momento do cadastro.
* Limite de Galerias: Defina um limite máximo de galerias que um usuário pode criar (por exemplo, até 10 galerias por usuário).
* Título Único por Usuário: Cada galeria deve ter um título único para cada usuário, facilitando a organização.
* Descrição Opcional: A descrição da galeria é opcional, mas, se presente, não pode exceder um número máximo de caracteres (por exemplo, 250 caracteres).
* Limite de Imagens por Galeria: Limite de 50 imagens por galeria para evitar sobrecarga.
* Limite de Tamanho de Arquivo: Cada imagem não pode exceder um limite (por exemplo, 5MB), garantindo uma experiência mais rápida para o usuário e menos carga no servidor.
* Formato de Arquivo Permitido: Apenas formatos específicos, como .jpg, .png, e .gif, são aceitos para upload.
* Data de Upload: Todas as imagens devem ser registradas com a data de upload para histórico de visualizações e gerenciamento.



