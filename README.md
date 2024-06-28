# hexagonal-jwt


# Dir Architecture
```
.
├── LICENSE
├── cmd
│   └── http
│       └── main.go
├── go.mod
├── go.sum
├── internal
│   ├── adapter
│   │   ├── auth
│   │   │   └── token
│   │   │       └── token.go
│   │   ├── config
│   │   │   └── config.go
│   │   ├── handler
│   │   │   └── http
│   │   │       ├── auth.go
│   │   │       ├── dto
│   │   │       │   ├── auth.go
│   │   │       │   ├── general.go
│   │   │       │   └── user.go
│   │   │       ├── middleware
│   │   │       │   └── middleware.go
│   │   │       ├── myerror
│   │   │       │   └── handler.go
│   │   │       ├── router
│   │   │       │   └── router.go
│   │   │       └── user.go
│   │   └── persistence
│   │       └── mysql
│   │           ├── database.go
│   │           ├── ent
│   │           │   ├── client.go
│   │           │   ├── ent.go
│   │           │   ├── enttest
│   │           │   │   └── enttest.go
│   │           │   ├── generate.go
│   │           │   ├── hook
│   │           │   │   └── hook.go
│   │           │   ├── intercept
│   │           │   │   └── intercept.go
│   │           │   ├── internal
│   │           │   │   └── schema.go
│   │           │   ├── migrate
│   │           │   │   ├── migrate.go
│   │           │   │   └── schema.go
│   │           │   ├── mutation.go
│   │           │   ├── predicate
│   │           │   │   └── predicate.go
│   │           │   ├── runtime
│   │           │   │   └── runtime.go
│   │           │   ├── runtime.go
│   │           │   ├── schema
│   │           │   │   ├── timemixin.go
│   │           │   │   └── user.go
│   │           │   ├── tx.go
│   │           │   ├── user
│   │           │   │   ├── user.go
│   │           │   │   └── where.go
│   │           │   ├── user.go
│   │           │   ├── user_create.go
│   │           │   ├── user_delete.go
│   │           │   ├── user_query.go
│   │           │   └── user_update.go
│   │           ├── migration.go
│   │           ├── repository
│   │           │   └── user.go
│   │           └── utils
│   │               └── sugar.go
│   └── core
│       ├── domain
│       │   ├── token_payload.go
│       │   ├── types.go
│       │   └── user.go
│       ├── port
│       │   ├── auth.go
│       │   ├── token.go
│       │   └── user.go
│       ├── service
│       │   ├── auth.go
│       │   └── user.go
│       └── util
│           └── password.go
└── pkg
    └── errors
        └── errors.go
```