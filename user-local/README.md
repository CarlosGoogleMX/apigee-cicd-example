gcloud beta builds triggers create cloud-source-repositories \
    --repo="interoperabilidad-telemedicina" --branch-pattern='.*' --name="cicd-example" \
    --build-config='user-local/cloudbuild/cloudbuild.yaml' \
    --substitutions="_API_VERSION=google,_DEPLOYMENT_ORG=worstation-379213,_APIGEE_TEST_ENV=dev,_INT_TEST_HOST=https://mocktarget.apigee.net"
    