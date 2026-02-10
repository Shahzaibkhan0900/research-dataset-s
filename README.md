
Category-wise NFR Consistency and Inconsistency Dataset

Overview

This repository contains a dataset created for category-wise consistency and inconsistency detection of Non-Functional Requirements (NFRs) in software engineering. The dataset was used in research combining MPNet embeddings with a Multi-Layer Perceptron (MLP) model to detect semantic conflicts between NFR statements.

Dataset Description

Original NFR Statements: 1,300 statements across 12 quality attributes: Availability, Functionality, Fault Tolerance, Legal, Look & Feel, Maintainability, Operability, Performance, Portability, Scalability, Security, Usability.

Generated NFR Pairs: 3,493 pairs for consistency detection.

Consistent (1): No conflicts between requirements.

Inconsistent (0): Requirements contradict each other.



Columns

Column	Description

Requirement_1	First NFR statement
Requirement_2	Second NFR statement
Category	Quality attribute of the pair
Consistency_Label	1 = Consistent, 0 = Inconsistent


Examples

Consistent Pair:

R1: Encrypt sensitive user information during transmission.

R2: Use TLS for secure communication.


Inconsistent Pair:

R1: Allow access to all features without authentication.

R2: Require authentication for all features.


Research Context

This dataset was used to train a single model for category-wise NFR classification and consistency detection. MPNet embeddings capture the semantic relationships between requirement statements, and the MLP model predicts consistency. This approach reduces manual effort and supports reliable software requirements analysis.

Usage

Train or evaluate models for NFR classification and consistency detection.

Analyze semantic patterns and conflicts in NFR statements.

Experiment with transformer embeddings or other neural network architectures.


License

This dataset is provided for research and educational purposes. Please cite the associated research paper when using it.
