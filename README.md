# seattle-nginx

This sample Docker container creates a small skyline picture.
The background color is dependent upon the time of day.

This container has already been built and pushed into my GCR repo.

# For GCP Cloud Run
# The default port is 8080, so we must alter it
gcloud run deploy --image gcr.io/nicks-playground-3141/seattle-nginx:latest --port 80

# Delete the service
gcloud beta run services delete seattle-nginx
