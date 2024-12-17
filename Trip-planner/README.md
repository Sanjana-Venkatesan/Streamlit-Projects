# Trip Planner Crew (Uses crew AI)

## Overview

The Trip Planner Crew is a web application designed to help users plan their perfect trip. It utilizes artificial intelligence and various tools to analyze cities, gather local insights, and provide personalized travel itineraries. The app generates a detailed trip plan based on the user's preferences, such as city selection, activities of interest, and travel dates.

## Features

- **City Selection**: Analyze and select the best city for your trip based on criteria such as weather, seasonal events, and travel costs.
- **Local Expertise**: Gather in-depth guides about the city's attractions, culture, customs, and hidden gems, with personalized recommendations.
- **Travel Itinerary Planning**: Generate a complete 7-day travel itinerary, including daily plans, suggested restaurants, packing lists, and a detailed budget breakdown.
- **Real-time Data**: Fetch real-time data for weather forecasts, flight costs, and seasonal events using external tools.
- **User-Friendly Interface**: Simple input fields for users to specify their travel preferences and get a detailed trip plan.

## Requirements

- Python 3.x
- Streamlit
- CrewAI
- LangChain
- Requests
- BeautifulSoup
- unstructured

### To Install Dependencies:

```bash
pip install -r requirements.txt
```

## Setup

1. **API Keys**: 
   - You will need an API key for Google's Gemini model. Replace the placeholder `<api key>` with your actual key in the `llm` initialization.

2. **Streamlit App**: 
   - Run the app using the following command:
   
   ```bash
   streamlit run app.py
   ```

3. **Customizing the Application**:
   - Modify the agent roles, tasks, and data fetching logic according to your needs.

## How It Works

1. **User Input**: 
   - Users enter the following information:
     - **Location**: Where they are traveling from.
     - **City Options**: The cities they are considering visiting.
     - **Date Range**: Their preferred travel dates.
     - **Interests**: High-level preferences and hobbies.

2. **AI Tasks**: 
   - The app assigns specific tasks to AI agents:
     - **City Selection**: The first agent analyzes the cities based on criteria like weather, season, and costs.
     - **Local Expertise**: The second agent provides a detailed guide on the selected city, including hidden gems, local customs, and recommendations.
     - **Travel Itinerary**: The final agent builds a complete itinerary, including a daily plan, restaurant suggestions, and budget breakdown.

3. **Output**: 
   - The result is a comprehensive trip plan displayed in the app, showing the itinerary, attractions, and other important details.

## Example Input & Output

**Input**:
- **Location**: "New York"
- **City Options**: "Paris, Tokyo, Barcelona"
- **Date Range**: "June 2024"
- **Interests**: "Museums, local cuisine, historical landmarks"

**Output**: 
- A detailed report on the best city to visit, a local guide to the city, and a full 7-day itinerary including places to visit, restaurants, packing tips, and budget.

## Tools & Libraries Used

- **Streamlit**: Used to create the web interface for input and displaying the result.
- **CrewAI**: Helps in managing and executing tasks with AI agents to select cities and generate detailed travel plans.
- **LangChain**: Facilitates integration with Google's Gemini model to generate responses and handle large language model-based tasks.
- **BeautifulSoup**: For scraping website content to gather real-time data.
- **unstructured.partition.html**: Used for processing and extracting meaningful data from HTML files.
- **Requests**: Makes HTTP requests to fetch web content and search results.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Contributions are welcome to improve the app's features, enhance the UI/UX, or fix bugs.

## License

This project is licensed under the MIT License.
