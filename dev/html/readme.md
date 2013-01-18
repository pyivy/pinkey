# Snippets

## htmlEncode

```html
<!doctype html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
</head>
<body>

<script type="text/javascript">

function htmlEncode(str) {
	var div = document.createElement("div");
	div.appendChild(document.createTextNode(str));
    return div.innerHTML;
}

function htmlDecode(str) {
	var div = document.createElement("div");
    div.innerHTML = str;
    return div.innerHTML;
}

var str = '<img src="/path/to/img.jpg" alt="alt text" title="Title" />';

console.log(htmlEncode(str));

</script>
	
</body>
</html>
```