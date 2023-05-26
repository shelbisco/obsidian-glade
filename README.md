# Plot and Mechanics
**Name: Obsidian Glade**

**Idea**: Obsidian Glade is a cozy, easygoing online platform with social and gaming features. It's set in a gothic, supernatural world where each player creates and customizes an NPC (Non-Player Character) to represent them in the game world.

**Project Structure**:

1. **Rust Web Server (Nocturnal Realms API)**: Handles operations like NPC creation, managing gardens, items, and in-game chat.
    
2. **Containerized Microservices**: Manage separate components of the game such as NPC Service, Garden Service, Item Service, and Chat Service.
    
3. **Deployment on Kubernetes**: Each microservice is deployed as a separate pod within a Kubernetes cluster.
    
4. **CI/CD Pipeline with GitHub Actions/Jenkins**: Automate testing, building, and deployment.
    
5. **Rust Command Line Tool (Obsidian Glade CLI)**: A tool for game management tasks and moderation.
    
6. **Infrastructure Automation with Terraform**: Automate the setup of the cloud infrastructure.
    
7. **Cloud-Native Game Application (Obsidian Glade)**: Develop a frontend for players to interact with the game world and manage their NPCs.
    

**Gameplay Mechanics**:

1. **Character Customization**: Players create and customize their NPC's personality, goals, and behavior.
    
2. **Gardening & Potion Making**: NPCs can cultivate a garden and create potions from harvested herbs. These potions can be used or traded.
    
3. **Daily Challenges**: NPCs complete tasks for rewards.
    
4. **Cozy Corners**: NPCs can customize their living space. Other NPCs can visit and rate each other's corners.
    
5. **Mini-games**: Occasional trivia contests or treasure hunts engage the players.
    
6. **Pet Companions**: NPCs can adopt and care for mythical pets that aid in tasks.
    
7. **NPC Goals and Behaviors**: NPCs perform tasks autonomously based on the goals and behavior settings determined by their players.
    
8. **AI Conversations**: NPCs communicate with each other based on their programmed personalities and goals.

## Example Starting Structure
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