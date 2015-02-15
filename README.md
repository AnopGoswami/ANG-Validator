[ANG Validator] - jQuery Form validation plugin
================================

The jQuery form validation plugin  makes easier to apply validations on html form field. It has many 
options for different types of validations like url, email, numeric type, file validation etc.

It provides easy way to apply custom validation options like inline css. 

```html
<hr>
```

## Getting Started


### Include required files in head tag :

```html
<script src="http://code.jquery.com/jquery-1.11.2.min.js"></script> 
<script type="text/javascript" src="angvalidate-1.0.min.js" ></script> 
<link rel="Stylesheet" type="text/css" href="angvalidate.css" />
```


### Initiate plugin using following code :

```html
<script type="text/javascript"> 
$(document).ready(function(){ 

$('.required').angvalidate(); 

}); 
</script>
```


#### Note: Here ".required" is the element selector you can use your own

### Use html code as below :

```html
<input type="text" name="sample_text" class="required" >
```

### You can apply custom options like inline css as below:

```html
<input  type="file" name="sample_file" class="required"  ang-options="allowed-ext:jpg,png;allowed-size:29000;msg:Please Select File;msg-ext:Please Select jpg or png File;msg-size:file size exceed">
```

### You can initialise plugin to override default settings :

```js
$('.required').angvalidate({ 

error_message :'This field is required.', //default error message 

error_message_ext :'File type is not valid.', //default file type error message 

error_message_size :'File size is not accepted.', //default file size error message 

error_msg_class :'error_msg', //default error message class 

error_input_class :'error_input', //default error input class 

success_input_class :'success_input', //default success input class 

allowed_max_size :1000, //default maximum file size in KB 

allowed_extesnsions :"jpg,png" //default allowed file extensions 

});
```

### Custom Options :

```html
<ul>
<li><strong>display-id : </strong> Id of element where error message to be displayed.</li>
<li><strong>msg : </strong> Message to be displayed when error. </li>
<li><strong>allowed-size : </strong> Maximum file size to be uploaded in KB for input type file. </li>
<li><strong>allowed-ext : </strong> Comma Separated value of allowed extensions for input type file. </li>
<li><strong>msg-size  : </strong> Message to be displayed when size exceeded for input type file. </li>
<li><strong>msg-valid  : </strong> Message to be displayed when value of input field is not valid.</li>
<li><strong>numeric : </strong>Value true or 1 . To take only numeric input.</li>
<li><strong>alphanum : </strong>Value true or 1 . To take only alpha numeric input.</li>
<li><strong>alpha : </strong>Value true or 1 . To take only alphabatic input.</li>
<li><strong>special-chars : </strong>Value true or 1 . To not accept special characters as input.</li>
<li><strong>url : </strong>Value true or 1 .  Not accept input if not a valid url. </li>
<li><strong>email : </strong>Value true or 1 . Not accept input if not a valid email address.</li>
<li><strong>match-id : </strong> Match value of current input whith other input having id as defined. </li>
<li><strong>min-length : </strong> Check for minimum length. </li>
<li><strong>max-length : </strong> Check for maximum length. </li>
<li><strong>custom-function : </strong>Call custom function. Value should be name of function </li>
</ul>
```

