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
| secsim    | @section('`name`', '`content`')  |
| hass      | @hasSection('`name`') <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- expr --\}\}** <br /> @endif  |
| yl        | @yield('`section`', '`default`') |
| lsec      | @section('`name`') <br /> **{{-- expr --\}\}** <br /> @show |
| par       | @parent   |

### Components & Slots

| Shortcut  | Result |
|-----------|--------|
| comp      | @component('`component`', '`data`') <br /> **{{-- expr --\}\}** <br /> @endcomponent  |
| slot      | @slot('`slot`') <br /> **{{-- expr --\}\}** <br /> @endslot |

### Displaying data

| Shortcut  | Result |
|-----------|--------|
| !!        | {!! $`var` !!}    |
| }}        | {{ `escaped output` }}    |

### Blade & JavaScript Frameworks

| Shortcut  | Result |
|-----------|--------|
| @{{       | @{{ `javascript` }}    |
| verb      | @verbatim <br /> **{{-- code --\}\}** <br /> @endverbatim  |

### Control Structures

| Shortcut  | Result |
|-----------|--------|
| if        | @if (`condition`) <br /> **{{-- expr --\}\}** <br /> @endif   |
| ife       | @if (`condition`) <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- expr --\}\}** <br /> @endif  |
| eif       | @elseif (`condition`) <br /> **{{-- expr --\}\}** |
| switch        | @switch($i) <br> &nbsp;&nbsp;&nbsp;&nbsp;@case(case1) <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;First case... <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;@break <br> <br>&nbsp;&nbsp;&nbsp;&nbsp;@default <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Default case... <br> @endswitch <br>|
| unless    | @unless (`condition`) <br /> **{{-- expr --\}\}** <br /> @endunless  |
| for       | @for (`$i` = `0`; `$i` `<` `…`; `$i++`) <br /> **{{-- expr --\}\}** <br /> @endfor  |
| foreach   | @foreach(`$array` as `$element`) <br /> **{{-- expr --\}\}** <br /> @endforeach  |
| fore      | @forelse (`$array` as `$element`) <br /> **{{-- expr --\}\}** <br /> @endforelse  |
| while     | @while (`condition`) <br /> **{{-- expr --\}\}** <br /> @endwhile  |
| inc       | @include('`view.name`', `['some' => 'data']`)  |
| incif     | @includeIf('`view.name`', `['some' => 'data']`)  |
| incwhen   | @includeWhen(`boolean`, '`view.name`', `['some' => 'data']`)  |
| incf      | @includeFirst(['`custom.admin`', '`admin`'], `['some' => 'data']`)  |
| each      | @each ('`item.view`', $`items`, '`item`', '`empty.view`') |
| continue  | @continue('condition') |
| break     | @break('condition') |
| php       | @php<br /> **{{-- expr --\}\}** <br /> @endphp   |
| empty     | @empty (`condition`)<br /> **{{-- expr --\}\}** <br /> @endempty   |
| isset     | @isset (`condition`)<br /> **{{-- expr --\}\}** <br /> @endisset   |

### Stacks

| Shortcut  | Result |
|-----------|--------|
| stack     | @stack('`name`')  |
| push      | @push('`name`') <br /> **{{-- expr --\}\}** <br /> @endpush    |
| prepend   | @prepend('`name`') <br /> **{{-- expr --\}\}** <br /> @endprepend    |

### Authentication Shortcuts

| Shortcut  | Result |
|-----------|--------|
| auth     | @auth('`name`') <br /> **{{-- expr --\}\}** <br /> @endauth    |
| guest      | @guest('`name`') <br /> **{{-- expr --\}\}** <br /> @endguest    |

### Policies

See the Laravel [Policies documentation](https://laravel.com/docs/5.3/authorization#via-blade-templates).

| Shortcut  | Result |
|-----------|--------|
| can       | @can('`policy`', Model::class) <br /> **{{-- expr --\}\}** <br /> @endcan |
| cane      | @can('`policy`', $model) <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- else expr --\}\}** @endcan |
| cannot    | @cannot('`policy`', Model::class) <br /> **{{-- expr --\}\}** <br /> @endcannot |
| cannote   | @cannot('`policy`', $model) <br /> **{{-- expr --\}\}** <br /> @else <br /> **{{-- else expr --\}\}** @endcannot |
| canany    | @canany('`policy`', $model) <br /> **{{-- expr --\}\}** @endcanany |
| cananye   | @canany(['`policy`', '`policy`'], $model) <br /> **{{-- expr --\}\}** <br> @elsecanany(['`policy`', '`policy`'], $model) <br /> **{{-- expr --\}\}** <br> @endcanany |

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
| csrf      | @csrf |
| method    | @method('`PUT`') |
| json      | @json(`expression`) |
| dump      | @dump(`expression`) |

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
