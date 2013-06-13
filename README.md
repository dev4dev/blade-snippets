## Blade Template Engine Snippets

These snippets support files with blade syntax: **PHP - Laravel Blade** available from [Laravel Blade Highlighter] (https://github.com/Medalink/laravel-blade) package beside file with normal html syntax.

###Usage
When you're on a blade file, type the snippet shortcut then press `tab` key.

###Avalable snippets

<table>
	<tr>
		<th>Shortcut</th>
		<th>Result</th>
	</tr>
	<tr>
		<td>lay</td>
		<td>
		<code>@layout('`name`')</code>
		</td>
	</tr>
	<tr>
		<td>sec</td>
		<td>
		<code>@section('`name`') 


		@endsection</code>
		</td>
	</tr>
	<tr>
		<td>secy</td>
		<td>
		<code>@section('`name`')


		@yield_section</code>
		</td>
	</tr>
	<tr>
		<td>yl</td>
		<td>
		<code>@yield('`name`')</code>
		</td>
	</tr>
	<tr>
		<td>par</td>
		<td>
		<code>@parent</code>
		</td>
	</tr>
	<tr>
		<td>}}</td>
		<td>
		<code>{{ $`var` }}</code>
		</td>
	</tr>
	<tr>
		<td>}}}</td>
		<td>
		<code>{{ `expression` }}</code>
		</td>
	</tr>
	<tr>
		<td>inc</td>
		<td>
		<code>@include('`name`')</code>
		</td>
	</tr>
	<tr>
		<td>if</td>
		<td>
		<code>@if (`condition`) 


		@endif</code>
		</td>
	</tr>
	<tr>
		<td>ife</td>
		<td>
		<code>@if (`condition`) 


		@else 


		@endif</code>
		</td>
	</tr>
	<tr>
		<td>foreach</td>
		<td>
		<code>@foreach(`$array` as `$element`) 


		@endforeach</code>
		</td>
	</tr>
	<tr>
		<td>fore</td>
		<td>
		<code>@forelse (`$array` as `$element`) 


		@endforelse</code>
		</td>
	</tr>
	<tr>
		<td>for</td>
		<td>
		<code>@for (`$i` = `0`; `$i` `<` `…`; `$i++`) 


		@endfor</code>
		</td>
	</tr>
	<tr>
		<td>while</td>
		<td>
		<code>@while (`condition`) 


		@endwhile</code>
		</td>
	</tr>
	<tr>
		<td>unless</td>
		<td>
		<code>@unless (`condition`) 


		@endunless</code>
		</td>
	</tr>
	</table>


---
Forked from [dev4dev/blade-snippets] (https://github.com/dev4dev/blade-snippets)