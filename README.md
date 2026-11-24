# Database ETL Pipeline

A Docker-based ETL project for transferring data between SQLite, PostgreSQL, and Elasticsearch.

## Components

- **sql_to_pg** — transfers data from SQLite to PostgreSQL.
- **postgres_to_es** — transfers data from PostgreSQL to Elasticsearch.
- **database** — PostgreSQL database initialization and fixtures.

## Technology Stack

- Python
- SQLite
- PostgreSQL
- Elasticsearch
- Docker
- Docker Compose

## Getting Started

### Configuration

Create environment files using the provided examples:

```bash
cp dbvars_example.env dbvars.env
cp webvars_example.env webvars.env
```

Configure the required environment variables.

### Running with Docker Compose

```bash
docker-compose up --build
```

### Local Run

```bash
./local_run.sh
```

## Project Structure

```text
.
├── database/       # Database initialization
├── sql_to_pg/      # SQLite to PostgreSQL transfer
├── postgres_to_es/ # PostgreSQL to Elasticsearch transfer
├── docker-compose.yml
└── local_run.sh
```
