# Blade Snippets for Sublime Text

`Blade` is a simple, yet powerful templating engine provided with [Laravel] (http://laravel.com).

These snippets works with blade files (`.blade.php`) either with php syntax or with blade syntax using: **PHP - Laravel Blade** available from [Laravel Blade Highlighter] (https://github.com/Medalink/laravel-blade) package.

##Usage
When you're on a blade file, type the snippet shortcut then press `tab` key.

##Installation
Clone this repository into your Packages folder:
		
    git clone https://github.com/AAlakkad/blade-snippets.git


Or download the snippets zip file and unzip it into your Packages folder.

##Avalable snippets
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
		<br><br>
		@endsection
		</td>
	</tr>
	<tr>
		<td>secy</td>
		<td>
		@section('`name`')
		<br><br>
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
		<br><br>
		@endif
		</td>
	</tr>
	<tr>
		<td>ife</td>
		<td>
		@if (`condition`) 
		<br><br>
		@else 
		<br><br>
		@endif
		</td>
	</tr>
	<tr>
		<td>foreach</td>
		<td>
		@foreach(`$array` as `$element`) 
		<br><br>
		@endforeach
		</td>
	</tr>
	<tr>
		<td>fore</td>
		<td>
		@forelse (`$array` as `$element`) 
		<br><br>
		@endforelse
		</td>
	</tr>
	<tr>
		<td>for</td>
		<td>
		@for (`$i` = `0`; `$i` `<` `…`; `$i++`) 
		<br><br>
		@endfor
		</td>
	</tr>
	<tr>
		<td>while</td>
		<td>
		@while (`condition`) 
		<br><br>
		@endwhile
		</td>
	</tr>
	<tr>
		<td>unless</td>
		<td>
		@unless (`condition`) 
		<br><br>
		@endunless
		</td>
	</tr>
	</table>


---
Find me on:
* Github: @AAlakkad.
* Twitter: [@Am_Alakkad](https://twitter.com/Am_Alakkad).
* Email: [am.alakkad@gmail.com] (mailto:am.alakkad@gmail.com).
