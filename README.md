# UwUlytics: Social Media Performance Dashboard 🎀

UwUlytics is a user-friendly social media analytics dashboard designed to help content creators, marketers, and analysts visualize and understand the performance of their social media posts. With insightful visualizations and actionable recommendations, it’s your go-to tool for improving engagement across various content types.

---

## Features

- **Customizable Analysis**: Select content types like Text, Image, Video, Reels, or Carousel to focus your analysis.
- **Performance Metrics**: View average likes, shares, comments, reach, and engagement rates for selected content types.
- **Visualizations**: Interactive pie charts and bar graphs to explore post performance.
- **Key Insights**: Highlighted insights tailored to the selected content types.
- **Recommendations**: Actionable suggestions to improve engagement.
- **Comparative Analysis**: Side-by-side comparisons of different content types.

---

## Technology Stack

- **Frontend**: [Streamlit](https://streamlit.io/)
- **Visualizations**: [Plotly](https://plotly.com/)
- **Data Handling**: [Pandas](https://pandas.pydata.org/)
- **Database**: [Astra DB](https://www.datastax.com/astra)
- **Language Model**: [Langflow](https://langflow.dev/)

---

## Workflow Overview

![Uploading image.png…]()

UwUlytics leverages Langflow for creating an AI-driven workflow with the following components:

1. **Astra DB Tool Component**: Fetches data from Astra DB and passes it to subsequent components.
2. **Custom Component**: Calculates the average values of likes, shares, comments, and reach for each content type.
3. **Chat Input Component**: Accepts user input specifying the post type to analyze.
4. **Prompt Component**: Combines user input and calculated average data to create a prompt.
5. **Gemini Model Component**: Processes the prompt to generate insights and recommendations in JSON format.
6. **Output to User**: Displays insights, comparative analysis, and actionable recommendations through the dashboard.

---

## Installation

Follow these steps to set up UwUlytics locally:

### Prerequisites
- Python 3.8+
- pip or a similar package manager
- Astra DB credentials (Contact your administrator for access)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/username/uwulytics.git
   cd uwulytics
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add Astra DB credentials:
   - Place your Astra DB credentials (`secure_connect.zip`) in the `./src/data` directory.
   - Unzip the file and ensure `secure_connect_bundle.json` is accessible.

4. Run the application:
   ```bash
   streamlit run app.py
   ```

5. Open your browser at `http://localhost:8501` to access the dashboard.

---

## Usage

1. Launch the dashboard by running the Streamlit app.
2. Select content types you wish to analyze from the checklist.
3. Click on **Generate Insights 🚀** to fetch data and view performance metrics.
4. Explore visualizations, key insights, and recommendations tailored to your selected content types.

---

## Data Sources

- **Input File**: `social_media_final_draft.csv`
- **Database**: Astra DB for scalable and secure data storage.

---

## Authors & Acknowledgments

- Developed by **Barbie Girls in the Barbie World 🎀**
- Special thanks to:
  - [Langflow](https://langflow.dev/) for enabling advanced AI integration.
  - [Astra DB](https://www.datastax.com/astra) for powering our database needs.
  - Streamlit and Plotly for their amazing libraries.

