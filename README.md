# Dealership Creative Automation Tool

An automated tool to generate branded dealership creatives for social media.

## Features
- **Smart Scaling**: Automatically resizes and crops background images to fit target dimensions (1:1, 4:5, 9:16) without distortion.
- **Bulk Processing**: Generate multiple creatives for different dealers and sizes in one click.
- **Dynamic Assets**: Automatically pulls correct panels and logos based on the selected brand and dealer.
- **ZIP Export**: Download all generated assets as a single ZIP file.

## Tech Stack
- **Backend**: Python 3, Flask, Pillow
- **Frontend**: Vanilla HTML5, CSS3 (Premium Dark Theme), Javascript
- **Database**: SQLite

## Setup Instructions

### 1. Install Dependencies
Ensure you have Python 3 installed, then run:
```bash
pip install -r requirements.txt
```

### 2. Initialize Database
Run the seeding script to populate brands and dealerships from the assets folder:
```bash
python3 init_db.py
```

### 3. Run the Application
Start the Flask server:
```bash
python3 app.py
```
Open your browser and navigate to `http://localhost:5000`.

## Admin Credentials
**Username:** admin  
**Password:** admin123

## SQL Dump
The database schema and initial data are provided in `database.sqlite`. You can also generate a SQL dump using:
```bash
sqlite3 database.sqlite .dump > database.sql
```
