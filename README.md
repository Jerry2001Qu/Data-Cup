# Data-Cup
This was my development code used when participating in the Data Cup, a $1mil AI challenge to detect fake news in headlines.

I ended 23rd in the Data Cup.

# Methodology Overview
BERT/XLNet Language Models used (SOTA Transformer models from @Huggingface)

# Data Source
As accordance to the rules on Data Cup, I am not able to upload/store the data used in the competition. However, I'll describe what it looked like here.

Feature 1: “claim”: statement
            Example: "claim": "Viral posts claim that climate change is a \"made-up catastrophe.\""
            
Feature 2: “claimant”: entity who made the claim
            Example: "claimant": "Social media posts"
            
Feature 3: “date”: when the claim was made
            Example: "date": "2019-05-08"

Feature 5: “related_articles”: list of source and supporting article ids (that point to files in
            train_articles).
            Example: "related_articles": [20540, 38088, 14596, 20539, 20546, 38393, 20541, 41754]
            
Label 1: “label”: truth labeling of the claim (0:false, 1:partly true, 2:true)
          Example: "label": 0
          
# Analysis
I'll be posting a Medium article in the future to talk about the steps I walked through while creating this code. There is a lot more code in other notebooks (Eg. Testing XLNet, RoBERTa. Data Visualizations. Failed iterations), but this is a sample of a single end-end process. If I could make the data available, you'd be able to run these 3 notebooks to preprocess, train, and visualize the data.
