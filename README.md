# Tokentrim_suste
TokenTrim was developed as part of IIT Roorkee's prestigious Tech Fest in March 2024, addressing a sophisticated challenge: reducing token overhead in user prompts to minimize the computational costs of utilizing large language models (LLMs). The task required designing a Python tool that intelligently mediates between the user and the LLM by optimizing token usage. The solution involved two innovative strategies:

Semantic Compression through Lexicalization: The first step leveraged the power of semantically dense words (lexicalized concepts) to replace verbose sentences. By compressing complex meanings into single words, the tool effectively reduced the token count, enhancing the efficiency of prompts without compromising the conveyed intent.

Instructed GPT-2 for Token Pruning: In the second step, we utilized a finely-tuned GPT-2 model to prune unnecessary words from the prompt according to a configurable ratio. For instance, a 0.5 ratio would prune 50% of the words. Multiple ratios (ranging from 0.3 to 0.8) were tested, and the resulting truncated prompts were passed through a semantic similarity checker. The mean similarity score of these outputs was used to identify the optimal pruning ratio, ensuring minimal token usage while retaining semantic integrity.

This dual approach—combining semantic density with token pruning—allowed TokenTrim to significantly reduce token overhead, making LLM interactions more cost-effective without degrading the quality of responses.

## Refrence
Refer to the *Selective Context* python library which was used as a part of the second step.

### TokenTrim Cognizance IIT Roorkee 2024 winner repository.
