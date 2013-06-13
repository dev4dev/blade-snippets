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
		@layout('`name`')
		</td>
	</tr>
	<tr>
		<td>sec</td>
		<td>
		@section('`name`') 

		@endsection
		</td>
	</tr>
	<tr>
		<td>secy</td>
		<td>
		@section('`name`')

		@yield_section
		</td>
	</tr>
	<tr>
		<td>yl</td>
		<td>
		@yield('`name`')
		</td>
	</tr>
	<tr>
		<td>par</td>
		<td>
		@parent
		</td>
	</tr>
	<tr>
		<td>}}</td>
		<td>
		{{ $`var` }}
		</td>
	</tr>
	<tr>
		<td>}}}</td>
		<td>
		{{ `expression` }}
		</td>
	</tr>
	<tr>
		<td>inc</td>
		<td>
		@include('`name`')
		</td>
	</tr>
	<tr>
		<td>if</td>
		<td>
		@if (`condition`) 

		@endif
		</td>
	</tr>
	<tr>
		<td>ife</td>
		<td>
		@if (`condition`) 

		@else 

		@endif
		</td>
	</tr>
	<tr>
		<td>foreach</td>
		<td>
		@foreach(`$array` as `$element`) 

		@endforeach
		</td>
	</tr>
	<tr>
		<td>fore</td>
		<td>
		@forelse (`$array` as `$element`) 

		@endforelse
		</td>
	</tr>
	<tr>
		<td>for</td>
		<td>
		@for (`$i` = `0`; `$i` `<` `…`; `$i++`) 

		@endfor
		</td>
	</tr>
	<tr>
		<td>while</td>
		<td>
		@while (`condition`) 

		@endwhile
		</td>
	</tr>
	<tr>
		<td>unless</td>
		<td>
		@unless (`condition`) 

		@endunless
		</td>
	</tr>
	</table>


---
Forked from [dev4dev/blade-snippets] (https://github.com/dev4dev/blade-snippets)