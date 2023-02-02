![Django logo](slides/django-squashmigrations/images/logo-django.svg)

"`squashmigrations`"<br>can be your enemy

&nbsp;

<small>

#### PyCon IT 2023

</small>


<aside class="notes">

## Elevator pitch (300 chars)

`squashmigrations` is a great Django command, but it has some limitations, and it could work in a way you don't need.

Let's inspect this command and the alternative of creating migrations "from scratch" in an existing project for improving your tests speed.


## Abstract (5000 chars)

Django migrations are a great tool for keeping track of changes you made to your models over time.
After years of changes in a project they can become very numerous and you may notice that it takes a long time to create the test database.

`squashmigrations` can help you reduce an existing set of many migrations down to one (or sometimes a few), which still represent the same changes.
However it has some limitations, and it could work in a way you don't need.

Let's inspect this command and the alternative of creating migrations "from scratch" in an existing project for improving your tests speed.


</aside>
