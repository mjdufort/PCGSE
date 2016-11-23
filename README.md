# PCGSE (with hacks by M.J. Dufort)
This is a forked copy of the PCGSE package, with some tweaks to enable the permutation method using pcgseViaSafe(). The local.
and global. functions that safe() uses to calculate gene and gene set statistics are exported so that safe() can find them, and
the code of global.StandAveDiff() is modified to use SparseM::as.matrix() instead of defaulting to base::as.matrix(), which
fails when passed a matrix.csr.
