# vuejs

#1. Component
```php
    When you use the class attribute on a custom component, those classes will be added to the component’s root element. Existing classes on this element will not be overwritten.

    Vue.component('my-component', {
        template: '<p class="foo bar">Hi</p>'
    });

    <my-component class="baz boo"></my-component>

    <p class="foo bar baz boo">Hi</p>
```