# YaMDb (Server Edition) #
*This is the version of API service YaMDb which automatically deploys to private server on every push via GitHub Actions. Virtual machine stopped for now so you can read full description of the project and try out dockered local edition of YaMDb here: https://github.com/Immalakhovskii/yamdb_docker*
****
#### Technology Stack ####
Python 3.7 / Django 2.2.16 / Django REST framework 3.12.4 / Docker 20.10.17 / PostgreSQL 13.0
#### GitHub Actions ####
On every push to GitHub the project has workflow with 5 ateps:
- Flake8 tests
- Custom tests
- Build and push updated backend Docker image to Docker Hub
- Deploy project on server
- Send message in Telegram after successful deploy

![Workflow badge](https://github.com/Immalakhovskii/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?event=push)

*Workflow fails now because of failing deploy on server*
