# Summary

This repo is used to try out open api generator mainly using npm and use redoc to generate document page. Additionally, the code can also be generated through docker command.

## Use Npm to generate

```bash
# generate typescript-fetch with
npm run codegen:client
# generate expressjs server with
npm run codegen:server
# generate redoc document
npm run redoc
```

## Use Docker to generate

#[Open Api Generator](https://openapi-generator.tech/)

```bash
docker run --rm \
 -v ${PWD}:/local openapitools/openapi-generator-cli generate \
 -i /local/petstore.yaml \
 -g typescript-node \
 -o /local/out/typescript-node
```
