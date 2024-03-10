# Laravel CLI

List of helpful artisan commands within Laravel framework.

---

## Generating stuff

```bash
# Generate models
# Flags:
#   -m - create migration
#   -f - create factory
#   -s - create seeder
php artisan make:model <model_name>

# Create factory
php artisan make:factory <factory_name>
```
---

## Migrations

```bash
# Run migrations
php artisan migrate

# Refresh database
# --seed flag, to seed the database aswell
php artisan migrate:refresh

# Rollback migrations
php artisan migrate:rollback --step=<steps>
```
---