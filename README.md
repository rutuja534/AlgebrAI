**AlgrbAI:  Code-Generating Linear Algebra Solver using Qwen 3 + LoRA**

**AlgrbAI** is a smart, code-generating assistant for solving linear algebra problems.  
It uses a fine-tuned **Qwen 3 1.7B** model trained with **LoRA adapters** on a custom dataset of Linear algrbra problems and Python-based solutions.
When a user inputs a natural language math problem, the model:
1. Understands the query,
2. Generates valid Python code to solve it (e.g., SVD, eigenvalues),
3. Executes the code, and
4. Returns the final result.
   
## 🧠 What Makes This Different

- 🧾 **Trained on real linear algebra problems**  
  The dataset pairs linear algebra problems with working Python code solutions (NumPy/SciPy).

- 🤖 **LLM-generated code execution**  
  The model doesn’t just explain — it writes working Python code and runs it.

  ## 📂 Project Files
<pre> ├── linear_algebra.ipynb # Main notebook (run your queries here) 
      ├── final_dataset_no_comments.json # Training/inference dataset
      └── README.md # Project documentation </pre>
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
🚀 Run It Yourself
<pre>```bash git clone https://github.com/Umme-2003/AlgrbAI.git cd AlgrbAI```</pre>

