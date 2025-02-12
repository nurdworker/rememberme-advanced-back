### **Backend**

1. **Clone our project repository**

```bash
git clone https://github.com/nurdworker/rememberme-advanced-back
```

2. **Install AWS SAM CLI**

- Windows
  - Download the installer from the [AWS SAM CLI Download Page](https://aws.amazon.com/serverless/sam/).
  - Run the installer and follow the on-screen instructions.
  - Add the installation path (usually `C:\Program Files\Amazon\AWSSAMCLI\bin`) to your `PATH` environment variable if not automatically configured.
- macOS
  - Install using Homebrew:
  ```bash
  brew install aws/tap/aws-sam-cli
  ```

3. **Build and Test API Gateway with Lambda**
   To build the API Gateway and Lambda environment using SAM, run:

```bash
sam build --no-cached
sam local start-api --env-vars ./env.json --no-cached
```

**env.json for SAM CLI**

```json
{
  "<lambda-name-1>": {
    "ENV_FIRST": "...",
    "ENV_SECOND": "///"
  },
  "<lambda-name-2>": {
    "ENV_FIRST": "...",
    "ENV_SECOND": "///"
  }
}
```

The added warning ensures users understand that **environment variables** are **crucial** for the proper functioning of Lambda functions and must be specified correctly in the `env.json` file.
