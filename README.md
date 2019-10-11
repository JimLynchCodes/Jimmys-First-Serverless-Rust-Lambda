# Jimmys-First-Serverless-Rust-Lambda
My first AWS Lambda function written in Rust


## Usage

1. Clone this repo
```
git clone ...
```

2. Install the "serverless-rust plugin".
```
npm i -D serverless-rust
```

3. Navigate into project directory:
```
cd jimmys-first-rust-lambda
```

3. Install node dependencies:
```
npm i
```

4. Then you will need to build the project (for some reason this is done with the deploy command)
```
npx serverless deploy
```

Then you should be able to invoke the lambda function locally:
```
npx serverless invoke -f hello -d '{"foo":"bar"}'
```

## Scaffolding
This project was created from the [serverless-aws-rust](https://github.com/softprops/serverless-aws-rust) project with this command:
```
npx serverless install \
  --url https://github.com/softprops/serverless-aws-rust \
  --name jimmys-first-rust-lambda
```