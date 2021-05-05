# textarea-auto-hight
[View Live Demo](http://textarea-auto-hight.bdroutines.com) or [View Live Demo](https://tasmir.github.io/textarea-auto-hight/index.html)

### HTML
```
<div class="container">
	<div class="h1 text-center my-2">Textarea Auto Hight</div>
	<div class="row">
		<div class="col">
			<div class="form-group">
				<label for="exampleFormControlTextarea1">Large textarea (Fixed Hight)</label>
				<textarea class="form-control rounded-0" id="exampleFormControlTextarea1" rows="10" name="inputCode"></textarea>
			</div>

		</div>
		<div class="col">
			<div class="form-group">
				<label for="exampleFormControlTextarea1">Large textarea (Auto Hight)</label>
				<textarea class="form-control rounded-0" id="exampleFormControlTextarea1" rows="10"></textarea>
			</div>
		</div>
	</div>
</div>
```

### SCRIPT
```
<script src="./js/jquery-3.6.0.min.js"></script>
<script type="text/javascript">
	{    jQuery.fn.extend({
		autoHeight: function () {
			function autoHeight_(element) {
				return jQuery(element).css({
					'height': 'auto',
					'overflow-y': 'hidden'
				}).height(element.scrollHeight);
			}
			return this.each(function () {
				autoHeight_(this).on('input', function () {
					autoHeight_(this);
				});
			});
		}
	});
	$('#exampleFormControlTextarea11').autoHeight();
}
</script>
```

### DEPENDENCY
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/js/bootstrap.bundle.min.js" integrity="sha384-JEW9xMcG8R+pH31jmWH6WWP0WintQrMb4s7ZOdauHnUtxwoG2vI5DkLtS3qm9Ekf" crossorigin="anonymous"></script>
```

## Complete Model
```
<!DOCTYPE html>
<html lang="en">
<head>

	<meta charset="UTF-8">

	<meta name="viewport" content="width=device-width, initial-scale=1">

	<title>Auto Input Width</title>

	DEPENDENCY PART 

</head>

<body>

	HTML PART

	SCRIPT PART
</body>
</html>
```
