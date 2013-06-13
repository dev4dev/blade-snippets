## Blade Template Engine Snippets
Forked from [dev4dev/blade-snippets] (https://github.com/dev4dev/blade-snippets)

These snippets support files with blade syntax: *PHP - Laravel Blade* available from [Laravel Blade Highlighter] (https://github.com/Medalink/laravel-blade) package.
###Avalable snippets
* lay - @layout('`name`')
* sec - @section('`name`') @endsection
* secy - @section('`name`') @yield_section
* yl - @yield('`name`')
* par - @parent
* }} - {{ $`var` }}
* }}} - {{ `expression` }}
* inc - @include('`name`')

* if - @if (`condition`) @endif
* ife - @if (`condition`) @else @endif
* foreach - @foreach(`$array` as `$element`) @endforeach
* fore - @forelse (`$array` as `$element`) @endforelse
* for - @for (`$i` = `0`; `$i` `<` `…`; `$i++`) @endfor
* while - @while (`condition`) @endwhile
* unless - @unless (`condition`) @endunless