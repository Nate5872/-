# -
name: CI on: push jobs:   prod-check:     if: ${{ github.ref == 'refs/heads/main' }}     runs-on: ubuntu-latest     steps:       - run: echo "Deploying to production server on branch $GITHUB_REF"
