# LLM-finetuning-benchmarking
Phi3 and Llama3 finetuning &amp; performance benchmarking
1. Introduction
Both the Phi-3 and LLaMA models have been fine-tuned for multi-class tasks. This documentation focuses on their performance metrics, efficiency, and overall suitability for the task.
2. Data Overview
●FinancialPhraseBank Dataset:

○Introduction: Within the realm of finance and economic texts, annotated datasets are notably rare, with many being exclusively reserved for proprietary purposes. To address the issue of insufficient training data, scholars from the Aalto University School of Business introduced in 2014 a set of approximately 5000 sentences.
○Purpose: This collection aimed to establish human-annotated benchmarks, serving as a standard for evaluating alternative modeling techniques.
○Annotators: The involved annotators (16 people with adequate background knowledge on financial markets) were instructed to assess the sentences solely from the perspective of an investor, evaluating whether the news potentially holds a positive, negative, or neutral impact on the stock price.
○Structure: The FinancialPhraseBank dataset captures the sentiments of financial news headlines from the viewpoint of a retail investor. Comprising two key columns, namely "Sentiment" and "News Headline," the dataset effectively classifies sentiments as either negative, neutral, or positive.
○Significance: This structured dataset serves as a valuable resource for analyzing and understanding the complex dynamics of sentiment in the domain of financial news.

3. Architecture
●Meta-Llama/Meta-Llama-3-8B:

○Size: 8 billion parameters, making it a larger model with potentially greater capabilities.
○Open source: Based on the Llama architecture and available for research and commercial use.
○Performance: Demonstrates strong performance across various tasks like text generation and question-answering.
○Versatility: Suitable for a wide range of applications, thanks to its size and open nature.
○Context window: ~8K tokens 
○Data trained on: A new mix of publicly available online data.

●Microsoft/Phi-3-mini-4k-instruct:

○Size: 3.8B parameters, making it a very small model.
○Efficiency: Designed for efficiency and can run on low-resource devices like smartphones.
○Instruction-tuned: Fine-tuned to follow instructions, making it particularly good at tasks like code generation and summarization.
○Performance: Despite its small size, it performs surprisingly well in certain tasks, especially when compared to other models of similar size.
○Context window: 4096 tokens (approximately 3200 words)
Data trained on: Not publicly disclosed, but likely a mix of web text and code.

10. Conclusion
Both models have their strengths and are suitable for different use cases. Phi-3 is efficient and performs well with less data, making it ideal for quick deployment scenarios. LLaMA, on the other hand, offers potentially higher performance but at the cost of increased resource usage, making it suitable for more detailed and large-scale sentiment analysis tasks.
