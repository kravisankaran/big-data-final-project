# big-data-final-project
# Dataset instructions
- We have provided combined dataset files that can be utilized across all available notebooks
    1. combined_train_data_chunked_10mb_latest.json (Training file)
    2. combined_test_data_chunked_10mb_latest.json (Testing file)
- If you would like to run the file combination logic yourself
-      Instructions to run file_combiner.ipynb
        1. Modify lines to use the datasets from the place you saved it in




# Running bigrams with cross validations 
- In a non chunked fashion - use sentiment_analysis.ipynb
    # Instructions to run sentiment_analysis.ipynb
    1. Modify lines to use the dataset from the place you saved it in 
            - json_df = spark.read.schema(schema).json("combined_train_data_chunked_10mb_latest.json")
            - json_test_df = spark.read.schema(schema).json("combined_test_data_chunked_10mb_latest.json")
- In a chunked fashion - use chunked_sentiment_analysis.ipynb
    # Instructions to run chunked_sentiment_analysis.ipynb
    1.  Modify lines to use the dataset from the place you saved it in 
            - json_training_file_path = "combined_train_data_chunked_10mb_latest.json"
            - df = spark.read.schema(schema).json("combined_test_data_chunked_10mb_latest.json")


# Running bigrams
# Instructions to run bigram_sentiment_analysis.ipynb
  1.  Modify lines to use the dataset from the place you saved it in 
            - json_training_file_path ="../combined_train_data_chunked_10mb_latest.json"
            - df = spark.read.schema(schema).json("../combined_test_data_chunked_10mb_latest.json")


# Running bag of words
# Instructions to run BoW_chunking.ipynb
 1. Modify lines to use the dataset from the place you saved it in
    - json_training_file_path = r"C:\Users\Emma\Downloads\school\Big_Data\project\finaldata\combined_train.json"
    - df_test = spark.read.schema(schema).json(r"C:\Users\Emma\Downloads\school\Big_Data\project\finaldata\combined_test.json")


