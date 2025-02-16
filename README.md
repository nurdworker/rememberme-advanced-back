# Remember Me

A serverless vocabulary memorization website built on AWS Lambda.

📢 **한국인 분들은 블로그 보시면 됩니다. 훨씬 정리 잘 되어 있어요!**
👉 [블로그 링크](https://blog.nurd.work/357)

Copyright (c) 2025 Nurd Worker. All rights reserved.
Contact: nurdworker@gmail.com

### 🎬 Implementation Advanced Version Video:

- 🎥[Video Link_korean](https://www.youtube.com/watch?v=MEIIWAcPjt0)

## Tech Stack

- Frontend : React, Tailwind, TypeScript, Redux
- Backend: : Node.js, AWS SAM CLI
- Database : MongoDB
- Cloud(AWS) : Lambda, API Gateway, Secrets Manager, Api Gateway, SNS, Cloud Watch

## Development

1. **Clone our project repository**

```bash
git clone https://github.com/nurdworker/rememberme-advanced-back.git
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

## Copyright

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to use, modify, and
distribute the Software under the following conditions:

1. The Software may be used, modified, and distributed for **personal use only**.
2. The Software may **not be used for any commercial purposes** or any business-related activities.
3. The Software may **not be used in personal portfolios or any personal projects**.
4. The Software may **not be redistributed for commercial purposes**.

Any use of the Software that does not comply with these conditions is strictly prohibited.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

이 소프트웨어 및 관련 문서 파일(이하 "소프트웨어")의 복사본을 얻은 모든 사람에게, 다음 조건에 따라 소프트웨어를 사용하고 수정하며 배포할 수 있는 권한이 부여됩니다:

1. 소프트웨어는 **개인적인 용도에만** 사용하고 수정하며 배포할 수 있습니다.
2. 소프트웨어는 **상업적 목적**이나 사업 관련 활동에 사용될 수 없습니다.
3. 소프트웨어는 **개인 포트폴리오**나 **개인 프로젝트**에 사용될 수 없습니다.
4. 소프트웨어는 **상업적 목적으로 재배포**할 수 없습니다.

이 조건을 준수하지 않는 소프트웨어의 사용은 엄격히 금지됩니다.

소프트웨어는 "있는 그대로" 제공되며, 명시적이거나 묵시적인 보증 없이 제공됩니다. 여기에는 상업성, 특정 목적에 대한 적합성 및 비침해에 대한 보증이 포함되나 이에 한정되지 않습니다. 저자나 저작권자는 소프트웨어의 사용 또는 기타 거래와 관련하여 발생하는 어떠한 청구, 손해 또는 기타 책임에 대해서도 책임지지 않습니다.
