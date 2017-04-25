# Blade Snippets for Sublime Text

`Blade` is a simple, yet powerful templating engine provided with [Laravel](http://laravel.com) PHP framework.

These snippets works with blade files (`.blade.php`) either with php syntax or with blade syntax using: **PHP - Laravel Blade** available from [Laravel Blade Highlighter](https://github.com/Medalink/laravel-blade) package.

## Usage
When you’re editing a blade file, type the snippet shortcut then press `tab` key.

## Installation
Via `Package Manager` search for `Blade Snippets` then click/tap…wait a sec and tadam!

![Blade Snippets](http://f.dev.mk.ua/files/dadbee44b4461b709d444951ba26f70f/file_51d27202c2a8b.png)

Or clone this repository into your Packages folder:

    git clone https://github.com/dev4dev/blade-snippets.git


Or download the snippets zip file and unzip it into your Packages folder.

---


## Available Snippets

### Template management

| Shortcut  | Result |
|-----------|--------|
| lay       | @layout('`name`')  |
| ext       | @extends('`name`') |
| sec       | @section('`name`') <br /> **{{-- expr --\}\}** <br /> @endsection    |
| secy      | @section('`name`') <br /> **{{-- expr --\}\}** <br /> @yield_section |
| hass      | @hasSection('`name`') <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- expr --\}\}** <br /> @endif  |
| yl        | @yield('`section`', '`default`') |
| lsec      | @section('`name`') <br /> **{{-- expr --\}\}** <br /> @show |
| par       | @parent   |

### Displaying data

| Shortcut  | Result |
|-----------|--------|
| !!        | {!! $`var` !!}    |
| }}        | {{ `escaped output` }}    |


### Control Structures

| Shortcut  | Result |
|-----------|--------|
| if        | @if (`condition`) <br /> **{{-- expr --\}\}** <br /> @endif   |
| ife       | @if (`condition`) <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- expr --\}\}** <br /> @endif  |
| unless    | @unless (`condition`) <br /> **{{-- expr --\}\}** <br /> @endunless  |
| for       | @for (`$i` = `0`; `$i` `<` `…`; `$i++`) <br /> **{{-- expr --\}\}** <br /> @endfor  |
| foreach   | @foreach(`$array` as `$element`) <br /> **{{-- expr --\}\}** <br /> @endforeach  |
| fore      | @forelse (`$array` as `$element`) <br /> **{{-- expr --\}\}** <br /> @endforelse  |
| while     | @while (`condition`) <br /> **{{-- expr --\}\}** <br /> @endwhile  |
| inc       | @include('`view.name`', `['some' => 'data']`)  |
| incif     | @includeIf('`view.name`', `['some' => 'data']`)  |
| each      | @each ('`item.view`', $`items`, '`item`', '`empty.view`') |
| continue  | @continue('condition') |
| break     | @break('condition') |
| php       | @php<br /> **{{-- expr --\}\}** <br /> @endphp   |

### Stacks

| Shortcut  | Result |
|-----------|--------|
| stack     | @stack('`name`')  |
| push      | @push('`name`') <br /> **{{-- expr --\}\}** <br /> @endpush    |


### Policies

See the Laravel [Policies documentation](https://laravel.com/docs/5.3/authorization#via-blade-templates).

| Shortcut  | Result |
|-----------|--------|
| can       | @can('`policy`', $model) <br /> **{{-- expr --\}\}** <br /> @endcan |
| cane      | @can('`policy`', $model) <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- expr --\}\}** @endcan |


### Miscellaneous

| Shortcut  | Result |
|-----------|--------|
| route     | {{ route('`name`') }} |
| asset     | {{ asset('`path`') }} |
| url       | {{ url('`path`') }}   |
| choice    | @choice('`language.line`', $`number`)  |
| comment   | {{-- `comment` --}}   |
| inject    | @inject('`name`', '`App\Services\ServiceName`') |
| trans     | {{ trans('`language.line`') }}    |
| lang      | @lang('`language.line`', ['`variable` => '`replacement`'])  |
| __        | {{ __('`language.line`') }}    |

---

## Envoy snippets

Snippets for [Laravel Envoy](https://laravel.com/docs/5.2/envoy).

| Shortcut  | Result |
|-----------|--------|
| serv      | @servers(['`web`' => '`user@192.168.1.1`']) |
| task      | @task('`foo`') <br /> **command** <br /> @endtask    |
| set       | @setup <br /> **{{-- expr --\}\}** <br /> @endsetup    |
| mac       | @macro('`deploy`') <br /> **command** <br /> @endmacro    |
| aft       | @after<br /> **hip** <br /> @endafter    |
| hip       | @hipchat('token', 'room', 'Envoy', "$task ran in the $env environment.") |
| sla       | @slack('hook', 'channel', 'message') |
| story     | @story('deploy') <br /> **command** <br /> @endstory |

---

## Blade Wordpress Plugin

Snippets for [Blade Wordpress Plugin](https://it.wordpress.org/plugins/blade/).

| Shortcut  | Result |
|-----------|--------|
| wpp       | @wpposts<br /> **{{-- expr --\}\}**<br />@wpempty<br>**{{-- empty expr --\}\}**<br /> @wpend |
| wpq       | @wpquery (['`post_type`' => '`post`'])<br /> **{{-- expr --\}\}**<br />@wpempty<br>**{{-- empty expr --\}\}**<br /> @wpend |
| acf       | @acfrepeater ('`fieldname`')<br /> **{{-- expr --\}\}**<br />**{{ get_sub_field('`fieldname`') \}\}**<br /> @acfend |

---

Original snippets by:
[@dev4dev](https://github.com/dev4dev)

Cool Readme formatting:
GitHub: [@AAlakkad](https://github.com/AAlakkad).

[Contributors](https://github.com/dev4dev/blade-snippets/graphs/contributors)
