#### Instalación
nest new products-ms

#### Escoger
npm

#### Abrir la carpeta
cd products-ms
code .

#### Levantar la aplicación
npm run start:dev

#### Instalar validador
npm i class-validator class-transformer

#### Añadir en el main la configuración global de pipes
app.useGlobalPipes(
    new ValidationPipe({
        whitelist: true,
        forbidNonWhitelisted: true,
    })
);

#### Instalar dotenv y joi para el manejo de las variables de entorno
npm i dotenv joi

#### Instalar Prisma
npm i prisma --save-dev
npx prisma init
npx prisma migrate dev --name init
npm i @prisma/client

#### Indexar el available
npx prisma migrate dev --name available-index

#### Instalar el microservice
npm i --save @nestjs/microservices