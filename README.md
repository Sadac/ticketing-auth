# Auth service

## Start project
```npm start```

## Basic setup
1. Init the project `npm init -y`
2. Install dependencies `npm install typescript ts-node-dev express @types/express` make sure you install typescript globally in order to use the `tsc` command line
3. Generate a ts config file `tsc --init`
4. Create the src/index.ts and basic express server
5. Configure a init script in package.json
```sh
"scripts": {
  "start": "ts-node-dev src/index.ts"
}
```
6. Create the Dockerfile to build the image and .Dockerignore to add the node_modules
7. Build the image `docker build -t roccosada/auth .`
8. Load the image into the kubernetes cluster within a Deployment

