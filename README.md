# curl

| Método HTTP | Uso típico | Exemplo com `curl` |
|-------------|------------|---------------------|
| **GET**     | Buscar dados de um recurso | `curl -X GET https://api.exemplo.com/data` |
| **POST**    | Enviar dados para criar algo | `curl -X POST https://api.exemplo.com/data -d '{"nome":"Marcelo"}' -H "Content-Type: application/json"` |
| **PUT**     | Atualizar completamente um recurso existente | `curl -X PUT https://api.exemplo.com/data/123 -d '{"nome":"Atualizado"}' -H "Content-Type: application/json"` |
| **PATCH**   | Atualizar parcialmente um recurso | `curl -X PATCH https://api.exemplo.com/data/123 -d '{"status":"ativo"}' -H "Content-Type: application/json"` |
| **DELETE**  | Remover um recurso | `curl -X DELETE https://api.exemplo.com/data/123` |

### Observações
- `-X` serve para **especificar o método HTTP**.  
- Se você não usar `-X`, o `curl` assume **GET** por padrão.  
- Para enviar dados (`POST`, `PUT`, `PATCH`), geralmente você precisa usar `-d` (data) e definir o cabeçalho `Content-Type`.  
