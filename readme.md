# Hotel Analysis Scripts Overview

This repository contains multiple scripts for analyzing hotel review data with different
focuses and functionalities.

## Scripts Overview

### 1. all_hotels.py

- **Primary Function**: Basic risk scoring system
- **Key Features**:
  - Single hotel analysis
  - Basic performance metrics
  - Risk score calculation
  - Batch processing capability
  - CSV export functionality

### 2. all_hotels1.py

- **Primary Function**: Risk benchmarking system
- **Key Features**:
  - Risk score distribution visualization
  - Benchmark statistics
  - Risk categorization (Low/Moderate/High)
  - Comparative analysis

### 3. analyzer.py

- **Primary Function**: Integration with HotelRiskAnalyzer class
- **Key Features**:
  - Monthly trend analysis
  - Volume and rating trends
  - Target rating tracking
  - 6-month risk score tracking

### 4. analyzer2.py

- **Primary Function**: Detailed single hotel analysis
- **Key Features**:
  - Rolling averages (7d, 30d, 90d)
  - Guest type and origin analysis
  - Room type performance
  - Trend acceleration metrics

### 5. finalv3.py

- **Primary Function**: Advanced visualization dashboard
- **Key Features**:
  - Heatmaps for guest origin/room type
  - Treemap visualizations
  - Stay type analysis
  - Disliked text analysis

## Key Differences

1. **Analysis Depth**

    - `all_hotels.py`: Basic risk scoring
    - `analyzer2.py`: Detailed single hotel metrics
    - `finalv3.py`: Comprehensive visualizations

2. **Visualization Approach**

    - `all_hotels1.py`: Focus on risk distribution
    - `analyzer.py`: Timeline-based analysis
    - `finalv3.py`: Multiple visualization types

3. **Use Case**

    - `all_hotels.py`: Batch processing
    - `analyzer2.py`: Individual hotel deep-dive
    - `finalv3.py`: Executive dashboard
    - `all_hotels1.py`: Comparative analysis
    - `analyzer.py`: Trend monitoring

## Usage

To run any of these scripts:

```bash
streamlit run <script_name>.py
```

Each script requires a CSV file with hotel review data containing specific columns:

- hotel_name
- rating
- review_post_date
- stay_type
- room_view
- user_country (for some scripts)
  