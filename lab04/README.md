## Modelo para Apresentação do Lab04 - Serviços

### ALUNO
   >Renan Alves da Silva
<br><br>

## Tarefa 1
  ![Tarefa1](images/image1.jpg)
## Tarefa 2
  ![Tarefa2](images/image2.jpg)
## Tarefa 3
  ![Tarefa3](images/image3.jpg)
## Tarefa 4
### Serviço Consulta CEP

* **Título do serviço**: `Consultar CEP
* **Breve descrição**: O serviço consulta CEP recebe como parâmetro o CEP desejado e o padrão de resposta, neste caso JSON, o mesmo retornará o endereço completo, caso o CEP seja válido.
  Serviço que recebe o número de uma das tirinhas do XKCD e retorna os dados da tirinha e a URL para a sua imagem.
* **URL completa da requisição**: https://viacep.com.br/ws/PARÂMETRO CEP/json
* **Cabeçalho HTTP da chamada**:
~~~http
GET /https://viacep.com.br/ws/13481645/json HTTP/2
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate, br
Accept-Language: pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7
Cache-Control: max-age=0
Connection: keep-alive
Host: viacep.com.br
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: none
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36
~~~
* **Cabeçalho HTTP da resposta**:
~~~http
Access-Control-Allow-Credentials: true
Access-Control-Allow-Headers: Content-Type, X-Request-With, X-Requested-By
Access-Control-Allow-Methods: GET, OPTIONS
Access-Control-Allow-Origin: *
Access-Control-Max-Age: 86400
Cache-Control: max-age=3600
Cache-Control: public
Connection: keep-alive
Content-Type: application/json; charset=utf-8
Date: Sun, 23 Aug 2020 20:00:48 GMT
Expires: Sun, 23 Aug 2020 21:00:48 GMT
Pragma: public
Server: nginx/1.18.0
Transfer-Encoding: chunked
~~~
* **Conteúdo da resposta**:
~~~json
{
  "cep": "13481-745",
  "logradouro": "Rua Celso Andrade",
  "complemento": "",
  "bairro": "Jardim Residencial Victório Lucato",
  "localidade": "Limeira",
  "uf": "SP",
  "ibge": "3526902",
  "gia": "4170",
  "ddd": "19"
}
~~~
