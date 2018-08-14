# Jquery Commonly Used Code With Syntax

## Jquery Ajax POST and GET

```
	var data = {'name': 'Asif'}
  	$.ajax({
        type: "POST",
        url: base_url + "test/abc",
        data: data,
        success: function(data)
        {
            var result = $.parseJSON(data);
            console.log(result);
        }
       });
```

## How To Get Form Data

```
	<form>
		<input type="text" id="name"/>
		<input type="email" id="email"/>
	</form>

	var name = $("#name").val();
	var email = $("#email").val();

	console.log(name);
	console.log(email);
```

## Jquery Events


```
	<form>
		<input type="text" id="name"/>
		<input type="email" id="email"/>
		<button type="button" class="saveButton"> Save</button>
	</form>

	$('body').on('click','saveButton',function(){
			alert('save button clicked');
		});
```