# Attendify Billing

FOSSBilling Docker container with basic CI/CD pipeline.

## Local Development

To run the FOSSBilling container locally:

```bash
cd Docker/fossbilling-docker
docker-compose up -d
```

Access the application at http://localhost:8080

## CI/CD Pipeline

This repository includes a basic GitHub Actions CI/CD pipeline that:

1. Triggers automatically when:
   - You push to the main branch
   - You create a pull request to the main branch
   - Only when changes are made in the Docker directory

2. The pipeline will:
   - Build the Docker containers
   - Start the services
   - Test if the application is accessible
   - Clean up after testing

### Setup Requirements

1. Enable GitHub Actions in your repository settings
2. That's it! The pipeline will run automatically when you push changes

After the guest lecture on CI/CD, we can enhance this pipeline with additional features and best practices.
