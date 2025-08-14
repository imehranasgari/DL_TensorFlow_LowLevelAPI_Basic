# TensorFlow Low-Level API – Core Operations & Workflows

## 1. Project Title

**Hands-on Exploration of TensorFlow’s Low-Level API**

---

## 2. Problem Statement and Goal of Project

This project demonstrates **direct usage of TensorFlow’s low-level operations** to provide maximum control over tensor creation, manipulation, and mathematical computation — bypassing high-level abstractions when needed.
The goal is to understand TensorFlow’s computation model from the ground up and to build a foundation for advanced, custom deep learning workflows.

---

## 3. Solution Approach

The notebook follows a structured, example-driven workflow:

1. **Environment setup & imports** – Initialize TensorFlow and supporting libraries.
2. **Tensor creation** – Use `tf.constant`, `tf.Variable`, and various initializers (`zeros`, `ones`, `fill`, `range`, `random`).
3. **Inspecting tensors** – Retrieve shape, rank, and dtype information.
4. **Type casting** – Change tensor data types with `tf.cast`.
5. **Mathematical operations** – Element-wise math, reductions (`reduce_sum`, `reduce_mean`), matrix multiplication (`matmul`).
6. **Shape manipulation** – Reshaping, expanding/squeezing dimensions, transposition.
7. **Tensor composition** – Concatenation, stacking, splitting, tiling, broadcasting.
8. **Indexing & slicing** – Python slicing and TensorFlow ops (`tf.gather`, `tf.slice`).
9. **Random tensors** – Generate tensors with controlled distributions.
10. **Practical demonstrations** – Show integration of these low-level ops into workflows.

---

## 4. Technologies & Libraries

From the code:

* **TensorFlow** – Low-level ops, tensor manipulation, math functions.
* **NumPy** – Array creation and interoperability with tensors.

---

## 5. Description about Dataset

**Not provided** – The notebook uses only synthetic/random tensors generated in memory.

---

## 6. Installation & Execution Guide

**Requirements:**

```bash
pip install tensorflow numpy
```

**Run the notebook:**

```bash
jupyter notebook low_level_api.ipynb
```

or in JupyterLab:

```bash
jupyter lab low_level_api.ipynb
```

Execute cells sequentially to follow the learning progression.

---

## 7. Key Results / Performance

* Illustrated **complete control** over tensor creation and manipulation using TensorFlow’s low-level API.
* Demonstrated **immutable vs mutable tensors** (`tf.constant` vs `tf.Variable`).
* Showed **graph-friendly slicing/indexing** with TensorFlow ops instead of Python-only indexing.
* Provided examples of **broadcasting** and shape alignment.
* Generated **random tensors** for reproducibility and experimentation.

Sample output snippets:

```
<tf.Tensor: shape=(2, 3), dtype=int32, numpy=
array([[1, 2, 3],
       [4, 5, 6]], dtype=int32)>
```

```
Tensor shape: (3, 2)
Tensor dtype: float32
Tensor rank: 2
```

---

## 8. Screenshots / Sample Out

**Creating a constant tensor:**

```
<tf.Tensor: shape=(3,), dtype=int32, numpy=array([1, 2, 3], dtype=int32)>
```

**Reshaping:**

```
Original shape: (6,)
Reshaped to: (2, 3)
```

**Concatenating tensors:**

```
<tf.Tensor: shape=(3, 3), dtype=int32, numpy=
array([[1, 2, 3],
       [4, 5, 6],
       [7, 8, 9]], dtype=int32)>
```

---

## 9. Additional Learnings / Reflections

* Mastering the low-level API gives **maximum flexibility** for building custom ops and experimenting with graph execution.
* **Broadcasting rules** are crucial to simplify math operations without explicit reshaping.
* Understanding **TensorFlow indexing methods** avoids runtime issues in compiled graphs.
* These skills directly support more advanced custom layers, ops, and training loops.

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---

## 👤 Author

**Mehran Asgari**
**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

---
