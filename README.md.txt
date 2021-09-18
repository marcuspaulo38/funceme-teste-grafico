1 - Entra na pasta onde você baixou o projeto e se precisar reistalar o composer
composer install --ignore-platform-reqs


2 - dentro de relatorios crie o contener:
docker-compose up -d
ou
docker-compose up --build (este aqui é pra forçar)

3 - Inicie o docker
docker-composer exec app bash

4 - Starte o projeto(os arquivos de configurações estão no docker-compose.yaml para mudar as portas)
php artisan serve --host=0.0.0.0