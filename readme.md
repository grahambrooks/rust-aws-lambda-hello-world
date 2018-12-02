# Sample Rust Lambda Hello World function

Sample described here:

https://aws.amazon.com/blogs/opensource/rust-runtime-for-aws-lambda/


    ./dev-setup
    
Sets up the local dev environment

    ./build
    
creates a rust.zip of the lambda function for deployment


Once deployed (as graham-test-rust) call the function through the console https://console.aws.amazon.com/lambda/home?region=us-east-1#/functions or command line

    aws lambda invoke --function-name graham-test-rust --payload '{"firstName": "World"}' output.json;cat output.json
    
