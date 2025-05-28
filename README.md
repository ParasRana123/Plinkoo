# Plinko Gambling Game

A browser-based gambling game inspired by **Stake.com's Plinko**, where users drop a ball into a board filled with obstacles. The ball bounces and falls through randomized paths, ultimately landing in a slot that determines the payout multiplier.

## Gameplay Overview

- Click "Drop Ball" to start.
- The ball travels downward, bouncing off pegs using realistic physics and collision mechanics.
- It lands in one of the final multipliers at the bottom.
- Your `winnings = Bet × Multiplier` from the slot where the ball lands.

## Features

-  Interactive UI with smooth ball animations
-  Collision mechanics for realistic bouncing behavior
-  Customizable multipliers and slot configurations
-  Unlimited plays with each click simulating a new drop
-  Calculates and displays final winnings based on hit multiplier  

## Tech Stack

- **Frontend**: React.js, Node.js, HTML, CSS, JavaScript `(Canvas or DOM-based)`
- **Physics**: Custom collision detection and response for bouncing logic
- **Animations**: JavaScript animation loop `requestAnimationFrame`

## Project Structure

```bash
├── static/            
│   ├── css/        # All CSS stylings in this file
│   ├── uploads/    # Contains user Uploaded images
│   └── matches/    # Matched images for the user uplaoded images
├── templates/
│   └── index.html  # Contains all the frontend HTML code
├── main.py         # Flask backend code
├── app.py          # Streamlit backend code
├── feature_extractor1.ipynb   # Useful for making filenames.pkl
├── feature_extractor.ipynb    # Useful for making embedding.pkl
├── requirements.txt           # Contains all the requirements
└── README.md
```

## Installation

> **Note**: Python Version greater than 3.7 needed.

1. **Clone the Repository**

```bash
git clone [repository-url]
cd face
```

2. **Create and activate python virtual environment**

```bash
conda create -p venv python==3.8.0 -y
activate venv/
```

3. **Install all the requirements necessary for this project**

```bash
pip install -r requirements.txt
```

4. **Install the Jupyter Notebook**

```bash
pip install notebook
```

5. **Run the `feature_extractor1.ipynb` to make `filenames.pkl`**

```bash
jupyter nbconvert --to notebook --feature.extractor1.ipynb --inplace
```

6. **Then run the `feature_extractor.ipynb` to make `embedding.pkl`**

```bash
jupyter nbconvert --to notebook --feature.extractor.ipynb --inplace
```

7. **Make the `uploads` and  `matches` inside `static` folder**

```bash
cd static
mkdir uploads
mkdir matches
```

8. **Start the flask application**

```bash
python main.py
```

   **You can also use the streamlit server (Optional)**
   ```bash
   streamlit run app.py
   ```

## Contributing

We welcome contributions from the community! Whether you're interested in improving features, fixing bugs, or adding new functionality, your input is valuable. Feel free to reach out to us with your ideas and suggestions.

## License
This project is licensed under the MIT License - see the LICENSE file for details.