This Project utilizes AWS IoT Device SDK v2 for Python to connect and communicate MQTT messages between the server and AWS IoT Core. Downstream wrapping can be performed in AWS Console.

This document provides information about the AWS IoT Device SDK v2 for Python. This SDK is built on the [AWS Common Runtime](https://docs.aws.amazon.com/sdkref/latest/guide/common-runtime.html)

## Installation

### Minimum Requirements
* Python 3.7+

### Install from source

```bash
# 1. Create a workspace directory to hold all the SDK files
mkdir sdk-workspace
cd sdk-workspace

# 2. Clone the repository. You could select the version of the SDK you desire to use.
git clone -b <SDK_VERSION> https://github.com/aws/aws-iot-device-sdk-python-v2.git

# 3. (Optional) Setup the version number of your local build. The default version 
#    for awsiotsdk is set to "1.0.0-dev", you can set the version number of the
#    local build in "aws-iot-device-sdk-python-v2/awsiot/__init__.py"
sed -i "s/__version__ = '1.0.0-dev'/__version__ = '<SDK_VERSION>'/" \
  aws-iot-device-sdk-python-v2/awsiot/__init__.py

# 4. Install using Pip (use 'python' instead of 'python3' on Windows)
python3 -m pip install ./aws-iot-device-sdk-python-v2
```
