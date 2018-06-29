# shardingRadixTrie
Sharding radix tries to reduce read/write locks

## implementation plan
1. implement normal radix trie
2. apply one lock on the hole trie 
   1. benchmark
3. apply the sharding strategy 
   1. first implementation is a hashmap with pointers to the root of each shard
   2. benchmark *performance can be affected by parameters one is **shard number***
 Inline-style: 
 ![sharding a tree](https://github.com/MheniMerz/shardingRadixTrie/shardingTree.png)

