## Local Setup

### Requirments
- Python 2.7
- Virtual Environment
- pip
- Boto3
  - Boto3 is installed as part of the lambda functions Environment.  To aviod the overhead of including it in your deployment artifact install boto3 on your system instead of in the virtual environment
- awscli (configured)

### Setup
From the repo root dir
``` bash
$ virtualenv venv
$ pip install -r requirements.txt
```


## Sample Task Definition

``` yaml
name: sample name
expression: "0 2 * * *"
queue_name: some-sqs-queue
task:
  key1: value 1
  key2: value 2
```
