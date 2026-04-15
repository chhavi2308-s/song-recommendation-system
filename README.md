# 🎵 Song Recommendation System using Linear Algebra Pipeline

---

## 📌 Project Overview

This project implements a **Song Recommendation System** using a complete **Linear Algebra pipeline**, starting from real-world data and ending with predicted ratings and personalized recommendations.

The system analyzes user listening behavior from the Last.fm dataset and predicts preferences for unseen songs.

---

## 🎯 Objective

* Convert real-world data into matrix form
* Apply core **linear algebra concepts step-by-step**
* Predict missing ratings using mathematical models
* Recommend songs efficiently

---

## 📊 Dataset

* Source: Last.fm HetRec 2011
* Features:

  * `userId` → User identifier
  * `songId` → Song/artist identifier
  * `playCount` → Listening frequency

### Preprocessing:

* Reduced dataset (first 5000 rows) for efficiency
* Normalized playCount to rating scale (1–5)
* Missing values filled with 0

---

# ⚙️ Methodology (Linear Algebra Workflow)

---

## 🔹 Step 1: Matrix Representation

* Users → Rows
* Songs → Columns
* Values → Ratings

👉 Forms the **User–Song Matrix A**

---

## 🔹 Step 2: Matrix Simplification (RREF)

* Applied **Row Reduced Echelon Form (RREF)** on a sample matrix
* Helps identify independent relationships

---

## 🔹 Step 3: Structure of Vector Space

* **Row Space** → User preference space
* **Column Space** → Song feature space
* **Null Space** → Missing preferences

👉 Rank and Nullity computed to analyze structure

---

## 🔹 Step 4: Remove Redundancy (Basis)

* Extracted **basis vectors** from RREF
* Represents independent preference patterns

---

## 🔹 Step 5: Orthogonalization (Gram-Schmidt)

* Converted basis into **orthogonal vectors**
* Ensures independent and uncorrelated features

---

## 🔹 Step 6: Projection

* User vector projected onto orthogonal basis
* Used to estimate unknown preferences

---

## 🔹 Step 7: Least Squares Approximation

[
\hat{x} = (A^T A)^{-1} A^T b
]

* Used to find best approximate solution
* Handles missing/inconsistent data

---

## 🔹 Step 8: System Simplification (SVD)

* Applied **Truncated SVD** for efficiency
* Reduced dimensionality
* Captured hidden relationships

---

## 🔹 Step 9: Prediction (Matrix Reconstruction)

* Reconstructed matrix using SVD
* Predicted missing ratings

---

## 🔹 Step 10: Pattern Discovery (Eigenvalues)

* Computed eigenvalues of covariance matrix
* Identified dominant user behavior patterns

---

## 🔹 Step 11: Final Recommendation

* Recommended top unseen songs for each user
* Based on predicted ratings

---

# 📈 Results

* Successfully modeled user preferences
* Predicted missing ratings
* Generated personalized recommendations

---

# 📸 Output Samples

### ✔ Predicted Ratings Matrix

(Include screenshot here)

### ✔ Final Recommendations

(Include screenshot here)

---

# 📚 Linear Algebra Concepts Used

* Matrix Representation
* Gaussian Elimination (RREF)
* Vector Spaces (Row, Column, Null Space)
* Basis and Linear Independence
* Gram-Schmidt Orthogonalization
* Projection onto Subspaces
* Least Squares Approximation
* Singular Value Decomposition (SVD)
* Eigenvalues and Eigenvectors

---

# ⚠️ Limitations

* Sparse dataset
* Cold-start problem
* No actual song names (only IDs)

---

# 🚀 Applications

* Music recommendation systems
* Streaming platforms (Spotify, Last.fm)
* Personalized content delivery

---

# 👨‍💻 Author

Chhavi S Wadhwa
Chetha Samrutha Vinod
Greeshma N
Harshitha P

