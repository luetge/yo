# HTREE

## SUMMARY

htree is a message digest tool (like md5sum, sha256sum) but fully multi-threaded.

This make significantly faster the creation of checksum for large files.

## USAGE

	htree [file1] [file...] [filen]


## ALGORITHM

htree uses by default a decomposition in 16MiB block size and a (Merkle tree)[https://en.wikipedia.org/wiki/Merkle_tree] associated with the (blake2b)[https://en.wikipedia.org/wiki/BLAKE_(hash_function)] hash function.

The implementation of htree is simple and fits in a single < 300 lines file.


## DEPENDENCIES

None. C++11 compatible compiler

Embedded component : (hadoken)[https://github.com/adevress/hadoken], (digestpp)[https://github.com/kerukuro/digestpp]


## LICENSE

GPLv3
