# Lab 2: Extending Your Neural Network with Experiments
## Deadline: February 11th at 2:30pm 

## Summary

This two-week assignment builds on your previous neural network work. You will conduct experiments to deepen your understanding of neural network training, activation functions, and evaluation. Refer to Chapters 2, 3, and 4 in the d2l.ai textbook:
- [Chapter 2: Preliminaries](https://d2l.ai/chapter_preliminaries/index.html)
- [Chapter 3: Linear Regression](https://d2l.ai/chapter_linear-regression/index.html)
- [Chapter 4: Linear Classification](https://d2l.ai/chapter_linear-classification/index.html)

By completing this assignment, you will gain hands-on experience in:
- Experimenting with different activation functions and hyperparameter tuning to improve model performance.
- Understanding the impact of dataset size and loss functions on neural network training and evaluation.
- Using GitHub Copilot to generate, refine, and optimize code for neural network implementation.
- Applying and connecting foundational concepts from Chapters 2, 3, and 4 of *Dive into Deep Learning* to practical experiments.

## Foundation from Lab 1

Your neural network from Lab 1 should already include:
- An input layer with at least three neurons (features).
- At least one hidden layer containing at least two neurons.
- A single output neuron that produces a prediction.
- A forward pass that computes a weighted sum and applies a chosen activation function.
- Backpropagation that updates weights and biases, using Mean Squared Error (MSE) loss.
- Basic evaluation metrics (e.g., accuracy).

If any of these elements are missing, address them before starting Lab 2 experiments.

## What is GitHub Copilot?

GitHub Copilot is an AI-powered code completion tool that helps developers write code more efficiently by suggesting lines or blocks of code based on context. It uses machine learning models trained on public code repositories and can assist with tasks such as function creation, error fixing, and refactoring. For this lab, you will use Copilot to:
1. Complete your implementations for activation/loss functions, dataset preprocessing, and evaluation metrics.
2. Refactor and optimize existing code to improve readability and performance.
3. Experiment with different prompts to explore how Copilot's suggestions can impact your workflow.

For guidance on crafting effective prompts for Copilot, refer to the [GitHub Copilot documentation](https://docs.github.com/en/copilot/).

## Tasks

### Step 0: Giving and Incorporating Peer Feedback

During lab on January 28th, present your neural network from lab 1. Your peers will provide feedback on your application, network setup, dataset, and initial results. To ensure the feedback is actionable:
- Present your chosen application, i.e. problem that you chose to predict.
- Discuss the structure of your neural network. 
- Share a summary of your approach in implementation.
- Encourage peers to comment on clarity and potential improvements.
- Document the feedback you receive in your report, identifying at least two specific suggestions to incorporate into extended network.

### Step 1: Extend Your Neural Network

- **Explore Activation Functions**: Test at least three activation functions, such as sigmoid, ReLU, or tanh. Evaluate their impact on model performance and relate the findings to the discussion of activation functions in Chapter 4.
- **Tune Hyperparameters**: Experiment with at least three hyperparameters, such as learning rate, number of hidden neurons, or number of training epochs. Connect your observations to the optimization techniques discussed in Chapter 3.
- **Replace Loss Function**: Try one additional loss function besides MSE, for example cross-entropy loss or another relevant loss function. Consider how loss functions are introduced and utilized in Chapters 3 and 4.

### Step 1a: Expand Your Dataset

Increase your dataset size beyond what was used in Lab 1. Aim for at least 50 data points to reveal meaningful trends in your experiments. Ensure the dataset remains balanced and representative of the problem domain. This aligns with the data preprocessing concepts from Chapter 2.

### Step 2: Use GitHub Copilot

- **Experiment with Prompts**: Use Copilot to:
  - Refactor your original neural network.
  - Complete code for new activation functions or loss functions.
  - Help with your experimental design.
  - Debug issues in your implementation.
- **Document Prompting Experiments**:  Try different prompts and note how Copilot's suggestions vary. Summarize these experiments in your report, reflecting on their effectiveness and limitations. Use the following format for documenting Copilot usage:
- Prompt Type: Debugging/Explaining/Code Completion
- Prompt Description: Detailed description of the prompt used.
- Copilot Suggestion: The suggestion provided by Copilot.
- Effectiveness: How effective the suggestion was and any modifications made.

### Step 3: Mid-Assignment Presentation

During lab on February 4th, present your initial experiment setups, dataset, and preliminary results to the class. Your peers and the instructor will provide live and actionable feedback.
- Showcase your experimental design, expanded dataset, and any preliminary results.
- Discuss how you have used Copilot so far, including what it did well and where manual intervention was required.
- Collect feedback and document it for incorporation into your final work.

### Step 4: Finalize Experiments

- Incorporate feedback from the mid-assignment presentation.
- Complete the reimaning experiments to gather all of your results. Note connections to optimization and classification concepts in Chapters 3 and 4.
- Use Copilot to assist in implementing any changes or optimizations.

### Step 5: Report

Document all experiments in `writing/report.md`. Include:
- Experiment setups, including dataset description, model architecture, and hyperparameter settings.
- Results with performance metrics (e.g., accuracy, loss) and visualizations (e.g., loss curves, scatter plots).
- Insights from the initial and mid-assignment presentation and how feedback was incorporated.
- Details on how Copilot was used, including successful completions and limitations.

### Step 6: (Optional) Additional Experiments

If you find interesting patterns or identify new questions during your experiments, conduct additional explorations and include them in your report.

### Intermediate Checkpoints

- Push code to GitHub after each major experiment or network change.

## Deliverables

1. Updated Python script (`src/neuralnetwork.py`) with extended network and experimental set up. Experiments must be automated. You can extend your implementation to more than one Python file and add additional files as needed. You are not allowed to use any external libraries besides `numpy` and `matplotlib` without permission of the instructor.
2. Updated report (`writing/report.md`) detailing:
   - Experimental designs.
   - Results and performance metrics.
   - Insights from the mid-assignment presentation.
   - Usage of Copilot and prompting experiments.
3. Dataset file (`src/data/data.csv`).
4. GitHub repository with commits demonstrating progress and changes throughout the two weeks.

## Evaluation Criteria

This assignment uses contract-based grading. To receive `A` for the lab, you must:

- Extend your neural network (Step 1) with updated source code in `src/neuralnetwork.py` and updated data in `src/data/data.csv`.
- Present your Lab 1 network to peers on January 28th and your initial experimental design on February 4th.
- Conduct meaningful experiments (including Copilot prompting) with documented outcomes and report your experimental results in `writing/report.md`.
- Submit intermediate commits on GitHub.

For each component that is largely incomplete or incorrect, the assignment will receive a letter grade reduction.

GatorGrader is used to assess portions of the criteria above. The following will be checked by the GatorGrader tool:

1. **Source File Checks**:
    - Ensure that `neuralnetwork.py` file exists in the `src/` directory.
2. **Technical Writing Checks**:
    - Ensure that `report.md` file exists in the `writing/` directory.
    - Write a minimum number of meaningful words (300) in the report.
    - Complete all TODOs and remove the TODO markers in the `report.md`.
    - Ensure the report contains at least three visualizations of experimental graphs.
3. **Dataset File Check**:
    - Ensure that `data.csv` file exists in the `src/data/` directory.
4. **GitHub Repository Checks**:
    - Have at least a specific minimum number of commits (12) in the repository.


