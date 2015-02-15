# ANG-Validator
A simplest form validator jquery plugin 

<div>
<h3> How to Use :=> </h3>
<p>
<h5>include required files in head tag :=></h5>
<code>
&#x3C;script src=&#x22;http://code.jquery.com/jquery-1.11.2.min.js&#x22;&#x3E;&#x3C;/script&#x3E;
<br>
&#x3C;script type=&#x22;text/javascript&#x22; src=&#x22;angvalidate-1.0.min.js&#x22; &#x3E;&#x3C;/script&#x3E;
<br>
&#x3C;link rel=&#x22;Stylesheet&#x22; type=&#x22;text/css&#x22; href=&#x22;angvalidate.css&#x22; /&#x3E;

</code>

</p>

<p>
<h5>initiate plugin using following code :=></h5>
<code>
&#x3C;script type=&#x22;text/javascript&#x22;&#x3E;
  <br> $(document).ready(function(){  <br>   <br> 
  
  $(&#x27;.required&#x27;).angvalidate();   <br>   <br> 
  
  });    <br> 
  &#x3C;/script&#x3E;
</code>
<h5 style="color:#f00;">Note: Here ".required" is the element selector you can use your own</h5>
</p>

<p>
<h5>Use html code as below :=></h5>
<code>
&#x3C;input  type=&#x22;text&#x22; name=&#x22;sample_text&#x22; class=&#x22;required&#x22;  &#x3E;

</code>

<h5>You can apply custom options as below :=></h5>
<code>
&#x3C;input  type=&#x22;file&#x22; name=&#x22;sample_file&#x22; class=&#x22;required&#x22; 
 ang-options=&#x22;display-id:valid_file;allowed-ext:jpg,png;allowed-size:29000;msg:Please Select File;msg-ext:Please Select jpg or png File;msg-size:file size exceed&#x22;&#x3E;
</code>

</p>

<hr>
<p>
<h3>Initialise plugin with custom options :=></h3>
<code>
 $(&#x27;.required&#x27;).angvalidate({
        <br><br>error_message        :&#x27;This field is required.&#x27;,      //default error message
&#x9;&#x9;<br><br>error_message_ext    :&#x27;File type is not valid.&#x27;,      //default file type error message
&#x9;&#x9;<br><br>error_message_size   :&#x27;File size is not accepted.&#x27;,   //default file size error message
&#x9;&#x9;<br><br>error_msg_class      :&#x27;error_msg&#x27;,                    //default error message class
&#x9;&#x9;<br><br>error_input_class    :&#x27;error_input&#x27;,                  //default error input class
&#x9;&#x9;<br><br>success_input_class  :&#x27;success_input&#x27;,                //default success input class
&#x9;&#x9;<br><br>allowed_max_size     :1000,                           //default maximum file size in KB
&#x9;&#x9;<br><br>allowed_extesnsions  :&#x22;jpg,png&#x22;                       //default allowed file extensions
  <br><br>}); 

</code>
</p>

<hr>
<p>
<h3>Custom Options :=></h3>
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
</p>


</div> 
