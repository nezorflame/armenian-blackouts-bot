# armenian-blackouts-bot [![Workflow status](https://github.com/nezorflame/armenian-blackouts-bot/actions/workflows/go.yml/badge.svg)](https://github.com/nezorflame/armenian-blackouts-bot/actions/workflows/go.yml) [![Go Report Card](https://goreportcard.com/badge/github.com/nezorflame/armenian-blackouts-bot)](https://goreportcard.com/report/github.com/nezorflame/armenian-blackouts-bot) [![GolangCI](https://golangci.com/badges/github.com/nezorflame/armenian-blackouts-bot.svg)](https://golangci.com/r/github.com/nezorflame/armenian-blackouts-bot)

Bot which allows you to be notified about the utilities' blackouts in Armenia.

## Description

TODO

## Dependencies

This bot uses:

- [telebot](https://pkg.go.dev/gopkg.in/telebot.v3) package to work with Telegram API
- [bolt](https://pkg.go.dev/go.etcd.io/bbolt) for the database
- [envconfig](https://pkg.go.dev/github.com/kelseyhightower/envconfig) + [godotenv](https://pkg.go.dev/github.com/joho/godotenv) for the configuration
- [slog](https://pkg.go.dev/log/slog) for the logging

## Structure

This project mostly adheres to the [Project Layout](https://github.com/golang-standards/project-layout) structure, excluding `pkg` folders.

`internal` package holds the private libraries:

- `config` for configuration
- `bolt` for database (using BoltDB)
- `file` for file and network helpers
- `telegram` package with bot implementation
