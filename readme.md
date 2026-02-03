# n8n Workflow Backup Automation

This repository contains an n8n automation workflow designed to automatically back up all workflows from an n8n instance to a GitHub repository, ensuring version control, redundancy, and operational safety. Each workflow is stored as a JSON file.

## 🧠 Problem Solved

Accidental deletions, failed updates, or instance issues can result in the permanent loss of critical automations. This workflow solves that problem by automatically exporting all n8n workflows and storing them as versioned files in GitHub without manual intervention.

## 💡 Workflow Summary

- The workflow runs automatically on a defined schedule, ensuring regular backups without human interaction.
- Checks the target GitHub repository to retrieve the list of existing backup files and get all workflows from the n8n instance using the internal n8n API.
- If A backup file already exists → Update File
- IF A backup file does not exist → Create File

## 📸 Workflow Preview
<img width="1504" height="708" alt="image" src="https://github.com/user-attachments/assets/1f93dac6-c62d-4ba5-b78d-d683ff5bfbc0" />
