#### 🧑‍🔬 `sqlmigrate`

```sh
$ manage.py sqlmigrate main 0001
```

```sql
BEGIN;
--
-- Create model Pizza
--
CREATE TABLE "main_pizza" ("id" bigint NOT NULL PRIMARY KEY GENERATED BY DEFAULT AS IDENTITY, "created_at" timestamp with time zone NOT NULL, "text" varchar(140) NOT NULL, "created_by_id" integer NOT NULL);
ALTER TABLE "main_pizza" ADD CONSTRAINT "main_pizza_created_by_id_de58f942_fk_auth_user_id" FOREIGN KEY ("created_by_id") REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED;
CREATE INDEX "main_pizza_created_by_id_de58f942" ON "main_pizza" ("created_by_id");
COMMIT;
```


<aside class="notes">
</aside>
