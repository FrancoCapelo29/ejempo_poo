
<p><mark>Fecha: 27/07/2023</mark></p>

<p>Comando para instalar nestjs <br> Es un backend</p>
$ npm i -g @nestjs/cli
$ nest new project-name

==tenemos dos puntos para levantar

$ npm run start
$ npm run start:dev

<p>Controladores<p/>
son los encargados de escuchar una solicitud y emitir una respuesta
$ nest g controller cats

<p><mark>Corregir cats</mark></p>

import { Controller, Get } from '@nestjs/common';
@Controller('cats')
export class CatsController {
@Get()
findAll(): string{
return 'This action return all cats'
}
}
![[Captura de Pantalla 2023-07-30 a la(s) 21.28.42 1.png]]
==Command line Interfase 

$ npx nest generate resource
por defecto acepta solo en plural asi que las palabras tienen que estarlo

1 $ creatures
2 $ REST API
3 $ yes

<H1>Postman</H1>
![[Captura de Pantalla 2023-07-30 a la(s) 21.28.56.png]]![[Captura de Pantalla 2023-07-30 a la(s) 21.27.56.png]]![[Captura de Pantalla 2023-07-30 a la(s) 21.28.20 1.png]]