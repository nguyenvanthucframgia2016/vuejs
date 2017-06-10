# vuejs

#1. computed properties
```php
    var app = new Vue({
        el: '#app',
        data: {
            firstName: 'Nguyen',
            lastName: 'Van'
        },
        computed: {
            lastName: function () {
                return this.firstName + ' ' + lastName;
            }
        }
    });

    <p>{{ lastName }}</p>

    Note: computed properties luon duoc cache. No chi duoc tu dong cap nhat lai neu cac tham so ma no phu thuoc thay doi.
    Use: Co the dung trong hau het cac truong hop (any complex logic).

    var test = new Vue({
        el: '#test',
        data: {
            message: 'Hello world'
        },
        computed: {
            reverseMessage: function () {
                return this.message.split('').reverse().join('');
            }
        }
    });

    <p>{{ reverseMessage }}</p>
```
#2. methods
```php
    var app = new Vue({
        el: '#app',
        data: {

        },
        methods: {
            now: function () {
                return Date.now();
            }
        }
    });

    <p>{{ now() }}</p>
```

    Note: methods duoc dung khi ma gia tri tra ve thay doi moi khi duoc goi. No khong duoc cache. Doi tuong ap dung cung tuong tu nhu computed properties.
#3. watch
```html
    <input type="text" v-model="question">
```

```php
    var app = new Vue({
        el: '#app',
        data: {
            question: ''
        },
        watch: {
            question: function (newValue) {
                // perform asynchronous or expensive operations in response to changing data
            }
        }
    })
```