#### Example Starting Structure
```
obsidian-glade/
├── .github
│   └── workflows
│       ├── ci.yml
│       └── cd.yml
├── crates
│   ├── user_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   ├── item_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   ├── trade_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   ├── chat_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   ├── npc_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   ├── time_service
│   │   ├── src
│   │   ├── tests
│   │   └── Cargo.toml
│   └── common
│       ├── src
│       ├── tests
│       └── Cargo.toml
├── docker
│   ├── user_service
│   │   └── Dockerfile
│   ├── item_service
│   │   └── Dockerfile
│   ├── trade_service
│   │   └── Dockerfile
│   ├── chat_service
│   │   └── Dockerfile
│   ├── npc_service
│   │   └── Dockerfile
│   ├── time_service
│   │   └── Dockerfile
│   └── db
│       ├── init.sql
│       └── Dockerfile
├── kubernetes
│   ├── user_service-deployment.yaml
│   ├── item_service-deployment.yaml
│   ├── trade_service-deployment.yaml
│   ├── chat_service-deployment.yaml
│   ├── npc_service-deployment.yaml
│   ├── time_service-deployment.yaml
│   ├── database-deployment.yaml
│   └── ingress.yaml
├── .dockerignore
├── .gitignore
├── README.md
├── LICENSE
└── Cargo.toml
```