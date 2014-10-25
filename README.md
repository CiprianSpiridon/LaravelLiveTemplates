Laravel Live Templates
====================
To install the Laravel live templates all you need to do is copy all .xml files to your IntelliJ/PhpStorm templates directory as defined below:
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

#### Laravel Form
- `Form::checkbox` Generate a Checkbox element (name, value, checked, attributes)
- `Form::email` Generate an Email Input element (name, default, attributes)
- `Form::input` Generate a File Input element (name, attributes)
- `Form::label` Generate a Label element
- `Form::macro` Generate a Form Macro
- `Form::model` Open a Form with Model Binding
- `Form::open` Open a Form
- `Form::openWithFileUpload` Open a Form and Enable File Upload
- `Form::password` Generate a Password Input element (name, attributes)
- `Form::radio` Generate a Radio element (name, value, checked, attributes)
- `Form::select` Generate a Drop-down list (name, array of options, default, attributes)
- `Form::selectMonth` Generate a Drop-down list with Months (name, default, attributes)
- `Form::selectRange` Generate a Drop-down list with Range (name, from, to, default, attributes)
- `Form::submit` Generate a Submit button (value, attributes)
- `Form::text` Generate a Text Input element (name, default, attributes)

#### Laravel Bootstrap fields - Generates a Div which contains a label and the field you requested
Example for `textfield`
```php
<!-- username Form Input  -->
<div class="form-group">
    {{ Form::label('username','Username:') }}
    {{ Form::text('username', null, ['class' => 'form-control']) }}
    {{$errors->first('username','<span class="danger">:message</span>')}}
</div>
```
- `checkboxfield`  
- `emailfield`
- `filefield`
- `passwordfield`
- `radiofield`
- `selectfield`
- `submitbutton`
- `textareafield`
- `textfield`
