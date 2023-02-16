```go
import (
	"encoding/json"
	"net/http"
)

func ReadBody(r *http.Request, result interface{}) {
    decoder := json.NewDecoder(r.Body)
    err := decoder.Decode(result)
    if err != nil {
        // error handling here
    }
}
```
