# Predictions-in-Social-Networks
Predicting properties of nodes and edges in a social network creating feature matrices with networkx.

Data Description:

    The Dataset nodes_df.csv contains information about the Department(indicating the department in the company which the person belongs to) and the ManagementSalary (indicating whether that person is receiving a management position salary) of people in a company
    The Dataset edge_list.csv contains information about the email-communication: each edge indicates that at least one email has been sent between two people
    The Dataset Future_Connections.csv contains pair of nodes that currently do not have a connection, and the Future Connection column indicates if an edge between those two nodes will exist in the future, where a value of 1.0 indicates a future connection and value 0.0 indicates no connection. Some connections have no value yet.

Predictions:

    ManagementSalary: Some people in the network have missing information about the Management Salary - I will predict whether or not these individuals are receiving a management position salary. For this purpose I will create a matrix of node features using networkx, train a LR classifier on nodes that have ManagementSalary data, and predict the probability of receiving a management salary for nodes where this is missing.

    Future connections: I will create a matrix of features for the edges using networkx and train a LR classifier classifier on edges, that have a connection and predict the probability of receiving a connection for those edges with a missing connection.

