# vuejs

#1. Filter
```php
    Filters are usable in two places: mustache interpolations and v-bind expressions.
```
#2. Filters can be chained
```php
    {{ message | filterA | filterB }}
```

#3 v-bind shorthand
```php
    full syntax
    <a v-bind:href="url">{{ url }}</a>

    shorthand
    <a :href="url">{{ url }}</a>
```

#4 v-on shorthand
```php
    full syntax
    <button v-on:click="events()">Button</button>

    shorthand
    <button @click="events()">Button</button>
```