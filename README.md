pgbackup
========

CLI for backing up remote PostgresSQL databases locally or to AWS S3.

## Usage

Pass in a full database URL, the storage driver and destination.

S3 Example w/ bucket name:

```
$ pgbackup postgres://tom@example.com:5432/db_one -- driver S3 backups
```

Local Example w/ local path:

```
$ pgbackup postgres://tom@example.com:5432/db_one -- driver local /var/local/db_one/backups
```

## Installation From Source

To install the packages after you've cloned the repository, you'il want to run the following command from within the project directory:

```
pip install --user -e .
```

## Preparing For Development

Follow these steps to start developing with this project

1. Ensure `pip` and `pipenv` are installed
2. Clone repository: `git clone git@github.com:example/pgbackup`
3. `cd` into repository
4. Activiate virtualenv: `pipenv shell`
5. Install dependencies: `pipenv install`

