HistoryModelViewSet

<small>

Extends django-rest-framework's `ModelViewSet` adding

- GET `/my-model-url/<pk>/history/`

    displays a list of all revisions of that specific record

- GET `/my-model-url/<pk>/history/<version_pk>/`

    displays a specific revisions of that specific record

- GET `/my-model-url/deleted/`

    displays a list of all deleted records

- POST `/my-model-url/<pk>/revert/<version_pk>/`

    revert to a previous revision of the object

</small>

<aside class="notes">
</aside>
