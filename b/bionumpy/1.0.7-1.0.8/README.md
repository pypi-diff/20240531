# Comparing `tmp/bionumpy-1.0.7.tar.gz` & `tmp/bionumpy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bionumpy-1.0.7.tar", last modified: Wed Mar  6 14:27:53 2024, max compression
+gzip compressed data, was "bionumpy-1.0.8.tar", last modified: Wed Mar  6 17:49:41 2024, max compression
```

## Comparing `bionumpy-1.0.7.tar` & `bionumpy-1.0.8.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.103960 bionumpy-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:27:15.000000 bionumpy-1.0.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-06 14:27:15.000000 bionumpy-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-06 14:27:15.000000 bionumpy-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-06 14:27:53.103960 bionumpy-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-06 14:27:15.000000 bionumpy-1.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.071960 bionumpy-1.0.7/bionumpy/
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.071960 bionumpy-1.0.7/bionumpy/alignments/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/alignments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/alignments/cigar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.071960 bionumpy-1.0.7/bionumpy/arithmetics/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/arithmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/arithmetics/bedgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/arithmetics/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/arithmetics/similarity_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.071960 bionumpy-1.0.7/bionumpy/bnpdataclass/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/bnpdataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/bnpdataclass/bnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/bnpdataclass/bnpdataclassfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/bnpdataclass/lazybnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/bnpdataclass/pandas_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/computation_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.071960 bionumpy-1.0.7/bionumpy/cupy_compatible/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/cupy_compatible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/cupy_compatible/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.075960 bionumpy-1.0.7/bionumpy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/datatypes/gtf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encoded_array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.075960 bionumpy-1.0.7/bionumpy/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/_legacy_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/alphabet_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/base_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/integer_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/kmer_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/string_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/encodings/vcf_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.075960 bionumpy-1.0.7/bionumpy/genomic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/binned_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/coordinate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genome_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genome_context_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genomic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    27334 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genomic_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genomic_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/genomic_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/genomic_data/global_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.083960 bionumpy-1.0.7/bionumpy/io/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/bam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.083960 bionumpy-1.0.7/bionumpy/io/buffers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/buffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/buffers/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/dump_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/fastq_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/file_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/genotype_buffer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/gfa.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/gzip_reading.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/indexed_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/indexed_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/jaspar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/matrix_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/motifs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/multiline_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/named_text_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/npdataclassreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/one_line_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/regexp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/strops.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/vcf_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/vcf_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/io/wig.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.083960 bionumpy-1.0.7/bionumpy/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/count_encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/debruin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/genes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.083960 bionumpy-1.0.7/bionumpy/sequence/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/indexing/kmer_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/indexing/wildcard_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/kmers.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/minimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/position_weight_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/rollable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/string_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/sequence/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.087960 bionumpy-1.0.7/bionumpy/simulate/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/chipseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/rnaseq.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/test_simulate_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/simulate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.087960 bionumpy-1.0.7/bionumpy/streams/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/chunk_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/groupby_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/grouped.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/left_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/multistream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/reductions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/streams/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/string_array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.087960 bionumpy-1.0.7/bionumpy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/tests/test_basic_functionality.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.087960 bionumpy-1.0.7/bionumpy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/ascii_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/formating.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/ragged_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.087960 bionumpy-1.0.7/bionumpy/variants/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/variants/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/variants/consensus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-06 14:27:15.000000 bionumpy-1.0.7/bionumpy/variants/mutation_signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.103960 bionumpy-1.0.7/bionumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 14:27:52.000000 bionumpy-1.0.7/bionumpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 14:27:53.000000 bionumpy-1.0.7/bionumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-06 14:27:53.103960 bionumpy-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-06 14:27:16.000000 bionumpy-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.099960 bionumpy-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.099960 bionumpy-1.0.7/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/api_tests/immune_ml.py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/genomic_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/gfa_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.103960 bionumpy-1.0.7/tests/io_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/io_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/io_tests/sub_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/io_tests/test_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/io_tests/test_sub_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.103960 bionumpy-1.0.7/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/performance/interval_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:53.103960 bionumpy-1.0.7/tests/property_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/oo_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/test_delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/property_tests/test_strops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_asciihash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_bam.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_binned_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_bionumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_bnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_chromosome_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_computation_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_coordinate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_debruijn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_encoded_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_encodedarrayfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_encodedcounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_entry_chunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_file_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_forbes_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_formating.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_genomic_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_genomic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_genomic_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_genomic_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_global_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_groupby.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_gtf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_immuneml_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_indexed_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_io_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_kmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_kmer_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_kmer_nmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_lazybnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_minimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_multistream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_mutation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_npdataclassstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_pandas_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_pileup.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_position_weight_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_ragged_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_real_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_regexp.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_rollable.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_seqeunces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_similarity_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_streambroadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_string_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_string_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_string_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_strops.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_vcf_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_wig.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/test_wildcard_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-06 14:27:16.000000 bionumpy-1.0.7/tests/vcf_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.587030 bionumpy-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:49:04.000000 bionumpy-1.0.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-06 17:49:04.000000 bionumpy-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-06 17:49:04.000000 bionumpy-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-06 17:49:41.587030 bionumpy-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-06 17:49:04.000000 bionumpy-1.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.551030 bionumpy-1.0.8/bionumpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/alignments/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/alignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/alignments/cigar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/arithmetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/arithmetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/arithmetics/bedgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/arithmetics/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/arithmetics/similarity_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/bnpdataclass/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/bnpdataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/bnpdataclass/bnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/bnpdataclass/bnpdataclassfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/bnpdataclass/lazybnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/bnpdataclass/pandas_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/computation_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/cupy_compatible/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/cupy_compatible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/cupy_compatible/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/datatypes/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encoded_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.555030 bionumpy-1.0.8/bionumpy/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/_legacy_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/alphabet_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/base_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/integer_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/kmer_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/string_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/encodings/vcf_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.559030 bionumpy-1.0.8/bionumpy/genomic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/binned_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/coordinate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genome_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genome_context_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genomic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27334 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genomic_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genomic_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/genomic_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/genomic_data/global_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.563030 bionumpy-1.0.8/bionumpy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/bam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.563030 bionumpy-1.0.8/bionumpy/io/buffers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/buffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/buffers/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25232 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/dump_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/fastq_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/file_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/genotype_buffer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/gfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/gzip_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/indexed_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/indexed_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/jaspar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/matrix_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/motifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/multiline_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/named_text_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/npdataclassreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/one_line_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/strops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/vcf_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/vcf_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/io/wig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.567030 bionumpy-1.0.8/bionumpy/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/count_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/debruin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/genes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.567030 bionumpy-1.0.8/bionumpy/sequence/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/indexing/kmer_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/indexing/wildcard_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/kmers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/position_weight_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/rollable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/string_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/sequence/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.567030 bionumpy-1.0.8/bionumpy/simulate/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/chipseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/rnaseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/test_simulate_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/simulate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.567030 bionumpy-1.0.8/bionumpy/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/chunk_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/groupby_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/grouped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/left_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/multistream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/reductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/streams/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/string_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.571030 bionumpy-1.0.8/bionumpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/tests/test_basic_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.571030 bionumpy-1.0.8/bionumpy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/ascii_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/formating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/ragged_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.571030 bionumpy-1.0.8/bionumpy/variants/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/variants/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/variants/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-06 17:49:04.000000 bionumpy-1.0.8/bionumpy/variants/mutation_signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.587030 bionumpy-1.0.8/bionumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 17:49:41.000000 bionumpy-1.0.8/bionumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-06 17:49:41.587030 bionumpy-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-06 17:49:05.000000 bionumpy-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.583030 bionumpy-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.583030 bionumpy-1.0.8/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/api_tests/immune_ml.py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/genomic_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/gfa_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.587030 bionumpy-1.0.8/tests/io_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/io_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/io_tests/sub_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/io_tests/test_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/io_tests/test_sub_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.587030 bionumpy-1.0.8/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/performance/interval_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:41.587030 bionumpy-1.0.8/tests/property_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/oo_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/test_delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/property_tests/test_strops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_asciihash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_bam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_binned_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_bionumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_bnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_chromosome_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_computation_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_coordinate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_debruijn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_encoded_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_encodedarrayfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_encodedcounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_entry_chunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_file_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_forbes_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_formating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_genomic_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_genomic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_genomic_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_genomic_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_global_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_gtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_immuneml_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_indexed_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_io_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_kmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_kmer_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_kmer_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_lazybnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_multistream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_mutation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_npdataclassstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_pandas_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_position_weight_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_ragged_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_rollable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_seqeunces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_similarity_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_streambroadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_string_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_string_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_string_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_strops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_vcf_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_wig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/test_wildcard_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-06 17:49:05.000000 bionumpy-1.0.8/tests/vcf_script.py
```

### Comparing `bionumpy-1.0.7/LICENSE` & `bionumpy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/PKG-INFO` & `bionumpy-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionumpy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for working with biological sequence data as numpy arrays.
 Home-page: https://github.com/bionumpy/bionumpy
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: bionumpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: numpy>=1.20
-Requires-Dist: npstructures>=0.2.9
+Requires-Dist: npstructures>=0.2.15
 Provides-Extra: full
 Requires-Dist: isal; extra == "full"
 
 ========
 BioNumPy
 ========
```

### Comparing `bionumpy-1.0.7/README.rst` & `bionumpy-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/__init__.py` & `bionumpy-1.0.8/bionumpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for bionumpy."""
 
 __author__ = """Knut Rand"""
 __email__ = "knutdrand@gmail.com"
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 import npstructures as nps
 
 from .io import (count_entries, open_indexed, MultiLineFastaBuffer, bnp_open,
                  Bed6Buffer, NarrowPeakBuffer, TwoLineFastaBuffer,
                  BedBuffer, GfaSequenceBuffer, get_bufferclass_for_datatype, FastQBuffer)
 from .encodings.alphabet_encoding import (DNAEncoding, RNAENcoding, AminoAcidEncoding)
```

### Comparing `bionumpy-1.0.7/bionumpy/alignments/__init__.py` & `bionumpy-1.0.8/bionumpy/alignments/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/alignments/cigar.py` & `bionumpy-1.0.8/bionumpy/alignments/cigar.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/arithmetics/bedgraph.py` & `bionumpy-1.0.8/bionumpy/arithmetics/bedgraph.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/arithmetics/intervals.py` & `bionumpy-1.0.8/bionumpy/arithmetics/intervals.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/arithmetics/similarity_measures.py` & `bionumpy-1.0.8/bionumpy/arithmetics/similarity_measures.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/bnpdataclass/bnpdataclass.py` & `bionumpy-1.0.8/bionumpy/bnpdataclass/bnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/bnpdataclass/bnpdataclassfunction.py` & `bionumpy-1.0.8/bionumpy/bnpdataclass/bnpdataclassfunction.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/bnpdataclass/lazybnpdataclass.py` & `bionumpy-1.0.8/bionumpy/bnpdataclass/lazybnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/bnpdataclass/pandas_adaptor.py` & `bionumpy-1.0.8/bionumpy/bnpdataclass/pandas_adaptor.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/computation_graph.py` & `bionumpy-1.0.8/bionumpy/computation_graph.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/datatypes/__init__.py` & `bionumpy-1.0.8/bionumpy/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/datatypes/gtf.py` & `bionumpy-1.0.8/bionumpy/datatypes/gtf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encoded_array.py` & `bionumpy-1.0.8/bionumpy/encoded_array.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/__init__.py` & `bionumpy-1.0.8/bionumpy/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/_legacy_encodings.py` & `bionumpy-1.0.8/bionumpy/encodings/_legacy_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/alphabet_encoding.py` & `bionumpy-1.0.8/bionumpy/encodings/alphabet_encoding.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/kmer_encodings.py` & `bionumpy-1.0.8/bionumpy/encodings/kmer_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/string_encodings.py` & `bionumpy-1.0.8/bionumpy/encodings/string_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/encodings/vcf_encoding.py` & `bionumpy-1.0.8/bionumpy/encodings/vcf_encoding.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/annotation.py` & `bionumpy-1.0.8/bionumpy/genomic_data/annotation.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/binned_genome.py` & `bionumpy-1.0.8/bionumpy/genomic_data/binned_genome.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/coordinate_mapping.py` & `bionumpy-1.0.8/bionumpy/genomic_data/coordinate_mapping.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genome.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genome.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genome_context.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genome_context.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genome_context_base.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genome_context_base.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genomic_data.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genomic_data.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genomic_intervals.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genomic_intervals.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genomic_sequence.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genomic_sequence.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/genomic_track.py` & `bionumpy-1.0.8/bionumpy/genomic_data/genomic_track.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/geometry.py` & `bionumpy-1.0.8/bionumpy/genomic_data/geometry.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/genomic_data/global_offset.py` & `bionumpy-1.0.8/bionumpy/genomic_data/global_offset.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/__init__.py` & `bionumpy-1.0.8/bionumpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/_legacy.py` & `bionumpy-1.0.8/bionumpy/io/_legacy.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/bam.py` & `bionumpy-1.0.8/bionumpy/io/bam.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/buffers/sam.py` & `bionumpy-1.0.8/bionumpy/io/buffers/sam.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/delimited_buffers.py` & `bionumpy-1.0.8/bionumpy/io/delimited_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/dump_csv.py` & `bionumpy-1.0.8/bionumpy/io/dump_csv.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/fastq_buffer.py` & `bionumpy-1.0.8/bionumpy/io/fastq_buffer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/file_buffers.py` & `bionumpy-1.0.8/bionumpy/io/file_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/files.py` & `bionumpy-1.0.8/bionumpy/io/files.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/gfa.py` & `bionumpy-1.0.8/bionumpy/io/gfa.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/headers.py` & `bionumpy-1.0.8/bionumpy/io/headers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/indexed_fasta.py` & `bionumpy-1.0.8/bionumpy/io/indexed_fasta.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/indexed_files.py` & `bionumpy-1.0.8/bionumpy/io/indexed_files.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/jaspar.py` & `bionumpy-1.0.8/bionumpy/io/jaspar.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/matrix_dump.py` & `bionumpy-1.0.8/bionumpy/io/matrix_dump.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/multiline_buffer.py` & `bionumpy-1.0.8/bionumpy/io/multiline_buffer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/named_text_buffer.py` & `bionumpy-1.0.8/bionumpy/io/named_text_buffer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/npdataclassreader.py` & `bionumpy-1.0.8/bionumpy/io/npdataclassreader.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/one_line_buffer.py` & `bionumpy-1.0.8/bionumpy/io/one_line_buffer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/parser.py` & `bionumpy-1.0.8/bionumpy/io/parser.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/regexp.py` & `bionumpy-1.0.8/bionumpy/io/regexp.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/strops.py` & `bionumpy-1.0.8/bionumpy/io/strops.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/vcf_buffers.py` & `bionumpy-1.0.8/bionumpy/io/vcf_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/io/vcf_header.py` & `bionumpy-1.0.8/bionumpy/io/vcf_header.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/plotting.py` & `bionumpy-1.0.8/bionumpy/plotting.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/__init__.py` & `bionumpy-1.0.8/bionumpy/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/bloom_filter.py` & `bionumpy-1.0.8/bionumpy/sequence/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/count_encoded.py` & `bionumpy-1.0.8/bionumpy/sequence/count_encoded.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/debruin.py` & `bionumpy-1.0.8/bionumpy/sequence/debruin.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/dna.py` & `bionumpy-1.0.8/bionumpy/sequence/dna.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/genes.py` & `bionumpy-1.0.8/bionumpy/sequence/genes.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/indexing/kmer_indexing.py` & `bionumpy-1.0.8/bionumpy/sequence/indexing/kmer_indexing.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/indexing/wildcard_index.py` & `bionumpy-1.0.8/bionumpy/sequence/indexing/wildcard_index.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/kmers.py` & `bionumpy-1.0.8/bionumpy/sequence/kmers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/lookup.py` & `bionumpy-1.0.8/bionumpy/sequence/lookup.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/minimizers.py` & `bionumpy-1.0.8/bionumpy/sequence/minimizers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/position_weight_matrix.py` & `bionumpy-1.0.8/bionumpy/sequence/position_weight_matrix.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/rollable.py` & `bionumpy-1.0.8/bionumpy/sequence/rollable.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/string_matcher.py` & `bionumpy-1.0.8/bionumpy/sequence/string_matcher.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/sequence/translate.py` & `bionumpy-1.0.8/bionumpy/sequence/translate.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/simulate/chipseq.py` & `bionumpy-1.0.8/bionumpy/simulate/chipseq.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/simulate/intervals.py` & `bionumpy-1.0.8/bionumpy/simulate/intervals.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/simulate/rnaseq.py` & `bionumpy-1.0.8/bionumpy/simulate/rnaseq.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/simulate/sequences.py` & `bionumpy-1.0.8/bionumpy/simulate/sequences.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/simulate/variants.py` & `bionumpy-1.0.8/bionumpy/simulate/variants.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/chunk_entries.py` & `bionumpy-1.0.8/bionumpy/streams/chunk_entries.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/decorators.py` & `bionumpy-1.0.8/bionumpy/streams/decorators.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/groupby_func.py` & `bionumpy-1.0.8/bionumpy/streams/groupby_func.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/grouped.py` & `bionumpy-1.0.8/bionumpy/streams/grouped.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/left_join.py` & `bionumpy-1.0.8/bionumpy/streams/left_join.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/multistream.py` & `bionumpy-1.0.8/bionumpy/streams/multistream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/reductions.py` & `bionumpy-1.0.8/bionumpy/streams/reductions.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/streams/stream.py` & `bionumpy-1.0.8/bionumpy/streams/stream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/string_array.py` & `bionumpy-1.0.8/bionumpy/string_array.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/tests/conftest.py` & `bionumpy-1.0.8/bionumpy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/tests/test_basic_functionality.py` & `bionumpy-1.0.8/bionumpy/tests/test_basic_functionality.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/util/__init__.py` & `bionumpy-1.0.8/bionumpy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/util/ascii_hash.py` & `bionumpy-1.0.8/bionumpy/util/ascii_hash.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/util/testing.py` & `bionumpy-1.0.8/bionumpy/util/testing.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/variants/_legacy.py` & `bionumpy-1.0.8/bionumpy/variants/_legacy.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/variants/consensus.py` & `bionumpy-1.0.8/bionumpy/variants/consensus.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy/variants/mutation_signature.py` & `bionumpy-1.0.8/bionumpy/variants/mutation_signature.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/bionumpy.egg-info/PKG-INFO` & `bionumpy-1.0.8/bionumpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionumpy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for working with biological sequence data as numpy arrays.
 Home-page: https://github.com/bionumpy/bionumpy
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: bionumpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: numpy>=1.20
-Requires-Dist: npstructures>=0.2.9
+Requires-Dist: npstructures>=0.2.15
 Provides-Extra: full
 Requires-Dist: isal; extra == "full"
 
 ========
 BioNumPy
 ========
```

### Comparing `bionumpy-1.0.7/bionumpy.egg-info/SOURCES.txt` & `bionumpy-1.0.8/bionumpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/setup.py` & `bionumpy-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
     requirements = ['numpy>=1.20',
-                    'npstructures>=0.2.9',]
+                    'npstructures>=0.2.15',]
 # 'npstructures @ git+https://github.com/knutdrand/npstructures.git']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Knut Rand",
     author_email='knutdrand@gmail.com',
@@ -42,14 +42,14 @@
     include_package_data=True,
     keywords='bionumpy',
     name='bionumpy',
     packages=find_packages(include=['bionumpy', 'bionumpy.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bionumpy/bionumpy',
-    version='1.0.7',
+    version='1.0.8',
     zip_safe=False,
     extras_require={'full': ['isal']}
 )
 
 # python -m build
 # twine upload dist/*
```

### Comparing `bionumpy-1.0.7/tests/buffers.py` & `bionumpy-1.0.8/tests/buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/fixtures.py` & `bionumpy-1.0.8/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/genomic_fixtures.py` & `bionumpy-1.0.8/tests/genomic_fixtures.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/io_tests/test_sam.py` & `bionumpy-1.0.8/tests/io_tests/test_sam.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/io_tests/test_sub_delimiters.py` & `bionumpy-1.0.8/tests/io_tests/test_sub_delimiters.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/performance/interval_sort.py` & `bionumpy-1.0.8/tests/performance/interval_sort.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/property_tests/strategies.py` & `bionumpy-1.0.8/tests/property_tests/strategies.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/property_tests/test_delimited_buffers.py` & `bionumpy-1.0.8/tests/property_tests/test_delimited_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/property_tests/test_encodings.py` & `bionumpy-1.0.8/tests/property_tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/property_tests/test_strops.py` & `bionumpy-1.0.8/tests/property_tests/test_strops.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_asciihash.py` & `bionumpy-1.0.8/tests/test_asciihash.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_bam.py` & `bionumpy-1.0.8/tests/test_bam.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_binned_genome.py` & `bionumpy-1.0.8/tests/test_binned_genome.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_bloom_filter.py` & `bionumpy-1.0.8/tests/test_bloom_filter.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_bnpdataclass.py` & `bionumpy-1.0.8/tests/test_bnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_chromosome_provider.py` & `bionumpy-1.0.8/tests/test_chromosome_provider.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_computation_graph.py` & `bionumpy-1.0.8/tests/test_computation_graph.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_coordinate_mapping.py` & `bionumpy-1.0.8/tests/test_coordinate_mapping.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_debruijn.py` & `bionumpy-1.0.8/tests/test_debruijn.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_delimited_buffers.py` & `bionumpy-1.0.8/tests/test_delimited_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_dna.py` & `bionumpy-1.0.8/tests/test_dna.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_encoded_array.py` & `bionumpy-1.0.8/tests/test_encoded_array.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_encodedarrayfunctions.py` & `bionumpy-1.0.8/tests/test_encodedarrayfunctions.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_encodings.py` & `bionumpy-1.0.8/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_entry_chunker.py` & `bionumpy-1.0.8/tests/test_entry_chunker.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_file_buffers.py` & `bionumpy-1.0.8/tests/test_file_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_forbes_acceptance.py` & `bionumpy-1.0.8/tests/test_forbes_acceptance.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_genomic_data.py` & `bionumpy-1.0.8/tests/test_genomic_data.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_genomic_sequence.py` & `bionumpy-1.0.8/tests/test_genomic_sequence.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_genomic_track.py` & `bionumpy-1.0.8/tests/test_genomic_track.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_geometry.py` & `bionumpy-1.0.8/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_global_offset.py` & `bionumpy-1.0.8/tests/test_global_offset.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_groupby.py` & `bionumpy-1.0.8/tests/test_groupby.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_gtf.py` & `bionumpy-1.0.8/tests/test_gtf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_immuneml_compat.py` & `bionumpy-1.0.8/tests/test_immuneml_compat.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_indexed_fasta.py` & `bionumpy-1.0.8/tests/test_indexed_fasta.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_integration.py` & `bionumpy-1.0.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_intervals.py` & `bionumpy-1.0.8/tests/test_intervals.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_io.py` & `bionumpy-1.0.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_io_exceptions.py` & `bionumpy-1.0.8/tests/test_io_exceptions.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_kmer.py` & `bionumpy-1.0.8/tests/test_kmer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_kmer_index.py` & `bionumpy-1.0.8/tests/test_kmer_index.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_kmer_nmf.py` & `bionumpy-1.0.8/tests/test_kmer_nmf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_lazybnpdataclass.py` & `bionumpy-1.0.8/tests/test_lazybnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_minimizers.py` & `bionumpy-1.0.8/tests/test_minimizers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_multistream.py` & `bionumpy-1.0.8/tests/test_multistream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_mutation_types.py` & `bionumpy-1.0.8/tests/test_mutation_types.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_npdataclassstream.py` & `bionumpy-1.0.8/tests/test_npdataclassstream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_parsers.py` & `bionumpy-1.0.8/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_pileup.py` & `bionumpy-1.0.8/tests/test_pileup.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_plotting.py` & `bionumpy-1.0.8/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_position_weight_matrix.py` & `bionumpy-1.0.8/tests/test_position_weight_matrix.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_real_data.py` & `bionumpy-1.0.8/tests/test_real_data.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_regexp.py` & `bionumpy-1.0.8/tests/test_regexp.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_rollable.py` & `bionumpy-1.0.8/tests/test_rollable.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_seqeunces.py` & `bionumpy-1.0.8/tests/test_seqeunces.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_similarity_measures.py` & `bionumpy-1.0.8/tests/test_similarity_measures.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_simulate.py` & `bionumpy-1.0.8/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_streambroadcast.py` & `bionumpy-1.0.8/tests/test_streambroadcast.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_streams.py` & `bionumpy-1.0.8/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_string_array.py` & `bionumpy-1.0.8/tests/test_string_array.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_string_encodings.py` & `bionumpy-1.0.8/tests/test_string_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_string_matcher.py` & `bionumpy-1.0.8/tests/test_string_matcher.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_strops.py` & `bionumpy-1.0.8/tests/test_strops.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_util.py` & `bionumpy-1.0.8/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_vcf.py` & `bionumpy-1.0.8/tests/test_vcf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_vcf_encoding.py` & `bionumpy-1.0.8/tests/test_vcf_encoding.py`

 * *Files identical despite different names*

### Comparing `bionumpy-1.0.7/tests/test_wildcard_index.py` & `bionumpy-1.0.8/tests/test_wildcard_index.py`

 * *Files identical despite different names*

