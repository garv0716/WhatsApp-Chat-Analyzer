# WhatsApp Chat Analyzer

A powerful **data analytics web application** built using **Python** and **Streamlit** that transforms exported WhatsApp chats into meaningful insights and interactive visualizations.

Whether it's personal conversations or large group discussions, this application helps users understand communication patterns, engagement levels, activity trends, and user behavior through data-driven analysis.

---

## Overview

The WhatsApp Chat Analyzer allows users to upload exported WhatsApp chat files and generate detailed statistics and visual reports. The application supports both **individual chats** and **group conversations**, making it useful for exploring interaction patterns in different contexts.

---

## Features

### Chat Statistics

Obtain key metrics from the uploaded chat, including:

- Total number of messages sent
- Total number of words exchanged
- Number of media files shared
- Number of links shared

---

### User-wise Analysis

For group chats, the application provides participant-level insights such as:

- Most active users based on message count
- Percentage contribution of each participant
- Individual chat statistics for selected users

---

### Timeline Analysis

Analyze how chat activity changes over time through:

#### Monthly Timeline

Displays message activity month by month to identify long-term trends.

#### Daily Timeline

Shows the distribution of messages across different dates.

---

### Activity Analysis

Understand when users are most active by exploring:

#### Most Active Day

Identifies the day of the week with the highest number of messages.

#### Most Active Month

Determines the month with the greatest overall activity.

#### Weekly Activity Heatmap

Visualizes chat intensity across different days and hours to reveal behavioral patterns.

---

### Word Cloud Generation

Creates a visual representation of frequently used words within the conversation, helping identify major discussion topics.

---

### Most Common Words Analysis

Lists the most frequently occurring words after removing stop words and irrelevant text.

This feature helps uncover the dominant themes within a chat.

---

### Emoji Analysis

Provides insights into emoji usage patterns, including:

- Most frequently used emojis
- Frequency distribution of emojis
- Percentage contribution of individual emojis

---

### URL Analysis

Detects and counts all hyperlinks shared within the conversation.

This helps understand information-sharing behavior among participants.

---

### Support for Different Chat Types

The application can analyze:

- One-to-one conversations
- Group chats

---

## Technology Stack

| Technology | Purpose |
|------------|----------|
| Python | Core programming language |
| Streamlit | Web application framework |
| Pandas | Data processing and manipulation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualizations |
| WordCloud | Word cloud generation |
| URLExtract | URL extraction |
| Emoji | Emoji processing |
| Regular Expressions (re) | Chat parsing and preprocessing |

---

## Project Structure

```text
WhatsApp-Chat-Analyzer/
│
├── app.py
│   └── Main Streamlit application
│
├── helper.py
│   └── Functions for statistical analysis and visualization
│
├── preprocessor.py
│   └── Chat preprocessing and data cleaning logic
│
├── stop_hinglish.txt
│   └── Stop words used during text analysis
│
├── requirements.txt
│   └── Project dependencies
│
└── README.md
```

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/whatsapp-chat-analyzer.git

cd whatsapp-chat-analyzer
```

---

### 2. Create a Virtual Environment (Recommended)

#### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

#### macOS/Linux

```bash
python3 -m venv venv

source venv/bin/activate
```

---

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4. Launch the Application

```bash
streamlit run app.py
```

The application will automatically open in your default web browser.

---

## Exporting WhatsApp Chats

Before using the analyzer, export the desired chat from WhatsApp.

### Android

1. Open WhatsApp.
2. Open the required chat.
3. Tap the three-dot menu.
4. Select **More** → **Export Chat**.
5. Choose **Without Media**.
6. Save the exported `.txt` file.

---

### iOS

1. Open WhatsApp.
2. Open the desired chat.
3. Tap the contact or group name.
4. Scroll down and select **Export Chat**.
5. Choose **Without Media**.
6. Save the exported `.txt` file.

---

## Usage

1. Start the application.

```bash
streamlit run app.py
```

2. Upload the exported WhatsApp chat file.

3. Choose one of the following options:

- **Overall Analysis** for complete chat insights.
- **User-specific Analysis** to explore statistics for an individual participant.

4. Click the **Show Analysis** button.

5. Review the generated statistics and visualizations.

---

## Insights Generated

The application can help answer questions such as:

- Who contributed the most messages in the group?
- Which month had the highest level of activity?
- During which hours are participants most active?
- What are the most frequently used words?
- Which emojis are used most often?
- How many links have been shared?
- What percentage of the conversation does each user contribute?

---

## Requirements

```text
streamlit
pandas
matplotlib
seaborn
wordcloud
urlextract
emoji
numpy
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## Future Enhancements

Possible improvements include:

- Sentiment analysis of conversations
- Topic modeling using Natural Language Processing
- Reply network visualization
- PDF report generation
- Date range filtering
- Support for additional languages
- Enhanced user interface customization

---

## Contributing

Contributions are welcome.

To contribute:

1. Fork the repository.
2. Create a new branch.

```bash
git checkout -b feature-name
```

3. Commit your changes.

```bash
git commit -m "Add new feature"
```

4. Push the branch.

```bash
git push origin feature-name
```

5. Open a Pull Request.

---

## License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this software in accordance with the license terms.

---

## Acknowledgements

This project was developed as a learning experience in data analysis and web application development using Python.

Special thanks to **CampusX** and **Mr. Nitish Singh**, whose educational content and project-based teaching approach served as a major source of inspiration and guidance during the development of this project.

The project also makes use of several excellent open-source libraries and frameworks, including:

- Streamlit
- Pandas
- Matplotlib
- Seaborn
- WordCloud
- URLExtract
- Emoji

Their contributions to the open-source community have made projects like this possible.
