# fake-contacts-api

A simple fake contacts API for testing web and mobile applications.

This project produces a fake JSON generated on [JSON Generator][1] and fake images generated on [Random User][2].

It also available on Heroku at this [link][3].

JSON template:

```javascript
[
  '{{repeat(100)}}',
  {
    id: '{{objectId()}}',
    age: '{{integer(20, 40)}}',
    name: '{{firstName()}} {{surname()}}',
    gender: '{{gender()}}',
    company: '{{company().toUpperCase()}}',
    email: '{{email()}}',
    photo: 'https://randomuser.me/api/portraits/men/{{integer(1, 50)}}.jpg'
  }
]
```

Thanks for [json-server][4] for the awesome project.

# License

```
MIT License

Copyright (c) 2018 Wellington Costa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

[1]: https://www.json-generator.com
[2]: https://randomuser.me
[3]: https://fake-contacts-api.herokuapp.com
[4]: https://github.com/typicode/json-server
