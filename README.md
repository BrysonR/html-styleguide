# uShip HTML Style Guide <html>

## <a name='TOC'>Table of Contents</a>

  1. [Syntax](#syntax)
  1. [Attributes](#attributes)
  1. [License](#license)

## <a name='syntax'>Syntax</a>
- Use tab/4-spaces to indent elements

	```html
	/* bad */
	<div>
	  <p>This is wrong</p>
	</div>

	/* good */
	<div>
		<p>This is right</p>
	</div>
	```

- Use a new line for every block, list, or table element, and indent every such child element
	
	```html
	/* bad */
	<blockquote><p><em>Space</em>, the final frontier.</p></blockquote><ul><li>Moe<li>Larry<li>Curly</ul>
	<table><thead><tr><th scope="col">Income<th scope="col">Taxes<tbody><tr><td>$ 5.00</td><td>$ 4.50</td></table>

	/* good */
	<blockquote>
	  <p><em>Space</em>, the final frontier.</p>
	</blockquote>
	<ul>
	  <li>Moe
	  <li>Larry
	  <li>Curly
	</ul>
	<table>
	  <thead>
	    <tr>
	      <th scope="col">Income
	      <th scope="col">Taxes
	  <tbody>
	    <tr>
	      <td>$ 5.00
	      <td>$ 4.50
	</table>
	```

## <a name='attributes'>Attributes</a>
- Pay attention to element attribute order 

	Order of basic attributes in element: 

	id -> class -> data-bind

	```html
	/* bad */
	<div data-bind="text: 'This Is Text'" class="test" id="test1"></div>

	/* good */
	<div id="test1" class="test" data-bind="text: 'This Is Text'"></div>
	```

- Use double quotations for attribute values

	```html 
	/* bad */
	<button id='nav-toggle' type='button'>

	/* good */
	<button id="nav-toggle" type="button">
	```

## <a name='license'>License</a>

(The MIT License)

Copyright (c) 2014 uShip

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

</html>