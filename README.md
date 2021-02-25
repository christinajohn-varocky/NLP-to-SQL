# NLP-to-SQL
## Introduction
A significant amount of the world's knowledge is stored in relational databases. However, the ability for users to retrieve facts from a database is limited due to a lack of understanding of query languages such as SQL.
Text-to-SQL is a task to translate a user’s query spoken in natural language into SQL automatically. Text-to-SQL technique allows users to query databases by using natural language questions.

## Model- EDITSQL
EditSQL takes into account the relation between the user utterance and the table structures as well as recent history of encoding to correctly identify the context. It can edit the generated tokens of the query and take care of this problem using another Bi-LSTM

## methodology
Cross-domain context-dependent text-to-SQL generation task. Here encoder is based on BERT which avails in capturing complex database structures and relate them to the utterances. Thus, given an arbitrary question, the model will most certainly identify correctly the database schema to which the question corresponds.Decoder uses enhanced LSTM to perform SQL generation.
BERT makes use of Transformer, an attention mechanism that learns contextual relations between words (or sub-words) in a text. Transformer includes two separate mechanisms — an encoder that reads the text input and a decoder that produces a prediction for the task.
Table aware decoder: approach addresses this problem by considering the structure of table and the syntax of SQL language. The quality of the generated SQL query is significantly improved through (1) learning to replicate content from column names, cells or SQL keywords; and (2) improving the generation of WHERE clause by leveraging the column-cell relation.

