### validatr
---
https://github.com/jaymorrow/validatr/

```js
jQuery(function($) {
  $('form').validatr();
});
```

```js
$('form').validatr('addTest', 'example', function(element){});

$('form').validatr('addTest', {
  example: function(element){}
});

$.validatr.addTest(name[, fn])

$.validatr.getElement(form)

$.validatr.validateElement(element)

$.validatr.validateForm(form)

$.validatr.messages = {
  checkbox: 'Please check this box if you want to proceed.',
  color: 'Please enter a color in the format #xxxxxx',
  email: {
    single: 'Please enter an email address.',
    multiple: 'Please enter a comma separated list of email addresses.'
  },
  pattern: 'Please match the requested format.',
  radio: 'Please select one of these options.',
  range: {
    base: 'Please enter a {{type}}',
    overflow: 'Please enter a {{type}} greate than or equal to {{min}}.',
    overflow: 'Please enter a {{type}} greater than or equal to {{min}}<br> and less than or equal to {{max}}.',
    invalid: 'Invalid {{type}}',
    underflow: 'Please enter a {{type}} less than or equal to {{max}}'
  },
  required: 'Please fill out this field.',
  select: 'Please select an item in the list.',
  time: 'Please enter a time in the format hh:mm:ss',
  url: 'Please enter a url.'
}

function(element){
  return{
    valid: true/false,
    message: 'Error'
  };
}

{
  valid: Boolean,
  message: 'String'
};



```

```
<input type="date" date-match="name-or-id">

<input type="text" data-as="date">
```

