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
│   │           │   ├── ... (many)
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