## AlgebrAI: A Code-Generating Linear Algebra Calculator
AlgebrAI is an AI-powered calculator built to solve linear algebra problems with high precision.

Unlike general-purpose language models that often produce incorrect or inconsistent math outputs, AlgebrAI generates and executes reliable Python code to directly compute the accurate final answer.

It is powered by a fine-tuned Qwen 3 1.7B model enhanced with QLoRA adapters, and trained on a custom dataset of linear algebra problems paired with executable Python solutions.

When a user inputs a natural language math problem (like "Find eigenvalues of this matrix"), AlgebrAI:

- Understands your query,

- Generates valid Python code,

- Executes the code securely,

- Returns the final answer with no manual math required.
   
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
**🚀 Run It Yourself**

**1. Clone the Repo**
<pre> 
   git clone https://github.com/Umme-2003/AlgrbAI.git 
   cd AlgrbAI 
</pre>

**2.Install dependencies**
<pre>
   pip install numpy torch transformers peft accelerate
</pre>
⚠️ GPU recommended for faster model inference

**3. Launch the notebook**
<pre>
   jupyter notebook
</pre>

Open linear_algebra.ipynb and run the cells step-by-step.
You can enter your own linear algebra problem and watch the model solve it with generated Python code.

**✨ Sample Usage**
Input Prompt: 
<pre>
   Let A = [[1, 2], [3, 4], [5, 6]]. Perform Singular Value Decomposition (SVD) on matrix A and return its singular values.
</pre>
Model Output:
<pre>
import numpy as np
A = np.array([[1, 2], [3, 4], [5, 6]])
U, S, Vt = np.linalg.svd(A)
print(S)
</pre>
Final Answer:
<pre>
   [9.5255, 1.5143]
</pre>
_____________________________________________________________________________________________________________________________________________________________________________________________________________________
**🧠 Model Info**

Base LLM: Qwen 3 1.7B

Tuning: LoRA adapters on a curated problem-code dataset

Inference Tools: Hugging Face Transformers + PEFT

Execution Env: Jupyter / Lightning AI





