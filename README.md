# AI Lead Qualification & Routing System

An AI-powered lead qualification system built with n8n to automatically evaluate, score, classify, and route incoming leads.

The system was designed around a real estate use case for HavenGate Properties, helping the sales team quickly identify leads that require attention.

## Overview

The workflow collects lead information through Google Forms and uses Google Gemini to analyse each lead based on factors such as property interest, budget, location, timeline, and level of intent.

Each lead receives a score and is classified as:

- HOT
- WARM
- COLD

The system also generates a short summary, explains the reason for the classification, and recommends the next action.

The results are stored in Google Sheets, while relevant lead information is sent to the sales team through Slack.

## How It Works

1. A lead submits their information through Google Forms.
2. The response is recorded in Google Sheets.
3. n8n detects the new lead and starts the workflow.
4. Lead information is sent to Google Gemini for analysis.
5. Gemini evaluates the lead and generates a score and classification.
6. The workflow routes the lead based on the classification.
7. The qualification result is stored in Google Sheets.
8. The sales team receives a Slack notification.

## Workflow

Google Forms  
↓  
Google Sheets  
↓  
n8n  
↓  
Google Gemini  
↓  
Lead Qualification  
↓  
HOT / WARM / COLD  
↓  
Google Sheets + Slack

## Key Features

- AI-powered lead qualification
- Automated lead scoring
- HOT / WARM / COLD classification
- AI-generated qualification reasoning
- Recommended next action
- Automated Slack notifications
- Centralized lead tracking

## Tech Stack

- n8n - Workflow automation
- Google Gemini - AI-powered lead analysis
- Google Forms - Lead collection
- Google Sheets - Lead data and qualification results
- Slack - Sales-team notifications
- APIs & Webhooks - System integration
- JSON - Data exchange and structured workflow output

