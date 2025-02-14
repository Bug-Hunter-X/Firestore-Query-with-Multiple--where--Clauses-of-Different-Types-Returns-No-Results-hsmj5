# Firestore Query Issue: Mismatched Data Types in 'where' Clauses

This repository demonstrates a common error when querying Firestore with multiple `where` clauses involving different data types.  The query may unexpectedly return an empty dataset even if matching documents exist due to type mismatches.

**Problem:**  The provided JavaScript code attempts to fetch documents from a Firestore collection that meet specific criteria using a query with `where` clauses comparing both strings and numbers.  A subtle type inconsistency leads to no results being retrieved.

**Solution:** The solution involves carefully examining the data types in Firestore and adjusting the query to ensure type consistency between the query and the data.