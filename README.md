# big-data-final-project
# Dataset instructions
- We have provided combined dataset files that can be utilized across all available notebook
    1. combined_train_data_chunked_10mb_latest.json (Training file)
    2. combined_test_data_chunked_10mb_latest.json (Testing file)
- If you would like to run the file combination logic yourself
    1. Run file file_combiner.ipynb
        


# Running bigrams with cross validations 
- In a non chunked fashion - use sentiment_analysis.ipynb
    # Instructions to run sentiment_analysis.ipynb
        - Modify lines to use the dataset from the path you saved it in 
            - json_df = spark.read.schema(schema).json("combined_train_data_chunked_10mb_latest.json")
            - json_test_df = spark.read.schema(schema).json("combined_test_data_chunked_10mb_latest.json")
- In a chunked fashion - use chunked_sentiment_analysis.ipynb
