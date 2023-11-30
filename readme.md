Application Programming Interface son mecanismos que permiten a dos componentes de software comunicarse entre sí mediante un conjunto de definiciones y protocolos. Comúnmente el formato de intercambio de datos utilizados es JSON o XML.

**XML**

```
`<name>`
    `<nombre>`Luke Skywalker `</nombre>`
    `<app>`172 `</app>`
    `<address>`
        `<street></street>`
            `<number>`
                `<int>`B `</int>`
                `<ext>`990 `</ext>`
            `</number>`
    `</address>`
`</name>`
```

**JSON**

```
{
	"name": "Luke Skywalker",
	"height": "172",
	"address": {
        	street: '',
        	number: { int: B, ext: 990 },
    	}
}
```

#### Conceptos de una API

* **Client:** Es quien realiza la petición.
* **Request:** Petición http conformada por url, params, payload.
* **Url:** Dirección de internet.
* **Payload:** Información que va en el body de la request.
* **Método o verbo:** Es la acción (GET, POST, PUT, PATCH y DELETE) con la que se accede a un endpoint.
* **Recurso:** Es el endpoint al que llegamos en la API.
* **Response:** Respuesta de la API.
* **Server:** Es quien responde la petición.

#### **Listado de protocolos**

* TCP/IP.
* HTTP.
* HTTPS.
* FTP.
* SMTP.
* IMAP.
* POP.
* SSL.
* TLS.

[Listado completo de puertos](https://docs.opencloud.cl/tutoriales/servidores/lista-de-puertos-mas-comunmente)

#### **Listado de status**

**100 Information**

* 100 Continue

**200 Success**

* 200 OK
* 201 Created
* 202 Accepted
* 204 No content

**300 Redirección**

* 304 Not modified

**400 Client Errors**

* 400 Bad request
* 401 Unauthorized
* 403 Forbidden
* 404 Not found
* 405 Not allowed method
* 408 Request timeout
* 409 Conflict

**500 Server Errors**

* 500 Internal server error
* 501 Not implemented
* 503 Service unavailable
* 504 Gate timeout

[Listado completo de estatus http.](https://developer.mozilla.org/es/docs/Web/HTTP/Status)

### Qué es REST y sus principios.

Es una “evolución” de SOAP (servicios web). REST es una interfaz para conectar varios sistemas.

### API Rest.

Es una serie de principios que las API siguen para “volverse” API REST, cuándo cumplen todos los principios, se les conoce como API Restful.

* Client.
* Request.
* Contrato.
* Response.
* Server.

#### **Contrato de un API**

Es un conjunto de acuerdos entre cliente y servidor para establecer la comunicación.

* Interfaz.
* Método.
* Body y parametros (si aplican).
* Estatus de respuesta.
* Formato de intercambio de datos.
