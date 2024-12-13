# MyLambdaFunction

## Overview
This project demonstrates a simple AWS Lambda function built with .NET. The function takes a string input and returns the uppercase version of the string.

## Prerequisites
- [.NET SDK 8.0.100](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- AWS CLI configured with appropriate permissions
- Visual Studio Code or any preferred text editor

## Project Structure
```
MyLambdaFunction/ 
├── MyLambdaFunction.sln
├── global.json
├── src/ 
│ ├── MyLambdaFunction/ 
│ │ ├── MyLambdaFunction.csproj
│ │ ├── Function.cs
│ │ ├── aws-lambda-tools-defaults.json
├── test/
│ ├── MyLambdaFunction.Tests.csproj
│ ├── FunctionTest.cs
```

## Setting Up the Environment 

### Step 1: Install .NET SDK 
Make sure the .NET SDK is installed on your machine. 
You can download it from the official [.NET website](https://dotnet.microsoft.com/en-us/download/dotnet/8.0). 

### Step 2: Restore the Packages 
Navigate to the root of your solution directory and run: 

```sh 
dotnet restore
```

### Step 3: Build the Solution
Run the following command to build the solution:

```sh 
dotnet build
```

### Step 4: Run the Tests
Run the following command to run tests:
```sh
dotnet test
```

### Step 5: Publish the Lambda Function
Run the following command to publish the solution:

```sh
dotnet publish -c Release -o publish
```

### Step 6: Create a ZIP Deployment Package
Create a ZIP file of the publish directory for deployment:

```sh
cd publish 
zip -r ../MyLambdaFunction.zip .
```



