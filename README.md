### Rotes Navigations


> /api/v1/faqs?lang=hindi(bangali, punjabi,kannada)
    --> Returns language in hindi , bangali, punjabi, kannada only  if available (most probably since the ai is doing)
    

> /api/v1/faqs?id=idOfTheFAQ&lang=language(hindi,benagali like that)
        ---> Returns the Faq Contaning id translated to the lang
        
> /api/faqs?id=idOfTheFAQ
        --> Returns specific FAQ by ID


## Overview 

This is a multi-language FAQ system built with Node.js and Express.js, designed to handle frequently asked questions efficiently. It supports rich-text formatting, automatic translations, and high-performance caching for a seamless user experience.

## Features
REST API for managing FAQs (Create, Read, Update, Delete)
Multi-language support
Rich-text formatting using 
Faster responses
MongoDB support


## Security Note: Google API Keys

API keys for Google Translate are NOT included in this repo to prevent exposure of sensitive credentials. To use translations:

Obtain a Google Cloud API Key from Google Cloud Console.

Store it securely in .env file:

GOOGLE_API_KEY=your_api_key_here

Use it in your code like this:

const API_KEY = process.env.GOOGLE_API_KEY;

