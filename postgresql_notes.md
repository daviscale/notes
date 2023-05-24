# Postgresql Notes

## Connecting to a PostgeSQL database on a docker container

The commands below assume you've already started a shell session on a docker container.

```bash
psql -h <db-hostname> -U <db-user> <db-name>
```

Example:

```bash
psql -h db -U postgres menu_management_development
```
