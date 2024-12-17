# Pomodoro App 🍅⏳

A simple Pomodoro Timer built with **Streamlit** to help you stay focused and boost productivity. The app allows you to set a Pomodoro session (work time) and a break time. It also provides a simple interface to control your work and break intervals with start and stop options.

## Features

- **Customizable Session Duration**: You can choose the length of your Pomodoro work session (in minutes).
- **Break Timer**: After completing a Pomodoro session, a 5-minute break is automatically triggered.
- **Stop Option**: If you wish to stop the session at any time, you can use the "Stop" checkbox.

## Prerequisites

Before running the application, ensure that you have the following dependencies installed:

- Python 3.x
- Streamlit

### Install the required dependencies

```bash
pip install streamlit
```

## Setup

1. **Clone or create the app**: Copy the script into your local directory.
2. **Run the Streamlit App**:
   - Open a terminal and navigate to your project directory.
   - Run the following command to start the app:

   ```bash
   streamlit run app.py
   ```

3. Open your browser and go to `http://localhost:8501` to use the app.

## How It Works

1. **Select Session Duration**: You can select your desired Pomodoro session duration from the drop-down menu (options range from 1 to 30 minutes).
2. **Start Timer**: After selecting the time, click the "Start" button to begin the Pomodoro session.
3. **Timer Countdown**: The app will show a countdown timer (in minutes and seconds) for the work session. You can stop the timer at any time by checking the "Stop" checkbox.
4. **Break Timer**: Once the work session is complete, a 5-minute break timer starts. After the break, the app signals that the session is over.

## Customization

- You can modify the duration of the break or add more Pomodoro sessions to the app as needed.
- You can also adjust the app's UI by editing the `styles.css` file to customize fonts, colors, and other design elements.

## License

This project is licensed under the **MIT License**.
