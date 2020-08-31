# web-api

It's a client-side web api for interacting with a rest-api service.  
Based on the standard js fetch method for request.

To use just create a new model and specify the required endpoint.

```javascript
class MyModel from CRUDModel {
  constructor() {
    super(new Route('api/your-endpoint'))
  }
}
```
