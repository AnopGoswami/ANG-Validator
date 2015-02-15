# ANG-Validator
A simplest form validator jquery plugin 

How to Use :=>

include required files in head tag :=>

<script src="http://code.jquery.com/jquery-1.11.2.min.js"></script> 
<script type="text/javascript" src="angvalidate-1.0.min.js" ></script> 
<link rel="Stylesheet" type="text/css" href="angvalidate.css" />
initiate plugin using following code :=>

<script type="text/javascript"> 
$(document).ready(function(){ 

$('.required').angvalidate(); 

}); 
</script>

Note: Here ".required" is the element selector you can use your own

use html code as below :=>

<input type="text" name="sample_text" class="required" >

you can apply custom options as below :=>

<input type="file" name="sample_file" class="required" ang-options="display-id:valid_file;allowed-ext:jpg,png;allowed-size:29000;msg:Please Select File;msg-ext:Please Select jpg or png File;msg-size:file size exceed">


Initialise plugin with custom options :=>

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



Custom Options :=>

display-id : Id of element where error message to be displayed.
msg : Message to be displayed when error.
allowed-size : Maximum file size to be uploaded in KB for input type file.
allowed-ext : Comma Separated value of allowed extensions for input type file.
msg-size : Message to be displayed when size exceeded for input type file.
msg-valid : Message to be displayed when value of input field is not valid.
numeric : Value true or 1 . To take only numeric input.
alphanum : Value true or 1 . To take only alpha numeric input.
alpha : Value true or 1 . To take only alphabatic input.
special-chars : Value true or 1 . To not accept special characters as input.
url : Value true or 1 . Not accept input if not a valid url.
email : Value true or 1 . Not accept input if not a valid email address.
match-id : Match value of current input whith other input having id as defined.
min-length : Check for minimum length.
max-length : Check for maximum length.
custom-function : Call custom function. Value should be name of function
