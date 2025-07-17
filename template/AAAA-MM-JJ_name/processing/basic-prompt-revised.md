---
name: Basic Prompt
description: A basic prompt that uses the GPT-3 chat API to answer questions
version: 1.0.0
Date: 2025-07-17T12:33:00Z
Type: zero-shot 
Patterns: pat-001, pat-002, pat-546
model:
  api: chat
  configuration:
    type: azure_openai
    azure_deployment: gpt-35-turbo
    api_key: ${env:AZURE_OPENAI_API_KEY}
    api_version: ${env:AZURE_OPENAI_API_VERSION}
    azure_endpoint: ${env:AZURE_OPENAI_ENDPOINT}
  parameters:
    max_tokens: 128
    temperature: 0.2
inputs:
  first_name:
    type: string
  last_name:
    type: string
  question:
    type: string
sample:
  first_name: John
  last_name: Doe
  question: Who is the most famous person in the world?
---
copy/paste here result from the AI agent

NB: adapt yaml properties to your needs
