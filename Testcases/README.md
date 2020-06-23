# Testcases

There are 7 different test cases present, going from as small as 100 queries to as large as 100k. In final evaluation, we'll go for a million queries (at least), but since that would just increase the repo size unnecessarily, we have skipped that in sample testcases. It's your job to make sure your code work for (very) large testcases too.

- For each test case, there's a query file, data file and expected answer file.
	+ The data file (`sortedData...`) contains STR sorted points. 
	+ Query file structure is explained appropriately in problem statement itself.
	+ The expected answer file is the output is an example of output we expect for the given testcase.

- Bulkload
	+ Always the first (and only first) line of query file.
	+ Starts with `BULKLOAD`.
	+ The second string is the path of data file you need to bulk load from, and you *may* need to change that according to your directory structure.  

- INSERT/QUERY
	+ Process all queries (insert/search) one after the other.
	+ For `QUERY`, you of course need to answer as per the *current* state of the tree.

- Testcase 6 and 7 are for partial credit -- in case you only want to do BULKLOAD (TC 6) or INSERT (TC 7).
