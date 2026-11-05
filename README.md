# Sonatype Policy Demo - PHP

This is a demo package for testing Sonatype policy functionality.

## Versions

- 1.0.0 - Normal status
- 1.1.0 - Malicious status
- 1.2.0 - Suspicious status
- 1.3.0 - Pending status

## Deployment Instructions (Composer / Packagist)

PHP packages managed by Composer are hosted in a version control system (like GitHub) and registered on Packagist.org.

1. Initialize Composer: Run composer init in your package directory to generate a composer.json file with proper PSR-4 autoloading and a vendor/package-name format:
   ```bash
   docker run --rm -v "$(pwd)":/app -w /app composer:latest composer init
   ```

2. Push to Version Control: Commit your code and push the repository to GitHub (or GitLab/Bitbucket):
   ```bash
   git add .
   git commit -m "Release v1.0.0"
   git push origin main
   ```

3. Submit to Packagist: Go to Packagist.org, sign in, click Submit, and paste your GitHub repository URL. Packagist will now index your package so others can install it via composer require username/repo-name.
