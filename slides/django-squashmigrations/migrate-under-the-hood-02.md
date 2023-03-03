#### 👷 Migrations, under the hood

```text
mydatabase=# select * from django_migrations;
 id |     app      |                           name           |            applied
----+--------------+------------------------------------------+-------------------------------
  1 | contenttypes | 0001_initial                             | 2023-01-24 15:52:35.711176+02
  2 | auth         | 0001_initial                             | 2023-01-24 15:52:35.762036+02
  3 | admin        | 0001_initial                             | 2023-01-24 15:52:35.777581+02
  4 | admin        | 0002_logentry_remove_auto_add            | 2023-01-24 15:52:35.784175+02
  5 | admin        | 0003_logentry_add_action_flag_choices    | 2023-01-24 15:52:35.791061+02
  6 | contenttypes | 0002_remove_content_type_name            | 2023-01-24 15:52:35.80472+02
  7 | auth         | 0002_alter_permission_name_max_length    | 2023-01-24 15:52:35.811821+02
  8 | auth         | 0003_alter_user_email_max_length         | 2023-01-24 15:52:35.819289+02
  9 | auth         | 0004_alter_user_username_opts            | 2023-01-24 15:52:35.82745+02
 10 | auth         | 0005_alter_user_last_login_null          | 2023-01-24 15:52:35.834425+02
 11 | auth         | 0006_require_contenttypes_0002           | 2023-01-24 15:52:35.836142+02
 12 | auth         | 0007_alter_validators_add_error_messages | 2023-01-24 15:52:35.842359+02
 13 | auth         | 0008_alter_user_username_max_length      | 2023-01-24 15:52:35.851443+02
 14 | auth         | 0009_alter_user_last_name_max_length     | 2023-01-24 15:52:35.858551+02
 15 | auth         | 0010_alter_group_name_max_length         | 2023-01-24 15:52:35.866384+02
 16 | auth         | 0011_update_proxy_permissions            | 2023-01-24 15:52:35.873575+02
 17 | auth         | 0012_alter_user_first_name_max_length    | 2023-01-24 15:52:35.880749+02
 18 | sessions     | 0001_initial                             | 2023-01-24 15:52:36.890749+02
(18 rows)
```


<aside class="notes">
</aside>
