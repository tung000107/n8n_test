# How to run n8n
- Install docker
- run `vi docker-compose.yml`
- input
```
volumes:
  n8n_storage:
services:
  n8n:
    image: n8nio/n8n:latest
    restart: always
    ports:
      - "127.0.0.1:5678:5678" 
    volumes:
      - n8n_storage:/home/node/.n8n
      - /Users/***/n8n:/home # mount docker directory to local directory
```
- docker-compose up


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
1. Open n8n host with `http://localhost:5678/`
2. Create New Workflow
3. Click `...` and choose `Import from file`
4. Choose `Project1.json`
5. Create a specific folder and upload related file or reference on your google drive
6. Setup the folder of the Google drive trigger inside the workflow

# Project2 - 文件去機密化
1. Open n8n host with `http://localhost:5678/`
2. Create New Workflow
3. Click `...` and choose `Import from file`
4. Choose `Project2.json`
5. Put your file which you want to be processed inside the mounted directory
6. Click the trigger button

## Prompt (reviewing)
```
0. Remove the file type from the content
1. Find all personal information from the file
2. Use random information to instead those personal information
3. Output all text from the file.
Don't need to speak other, just follow the point above
```



