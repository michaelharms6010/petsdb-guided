# Requirements

Build an API for managing pets

-save informationa bout pets. Record
    -name
    -species
    -breed
    -food
    -weight
    -weightUnit
-see a list of all pets
-update pet info
-mark pet as owned

Started an Express JS API
-npm packages: express, helmet, knex, sqlite3

run "git init"
run "npm init -y"
run "npx gitignore node"

Migrations are a way to record changes to the db schema

## Like GIT but for db sctructure

Every change to schema must be done with a new migration

### Migrations

install knex globally on your system: npm i -g knex

Create a Migration: `npx knex migrate:make name`

Run a migration: `npx knex migrate:up`

Rollback to an older migration: `npx knex migrate:down`

Update DB to latest config: `npm knex migrate:latest` <== multiple migrations

Undo multiple migrations: `npx knex migrate:rollback`