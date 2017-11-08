# Introduction
***



This is some text



This is some equation

$\chi^2$



This is some graphic

![](/img/optimizable-parameters.svg)



This is some code in Python
```python
from datalab import storage
if storage.Buckets().contains('some-bucket'):
  print('The outcome was {}'.format(True))
```

This is some code in JavaScript
```javascript
import { storage } from 'datalab'
const checkBucket = callback => {
  if (storage.Buckets().contains('some-bucket')) {
    callback(null, true)
  } else {
    callback('error')
  }
}
checkBucket((err, result) => {
  if err console.error(err)
  console.log(`The outcome was ${result}`)
})
```
