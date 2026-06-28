# NLP SMS Spam Detection

A machine learning project to detect spam SMS messages using natural language processing techniques.

## Project Overview

This project implements an SMS spam detection system using machine learning. It performs:
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data preprocessing and balancing
- Model training and evaluation

## Dataset

The project uses the Combined Enron dataset for SMS spam detection.

### Key Statistics
- **Total Messages**: 33,829
- **Spam Messages**: 17,157
- **Ham Messages**: 16,672
- **Dataset Balance**: Nearly balanced (50/50 split after preprocessing)

## Features Engineered

1. **word_count**: Number of words in each message
   - Spam messages: typically 15-30 words
   - Ham messages: below 25 words

2. **contains_currency_symbol**: Detects presence of currency symbols (€, $, ¥, £, ₹)
   - ~1/3 of spam messages contain currency symbols
   - Rarely used in ham messages

3. **contains_number**: Detects presence of numeric digits
   - Helps differentiate between message types

## Project Structure

