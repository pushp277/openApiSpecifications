# OpenApi Specifications

## auth-service
docker command:
```bash
cd authService
docker run --rm \
  -v ${PWD}:/local \
  openapitools/openapi-generator-cli:latest generate \
  -i /local/auth-service.yaml \
  -g spring \
  -o /local/target \
  --additional-properties=useSpringBoot3=true,interfaceOnly=true,useJakartaEe=true,javaVersion=21 \
   --skip-validate-spec
```
