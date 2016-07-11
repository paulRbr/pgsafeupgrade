# pgSafeUpgrade

Script to automatically follow procedure from https://www.postgresql.org/docs/9.5/static/pgupgrade.html

## Usage

Launch a dry-run upgrade (`-C`), prompting step by step (`-S`), from 9.2 to 9.5 on primary `pg.example.org` and secondaries `pg2.example.org`, `pg3.example.org`:

```bash
> pg_safe_upgrade -C -S -f 9.2 -t 9.5 -p pg.example.org -r pg2.example.org,pg3.example.org -C
```
