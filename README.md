# AI Bench Archive
 
 
 A repository that aggregates commonly used benchmarks to test LLM and multimodal models on different modalities and functionalites.

## Leaderboards

### General capability leaderboards
- [Chatbot Arena Leaderboard](https://lmarena.ai/?leaderboard) - an open source platform for evaluating AI through human preference, developed by researchers at UC Berkeley 
- [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) - hosted by HuggingFace, a leaderboard testing open source models on various benchmarks.'
- [ProLLM Leaderboard](https://prollm.toqan.ai/leaderboard) - holds leaderboard evaluating coding assistance, summarization, judging capabilites, entity extraction and many more
- [Judge Arena](https://huggingface.co/spaces/AtlaAI/judge-arena) - community voted leaderboard regarding LLM as a judge capabilites made by Atla

### Coding leaderboards
- [Aider LLM Leaderboards](https://aider.chat/docs/leaderboards/) - hosted by Aider, a pair programming solution. Has leaderboards for Code Editing and Code Refactoring using LLMs
- [Can AI Code Leaderboard](https://huggingface.co/spaces/mike-ravkine/can-ai-code-results) - hosted on HuggingFace, leaderboard summarizing results of the [CanAICode](https://github.com/the-crypt-keeper/can-ai-code) test suite
- [BigCodeBench leaderboard](https://huggingface.co/spaces/bigcode/bigcodebench-leaderboard) - hosted on HuggingFace, leaderboard summarizing the results of the [BigCodeBench](https://huggingface.co/datasets/bigcode/bigcodebench) benchmark.

## General capabilities

### Overall capability text-based benchmarks

- [GPQA](https://paperswithcode.com/dataset/gpqa) - Graduate Level, Google-Proof Q&A Benchmark. Designed to be more challenging than MMLU. Consists of 448 multiple-choice questions in biology, physics and chemistry. Human PhD experts achieve 65% accuracy. Non-experts with unrestricted access to the internet reach only 34%. 
- [MMLU](https://paperswithcode.com/dataset/mmlu) - Massive Multitask Language Understanding, testing undergraduate level knowledge. [Published in 2021](https://arxiv.org/pdf/2009.03300), one of most commonly used benchmarks. GPT-4o level models hover around 88%. While not without [flaws](https://www.youtube.com/watch?v=hVade_8H8mE), it's results are commonly referenced when talking about the performance of AI models. 
- [BIG-Bench-Hard](https://github.com/suzgunmirac/BIG-Bench-Hard) - a benchmark of mixed evaluations, which is an extension of [BIG-Bench](https://arxiv.org/abs/2206.04615). Out of original 204 tasks, 23 most challenging tasks were chosen for this benchmark. Many of those require multi-step reasoning.
- [DROP](https://paperswithcode.com/dataset/drop) - Discrete Reasoning Over Text, a crowdsourced 96k-question benchmark. Requires the system to perform discrete operations, like addition, counting and sorting. The questions consist of passages extracted from Wikipedia articles.
- [HellaSWAG](https://paperswithcode.com/dataset/hellaswag) - otherwise called "Harder Endings, Longer contexts, and Low-shot Activities for Situations With Adversarial Generations". Made in 2019. It is a common knowledge benchmark that is designed to be challenging for LLMs, but trivial for humans (>95% accuracy).
- [WinoGrande](https://winogrande.allenai.org/) - a large scale dataset of 44k problems, introduced in 2019.
- [ARC, the AI2 Reasoning Challenge](https://paperswithcode.com/dataset/arc) - not to be confused with  ARC-AGI. This is a multiple choice question-answering dataset which contains questions from science exams from grade 3 to 9. Split into two parts, Easy in Challenge, latter part requires reasoning.
- [TruthfulQA](https://paperswithcode.com/dataset/truthfulqa) - a benchmark to measure whether a language model is truthful in answering questions. Has 817 questions that are interdisciplinary, including health, law, finance and politics.
- [MT-Bench](https://paperswithcode.com/dataset/mt-bench) - contains 3.3k expert level human preferences for model responses generated by 6 models in response to 80 MT-bench questions. Was introduced in the [LLM-as-a-judge](https://arxiv.org/pdf/2306.05685) paper in 2023.
- [LiveBench](https://livebench.ai/) - benchmarking initiative created in June 2024. Started with 17 diverse tasks initially, with new harder tasks to be added over time.
- [AIME](https://github.com/codelion/optillm/blob/main/scripts/eval_aime_benchmark.py) - American Invitational Mathematics Examination but in the benchmark form
- [Simple Bench](https://simple-bench.com/) - multiple choice text benchmark for LLMs, high school grade but outperforming SOTA models. Over 200 questions including trick questions, social intelligence and spatio-temporal reasoning.

### Towards AGI 

- [GAIA](https://huggingface.co/gaia-benchmark) - benchmark [published](https://ai.meta.com/research/publications/gaia-a-benchmark-for-general-ai-assistants/) by Meta and Yann LeCun, which measures reasoning, multi-modality handling, web-browsing and tool use. Like Hella-Swag, it is designed to be easy for humans but challenging for General AI Assistants.
- [ARC-AGI](https://github.com/fchollet/ARC-AGI) - created by [François Chollet](https://en.wikipedia.org/wiki/Fran%C3%A7ois_Chollet) (creator of the [Keras](https://keras.io/) library), which was created to benchmark the measure the ability of AI systems to solve novel reasoning problems. This benchmark also comes with a [prize](https://arcprize.org/) of 1 million US dollars when beat.
- [MMMU](https://mmmu-benchmark.github.io/) - "Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark for Expert AGI", a benchmark that covers disciplines such as engineering, art and design, science in general, humanities and social studies, business cases and medicine. It has images with diagrams, tables, plots and charts, photograps, chemical structures and many more. Covers cases where both text and images are mixed.

### Other multimodal benchmarks

- [MathVista (testmini)](https://mathvista.github.io/) - is a benchmark combining challenges from diverse mathematical and visual tasks. It consists of 6.141 examples from 28 existing multimodal datasets involving mathematics.
- [Chart Q&A](https://paperswithcode.com/dataset/chartqa) - contains variety of complex questions related to charts
- [AI2D](https://paperswithcode.com/dataset/ai2d) - contains over 5000 grade school science diagrams with over 150 000 rich annotations with their ground truth syntatic parsers, and more than 15 000 multiple choice questions
- [ANLS and ANLS*](https://arxiv.org/abs/2402.03848) - benchmark evaluating a
wide variety of tasks, including information extraction and classification tasks from documents

### Coding benchmarks

- [HumanEval](https://paperswithcode.com/paper/evaluating-large-language-models-trained-on) - used to measure functional correctness for synthesizing programs from docstrings. It consists of 164 original programming problems, assessing language comprehension, algorithms, and simple mathematics, with some comparable to simple software interview questions. It was made in 2021, being one of the most commonly ran benchmarks in the 2023-2024 period. Currently GPT-4 level or better models score above 90%, necessitating the creation and use of better benchmarks for the frontier models. 
- [MathQA-Python](https://arxiv.org/pdf/2108.07732) - a Python version of the MathQA benchmark, contains 23914 problems that evaluate the ability of the models to synthesize code from more complex text, introduced by Google Research
- [MBPP](https://paperswithcode.com/dataset/mbpp) - Mostly Basic Python Programming is a benchmark consisting of around a thousand crowd sourced Python programming problems, designed to be solvable by entry-level programmers. Each problem consists of a task description, code solution and 3 automated test cases.
- [BigCodeBench](https://huggingface.co/datasets/bigcode/bigcodebench) - a dataset of 1.14k problems and solutions related to coding in Python. [Published](https://arxiv.org/abs/2406.15877) on 7th of October 2024.

### Tool use

- [BFCL](https://huggingface.co/datasets/gorilla-llm/Berkeley-Function-Calling-Leaderboard) - Berkeley Function Calling Leaderboard, which evaluates the ability of different LLM to call functions/tools. Covers basic use cases and agentic workflows. 
- [MetaTool](https://arxiv.org/abs/2310.03128) - a benchmark designed to asses the ability of LLMs to use correct tools given situation. Includes ToolE dataset, which contains prompts triggering single and multi tool use.
- [API-Bank](https://arxiv.org/abs/2304.08244) - is a runnable evaluation system consisting of 73 APIs published in 2023.

### Agent evaluation

- [WorkArena++](https://github.com/ServiceNow/WorkArena) - a suite of browser-based tasks to measure web agent performance - also a part of [BrowserGym](https://github.com/ServiceNow/BrowserGym) which holds many smaller agentic benchmarks.

## Field-based capabilities

### Math benchmarks

- [MATH](https://paperswithcode.com/dataset/math) - a dataset of 12 500 challenging competition mathematics problems. Each problem has a step-by-step solution that can be used to teach models to generate answer derivations and explanations.
- [MGSM](https://paperswithcode.com/dataset/mgsm) - Multilingual Grade School Math Benchmark is a collection of grade-school math problems. Consists of 250 problems from GSM8K translated across 10 languages.
- [GSM8K](https://paperswithcode.com/dataset/gsm8k) - introduced in 2021, a dataset of 8.5k quality 8th grade math problems. Each problem takes between 2 to 8 steps to solve, necessitating use of basic arithmetic operations to reach the final answer. 
- [Putnam Bench](https://arxiv.org/pdf/2407.11214) - multi language benchmark for evaluation of the ability to solve competition mathematic problems. Includes 1692 formalizations of 640 problems from the William Lowell Putnam Mathematical Competition, college level problems.

### Legal benchmarks

- [LegalBench](https://arxiv.org/pdf/2308.11462) - a collaboratively constructed legal reasoning benchmark consisting of 162 tasks covering six different types of legal reasoning. Made by subject experts between many highly esteemed universities, this benchmark measures legal reasoning capabilites that are useful to lawyers and reasoning skills that are interesting to them.

### Biology benchmarks

- [LAB-Bench](https://arxiv.org/abs/2407.10362) - Language Agent Biology Benchmark, evaluates LLM capabilites on literature search, protocol planning and data analysis.

## Resources used

- [Claude 3.5 Sonnet announcement](https://www.anthropic.com/news/claude-3-5-sonnet), attached used benchmarks - GPQA, MMLU, BIG-Bench-Hard, DROP, MATH, MGSM, GSM8K, HumanEval, multimodal ones - MathVista (testmini), AI2D, Chart Q&A, ANLS
- [GPT-4 technical report](https://arxiv.org/pdf/2303.08774) - attached used benchmarks not mentioned above - HellaSwag, ARC, WinoGrade
- [HuggingFace](https://huggingface.co/) - attached leaderboards and benchmarks used there
