# Improving SEO of AI-Generated Articles

A comprehensive machine learning project that analyzes and predicts SEO ranking performance for AI-generated content using web scraping, text analysis, and advanced ML techniques.

## 📋 Project Overview

This project focuses on understanding and improving the SEO performance of AI-generated articles by analyzing various ranking factors and building predictive models. The system combines web scraping, natural language processing, and machine learning to provide insights into what makes content rank well in search engines.

## 🚀 Features

### Data Collection & Analysis
- **Web Scraping**: Automated collection of search results and page content
- **SEO Metrics Extraction**: Comprehensive analysis of 30+ SEO factors including:
  - Keyword density and placement
  - Meta tags and descriptions
  - Heading structure (H1, H2, H3)
  - Image alt text optimization
  - Page load speed and technical factors
  - Content structure and readability

### Machine Learning Pipeline
- **Multiple ML Models**: Random Forest, SVM, Logistic Regression, Decision Tree
- **Deep Learning**: DNN, CNN, LSTM, and Autoencoder implementations
- **Feature Engineering**: PCA dimensionality reduction and feature scaling
- **Class Imbalance Handling**: SMOTE oversampling for balanced training
- **Hyperparameter Optimization**: GridSearchCV for model tuning

### Text Analysis
- **Content Analysis**: Word frequency analysis and text statistics
- **Competitor Research**: Automated analysis of competitor articles
- **Visualization**: Word clouds, frequency charts, and comparative analysis

## 📁 Project Structure

```
├── Dataset building and Modeling/
│   ├── Dataset_Model.ipynb              # Main ML pipeline notebook
│   ├── keywords_200.csv                 # Keywords dataset
│   ├── page_raw_metrics_all_article_220.csv  # SEO metrics dataset
│   └── search_results_200.csv           # Search results data
├── Text Analysis/
│   ├── Webscraping_and_text_anlysis.ipynb  # Text analysis notebook
│   ├── Articles.csv                     # Articles dataset
│   └── Output.csv                       # Analysis results
├── Project Summary Presentation.pdf     # Comprehensive project overview
└── README.md                           # This file
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required Python packages (see requirements below)

### Required Libraries
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
pip install requests beautifulsoup4 nltk imbalanced-learn
pip install tensorflow keras wordcloud
```

### API Setup
1. Get Google Custom Search API key from [Google Cloud Console](https://console.cloud.google.com/)
2. Create a Custom Search Engine ID
3. Update the API credentials in `Dataset_Model.ipynb`:
   ```python
   API_KEY = 'your_api_key_here'
   CX_ID = 'your_search_engine_id_here'
   ```

## 📊 Usage

### 1. Data Collection
Run the data collection pipeline in `Dataset_Model.ipynb`:
- Execute keyword search collection
- Scrape page content and extract SEO metrics
- Build comprehensive dataset

### 2. Model Training
- Preprocess data with feature engineering
- Train multiple ML models
- Evaluate performance with cross-validation
- Select best performing model

### 3. Text Analysis
Use `Webscraping_and_text_anlysis.ipynb` for:
- Competitor content analysis
- Word frequency analysis
- Content optimization insights

## 📈 Results

### Model Performance
- **Best Model**: Random Forest Classifier
- **Accuracy**: ~41.6%
- **Precision**: ~45.2%
- **Recall**: ~41.6%

### Key Insights
- Keyword placement in titles and URLs significantly impacts rankings
- Image alt text optimization is crucial for SEO
- Content length and structure affect search performance
- Technical factors (HTTPS, mobile optimization) play important roles

## 🔧 Technical Details

### SEO Metrics Analyzed
- **Content Metrics**: Word count, keyword density, readability
- **Technical SEO**: Page speed, mobile optimization, HTTPS
- **On-Page SEO**: Title tags, meta descriptions, heading structure
- **Image SEO**: Alt text presence and keyword optimization
- **Link Structure**: Internal linking and URL optimization

### Machine Learning Approach
- **Feature Engineering**: 30+ engineered features from raw data
- **Dimensionality Reduction**: PCA with 20 principal components
- **Class Balancing**: SMOTE for handling imbalanced datasets
- **Model Selection**: Comprehensive comparison of multiple algorithms

## 📚 Methodology

1. **Data Collection**: Systematic gathering of search results and page metrics
2. **Feature Engineering**: Creation of meaningful SEO indicators
3. **Model Development**: Training and validation of predictive models
4. **Performance Evaluation**: Comprehensive assessment using multiple metrics
5. **Insight Generation**: Analysis of factors affecting SEO performance

## 🎯 Applications

- **Content Optimization**: Improve AI-generated article SEO performance
- **Competitor Analysis**: Understand ranking factors in your niche
- **SEO Strategy**: Data-driven approach to content marketing
- **Research**: Academic study of SEO ranking factors

## 📄 Documentation

For detailed project information, see:
- `Project Summary Presentation.pdf` - Comprehensive project overview
- Individual Jupyter notebooks contain detailed code documentation
- Inline comments explain methodology and implementation

## 🤝 Contributing

This project is part of academic research. For questions or collaboration:
- Review the project structure and methodology
- Examine the Jupyter notebooks for implementation details
- Refer to the presentation for comprehensive insights

## 📝 License

This project is for educational and research purposes. Please ensure compliance with web scraping policies and API terms of service when using this code.

## 🔗 Related Resources

- [Google Custom Search API Documentation](https://developers.google.com/custom-search/v1/introduction)
- [SEO Best Practices Guide](https://developers.google.com/search/docs)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)

---

**Note**: This project demonstrates the application of machine learning techniques to SEO analysis. Results may vary based on search engine algorithms and market conditions.
