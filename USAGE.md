<!-- Start SDK Example Usage -->


```go
package main

import (
	"context"
	testauthsamplesdk "github.com/speakeasy-sdks/test-auth-sample-sdk"
	"log"
)

func main() {
	s := testauthsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->