# web-api

Custom http client for interacting with a rest-api service.  
Based on the standard js fetch method for request.

To use just create a new model and specify the required endpoint.

```javascript
class MyModel from CRUDModel {
  constructor() {
    super(new Route('api/your-endpoint'))
  }
}

export default new MyModel();

...

MyModel.getAll().then(result => result.data);

const id = 23; 
MyModel.get(id).then(console.log);

const data = { title: 'Post#23', descr: '...' };
MyModel.create(data).then(console.log);

const newData = { title: 'New post' };
MyModel.update(id, newData).then(console.log);

MyModel.delete(id).then(result => result.success);
```
