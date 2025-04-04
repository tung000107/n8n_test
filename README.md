# How to run n8n
- Install docker
- `docker-compose up`
- Open n8n with `http://localhost:5678/`

# How to setup crenditals
## Google
url: https://console.cloud.google.com/


## OpenAI
url: https://platform.openai.com/docs/api-reference/introduction

## Supabase
url: https://supabase.com/docs/guides/api

## PostgreSQL
應用supabase的database

# Project1 - 宣傳文案與故事輸出
1. Create New Workflow
2. Click `...` and choose `Import from file`
3. Choose `Project1.json`
4. Create a specific folder and upload related file or reference on your google drive
5. Setup the folder of the Google drive trigger inside the workflow

# Project2 - 文件去機密化
1. Create New Workflow
2. Click `...` and choose `Import from file`
3. Choose `Project2.json`
4. Put your file which you want to be processed inside the mounted directory
5. Click the trigger button

## Prompt (reviewing)
```
Upload a document. Replace all confidential or personal information with randomized placeholders while keeping the structure intact. Ensure that names, addresses, phone numbers, emails, and any other sensitive data are anonymized while keeping the document's structure intact. The result should be a template that maintains the original formatting and context without exposing any real information. Output only the modified document without extra commentary.
```



