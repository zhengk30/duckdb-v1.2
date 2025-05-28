# duckdb-v1.2
A copy of DuckDB v1.2.2 used for testing. For its original repo, refer to [here](https://github.com/duckdb/duckdb/tree/main).

### Modifications
There are some modifications made to the original DuckDB v1.2.2 to cater to certain needs for the purpose of experimentation. Specifically, the changes are listed as follows:
* In `src/function/scalar/string/like.cpp`, the unescaped version of `LikeOperatorFunction` is reimplemented using Google's RE2.
* In `src/function/scalar/string/contains.cpp`, `idx_t FindStrInStr(const unsigned char* , idx_t, const unsigned char*, idx_t)` is reimplemented using Google's RE2.
* TODO
