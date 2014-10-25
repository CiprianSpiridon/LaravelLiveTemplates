LaravelLiveTemplates
====================
To install the Laravel live templates all you need to do is copy Laravel.xml and Envoy.xml files to your IntelliJ/PhpStorm templates directory as defined below:
### IntelliJ

    Windows <User home>\.IntelliJIdea13\config\templates
    Linux ~/.IntelliJIdea13/config/templates
    Mac OS ~/Library/Preferences/IntelliJIdea13/templates

### PhpStorm 8

    Windows <User home>\.WebIde80\config\templates
    Linux ~/.WebIde80/config/templates
    Mac OS ~/Library/Preferences/WebIde80/templates

#### Classes
- `l:c` Laravel Controller
- `l:m` Laravel Model
- `l:v` Laravel Validator
 
#### Routes
- `l:r:g`  Route::get()
- `l:r:p`  Route::post()
- `l:r:r`  Route::resource()
- `l:r:gr` Route::group()
- `l:r:a`  Route::any()
- `l:r:b`  Route::bind()

#### Laravel Bootstrap fields - Generates a Div which contains a label and the field you requested
Example
[code]
<!-- username Form Input  -->
<div class="form-group">
    {{ Form::label('username','Username:') }}
    {{ Form::text('username', null, ['class' => 'form-control']) }}
    {{$errors->first('username','<span class="danger">:message</span>')}}
</div>
[/code]
- `checkboxfield`  
- `emailfield`
- `filefield`
- `passwordfield`
- `radiofield`
- `selectfield`
- `submitbutton`
- `textareafield`
- `textfield`
