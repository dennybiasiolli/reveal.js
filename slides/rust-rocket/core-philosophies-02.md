#### Rocket core philosophies

All request handling information<br>
should be typed and self-contained.

<small>
Because the web and HTTP are themselves untyped (or stringly typed, as some call it),
this means that something or someone has to convert strings to native types.

Rocket does this for you with zero programming overhead.

What's more, Rocket's request handling is self-contained with zero global state:
handlers are regular functions with regular arguments.
</small>


<aside class="notes">
</aside>
