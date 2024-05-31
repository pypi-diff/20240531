# Comparing `tmp/anospp_analysis-0.2.1.tar.gz` & `tmp/anospp_analysis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anospp_analysis-0.2.1.tar", max compression
+gzip compressed data, was "anospp_analysis-0.3.0.tar", max compression
```

## Comparing `anospp_analysis-0.2.1.tar` & `anospp_analysis-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-01-24 21:08:31.753757 anospp_analysis-0.2.1/LICENSE
--rw-r--r--   0        0        0     2639 2023-05-18 13:18:30.578112 anospp_analysis-0.2.1/README.md
--rw-r--r--   0        0        0       21 2023-05-18 13:18:45.058645 anospp_analysis-0.2.1/anospp_analysis/__init__.py
--rw-r--r--   0        0        0     6776 2023-05-18 09:50:03.443460 anospp_analysis-0.2.1/anospp_analysis/iplot.py
--rw-r--r--   0        0        0    26194 2023-05-18 12:21:59.393337 anospp_analysis-0.2.1/anospp_analysis/nn.py
--rw-r--r--   0        0        0    34887 2023-05-18 12:21:59.395203 anospp_analysis-0.2.1/anospp_analysis/plasm.py
--rw-r--r--   0        0        0     4457 2023-04-05 09:27:05.840619 anospp_analysis-0.2.1/anospp_analysis/prep.py
--rw-r--r--   0        0        0    10858 2023-05-18 12:21:59.397129 anospp_analysis-0.2.1/anospp_analysis/qc.py
--rw-r--r--   0        0        0     8737 2023-05-18 12:05:29.523105 anospp_analysis-0.2.1/anospp_analysis/test_functions_vae.py
--rw-r--r--   0        0        0    11738 2023-05-18 12:21:59.398743 anospp_analysis-0.2.1/anospp_analysis/util.py
--rw-r--r--   0        0        0    27689 2023-05-18 12:05:29.523497 anospp_analysis-0.2.1/anospp_analysis/vae.py
--rw-r--r--   0        0        0      732 2023-05-18 13:18:39.045673 anospp_analysis-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 anospp_analysis-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-10 08:03:04.746026 anospp_analysis-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2639 2023-06-10 08:03:04.746214 anospp_analysis-0.3.0/README.md
+-rw-r--r--   0        0        0       21 2024-05-31 12:52:27.009582 anospp_analysis-0.3.0/anospp_analysis/__init__.py
+-rw-r--r--   0        0        0     8792 2024-05-31 12:52:27.012158 anospp_analysis-0.3.0/anospp_analysis/agg.py
+-rw-r--r--   0        0        0     8071 2024-05-31 12:52:27.014663 anospp_analysis-0.3.0/anospp_analysis/iplot.py
+-rw-r--r--   0        0        0    38696 2024-05-31 12:52:27.017203 anospp_analysis-0.3.0/anospp_analysis/nn.py
+-rw-r--r--   0        0        0    16593 2024-05-31 12:52:27.020537 anospp_analysis-0.3.0/anospp_analysis/plasm.py
+-rw-r--r--   0        0        0     5095 2024-05-31 12:52:27.022236 anospp_analysis-0.3.0/anospp_analysis/prep.py
+-rw-r--r--   0        0        0    18538 2024-05-31 12:52:27.023774 anospp_analysis-0.3.0/anospp_analysis/qc.py
+-rw-r--r--   0        0        0     8737 2023-06-10 08:03:04.748457 anospp_analysis-0.3.0/anospp_analysis/test_functions_vae.py
+-rw-r--r--   0        0        0    15727 2024-05-31 12:52:27.025399 anospp_analysis-0.3.0/anospp_analysis/util.py
+-rw-r--r--   0        0        0    26547 2024-05-31 12:52:27.027657 anospp_analysis-0.3.0/anospp_analysis/vae.py
+-rw-r--r--   0        0        0      794 2024-05-31 12:52:27.036311 anospp_analysis-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 anospp_analysis-0.3.0/PKG-INFO
```

### Comparing `anospp_analysis-0.2.1/LICENSE` & `anospp_analysis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anospp_analysis-0.2.1/README.md` & `anospp_analysis-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `anospp_analysis-0.2.1/anospp_analysis/iplot.py` & `anospp_analysis-0.3.0/anospp_analysis/iplot.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 from bokeh.transform import dodge
 
 import os
 import matplotlib
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 
-from .util import *
+from anospp_analysis.util import *
 
 
-def view_alignment(aln, aln_view_fn, fontsize="9pt", plot_width=1200):
-    """Bokeh sequence alignment view"""
+def view_alignment(aln, aln_view_fn, fontsize='9pt', plot_width=1200):
+    '''Bokeh sequence alignment view'''
 
     def get_colors(seqs):
-        """make colors for bases in sequence"""
+        '''make colors for bases in sequence'''
         text = [i for s in list(seqs) for i in s]
         clrs =  {'a':'red','t':'green','g':'orange','c':'blue','-':'white', 'n':'black'}
         colors = [clrs[i] for i in text]
         return colors
 
-    output_file(filename=aln_view_fn, title="Static HTML file")
+    output_file(filename=aln_view_fn, title='Static HTML file')
 
     #make sequence and id lists from the aln object
     seqs = [rec.seq for rec in (aln)]
     ids = [rec.id for rec in aln]    
     text = [i for s in list(seqs) for i in s]
     colors = get_colors(seqs)    
     N = len(seqs[0])
@@ -53,136 +53,166 @@
     x_range = Range1d(0,N+1, bounds='auto')
     if N>100:
         viewlen=100
     else:
         viewlen=N
     #view_range is for the close up view
     view_range = (0,viewlen)
-    tools="xpan, xwheel_zoom, reset, save"
+    tools='xpan, xwheel_zoom, reset, save'
 
     #entire sequence view (no text, with zoom)
     p = figure(title=None, width = plot_width, height=50,
                x_range=x_range, y_range=(0,S), tools=tools,
                min_border=0, toolbar_location='below')
-    rects = Rect(x="x", y="recty",  width=1, height=1, fill_color="colors",
+    rects = Rect(x='x', y='recty',  width=1, height=1, fill_color='colors',
                  line_color=None, fill_alpha=0.6)
     p.add_glyph(source, rects)
     p.yaxis.visible = False
     p.grid.visible = False  
 
     #sequence text view with ability to scroll along x axis
     p1 = figure(title=None, width=plot_width, height=plot_height,
-                x_range=view_range, y_range=ids, tools="xpan,reset",
+                x_range=view_range, y_range=ids, tools='xpan,reset',
                 min_border=0, toolbar_location='below')#, lod_factor=1)          
-    glyph = Text(x="x", y="y", text="text", text_align='center',text_color="black",
-                text_font="monospace",text_font_size=fontsize)
-    rects = Rect(x="x", y="recty",  width=1, height=1, fill_color="colors",
+    glyph = Text(x='x', y='y', text='text', text_align='center',text_color='black',
+                text_font='monospace',text_font_size=fontsize)
+    rects = Rect(x='x', y='recty',  width=1, height=1, fill_color='colors',
                 line_color=None, fill_alpha=0.4)
     p1.add_glyph(source, glyph)
     p1.add_glyph(source, rects)
 
     p1.grid.visible = False
-    p1.xaxis.major_label_text_font_style = "bold"
+    p1.xaxis.major_label_text_font_style = 'bold'
     p1.yaxis.minor_tick_line_width = 0
     p1.yaxis.major_tick_line_width = 0
 
     p = gridplot([[p],[p1]], toolbar_location='below')
     save(p)
 
-def plot_plate_view(df, fname, target, reference, title=None):
+def plot_plate_view(df, out_fn, reference_path, title=None):
 
-    """
+    '''
     Plots a plate map for a given plate and Plasmodium type.
 
-    Parameters:
-    df (pandas.DataFrame): The DataFrame to plot.
-    P (str): The Plasmodium type to plot the total reads for.
-    title (str): The title for the plot. Default is None.
-    plate (str): The name of the plate. Default is None.
-    annot (bool): Whether to annotate the heatmap with the values. Default is True.
-    cmap (str): The color map to use for the heatmap. Default is 'coolwarm'.
-    center (float): The center value for the color map. Default is None.
+    Args:
+    - df (pandas.DataFrame): DataFrame to plot.
+    - out_fn (str): name of the file to save the plot
+    - reference_path (str): path to the reference directory
+    - title (str): title for the plot. Default is None.
 
     Returns:
     None.
-    """
+    '''
+
+    assert os.path.isdir(reference_path), f'{reference_path} reference directory does not exist'
 
- 
     # set the output filename
-    output_file(fname)
+    output_file(out_fn)
 
     #extract the column and generate the row values
-    cols = list(map(str, sorted(df.lims_row.unique().tolist())))
+    cols = list('ABCDEFGHIJKLMNOP')
     rows = [str(x) for x in range(1, 25)]
-    df["species_count"] = df["species_count"].astype(str)
-    df["row"] = df["lims_col"].astype(str)
-    df["col"] = df["lims_row"].astype(str)
-
-    #remove all NaNs
-    df = df[df.species_count != "nan"]
+    df = df.reset_index(drop=False)
+    df['col'] = df['lims_well_id'].str[0]
+    df['row'] = df['lims_well_id'].str[1:]
+    
+    # display values
+    df['P1_hapids_disp'] = df['P1_hapids_pass'].str.replace(',.*', '...', regex=True)
+    df['P2_hapids_disp'] = df['P2_hapids_pass'].str.replace(',.*', '...', regex=True)
+    df['comb_hapids_disp'] = df['P1_hapids_disp'] + '\n' + df['P2_hapids_disp']
 
-    #load the datframe into the source
+    #load the dataframe into the source
     source = ColumnDataSource(df)
 
     #set up the figure
-    p = figure(width=1300, height=600, title=title,
-               x_range=rows, y_range=list(reversed(cols)), toolbar_location=None, tools=[HoverTool(), 'pan', 'wheel_zoom', 'reset'])
+    p = figure(
+        width=1300,
+        height=600,
+        title=title,
+        x_range=rows,
+        y_range=list(reversed(cols)),
+        toolbar_location=None,
+        tools=[HoverTool(), 'pan', 'wheel_zoom', 'reset']
+        )
 
     # add grid lines
     for v in range(len(rows)):
-        vline = Span(location=v, dimension='height', line_color='black')
+        line_width = 2 if (v % 2 == 0) else 1
+        vline = Span(location=v, dimension='height', line_color='black', line_width=line_width)
         p.renderers.extend([vline])
 
     for h in range(len(cols)):
-        hline = Span(location=h, dimension='width', line_color='black')
+        line_width = 2 if (h % 2 == 0) else 1
+        hline = Span(location=h, dimension='width', line_color='black', line_width=line_width)
         p.renderers.extend([hline])
 
     #load colors
-    if not os.path.isfile(f'{reference}/species_colours.csv'):
-        logging.warning('No colors defined for plotting.')
+    if not os.path.isfile(f'{reference_path}/species_colours.csv'):
+        logging.warning('no colors defined for plotting')
         cmap = {}
     else:
-        colors = pd.read_csv(f'{reference}/species_colours.csv')
+        colors = pd.read_csv(f'{reference_path}/species_colours.csv')
         cmap = dict(zip(colors['species'], colors['color']))
 
-    # Assign grey color to data with more than one species
+    
     for index, row in df.iterrows():
+        # Assign grey color to data with more than one species
         if len(row['plasmodium_species'].split(',')) > 1:
             cmap[row['plasmodium_species']] = '#cfcfcf'
+        # Assign white color to data with no species
+        elif len(row['plasmodium_species']) == 0:
+            cmap[row['plasmodium_species']] = '#ffffff'
 
     #add the rectangles
-    p.rect("row", "col", 0.95, 0.95, source=source, fill_alpha=.9, legend_field="plasmodium_species",
-           color=factor_cmap('plasmodium_species', palette=list(cmap.values()), factors=list(cmap.keys())))
+    p.rect(
+        'row',
+        'col',
+        0.95,
+        0.95,
+        source=source,
+        fill_alpha=.9,
+        legend_field='plasmodium_species',
+        color=factor_cmap('plasmodium_species', palette=list(cmap.values()), factors=list(cmap.keys()))
+        )
 
     #add the species count text for each field
-    text_props = {"source": source, "text_align": "left", "text_baseline": "middle"}
-    x = dodge("row", -0.4, range=p.x_range)
-    if target == 'P1':
-        r = p.text(x=x, y="col", text="hap_ID_P1", **text_props, )
-
-    else:
-        r = p.text(x=x, y="col", text="hap_ID_P2", **text_props, )
-    r.glyph.text_font_size="10px"
-    r.glyph.text_font_style="bold"
+    text_props = {'source': source, 'text_align': 'left', 'text_baseline': 'middle'}
+    x = dodge('row', -0.4, range=p.x_range)
+    r = p.text(x=x, y='col', text='comb_hapids_disp', **text_props)
+    r.glyph.text_font_size = '10px'
+    r.glyph.text_font_style = 'bold'
 
     #set up the hover value
     p.add_tools(HoverTool(tooltips=[
-        ("sample id", "@{Source_sample}"),
-        ("Parasite species", "@plasmodium_species"),
-        ("Detection confidence", "@plasmodium_status"),
-        ("P1 & P2 consistency", "@P1_P2_consistency"),
-        ("P1 haplotype ID", "@hap_ID_P1"),
-        ("Total P1 read count", "@total_reads_P1"),
-        ("P2 haplotype ID", "@hap_ID_P2"),
-        ("Total P2 read count", "@total_reads_P2"),
+        ('sample id', '@{sample_id}'),
+        ('Parasite species', '@plasmodium_species'),
+        ('Detection status', '@plasmodium_detection_status'),
+        ('P1 total reads', '@P1_reads_total'),
+        ('P1 QC pass reads', '@P1_reads_pass'),
+        ('P1 QC pass haplotype IDs', '@P1_hapids_pass'),
+        ('P1 reads per QC pass haplotype', '@P1_hapids_pass_reads'),
+        ('P1 species assignments for pass haplotypes', '@P1_species_assignments_pass'),
+        ('P1 contamination haplotype IDs', '@P1_hapids_contam'),
+        ('P1 reads per contamination haplotype', '@P1_hapids_contam_reads'),
+        ('P1 low coverage haplotype IDs', '@P1_hapids_locov'),
+        ('P1 reads per low coverage haplotype', '@P1_hapids_locov_reads'),
+        ('P2 total reads', '@P2_reads_total'),
+        ('P1 QC pass reads', '@P2_reads_pass'),
+        ('P2 QC pass haplotype IDs', '@P2_hapids_pass'),
+        ('P2 reads per QC pass haplotype', '@P2_hapids_pass_reads'),
+        ('P2 species assignments for pass haplotypes', '@P2_species_assignments_pass'),
+        ('P2 contamination haplotype IDs', '@P2_hapids_contam'),
+        ('P2 reads per contamination haplotype', '@P2_hapids_contam_reads'),
+        ('P2 low coverage haplotype IDs', '@P2_hapids_locov'),
+        ('P2 reads per low coverage haplotype', '@P2_hapids_locov_reads'),
     ]))
 
     #set up the rest of the figure and save the plot
     p.outline_line_color = 'black'
     p.grid.grid_line_color = None
     p.axis.axis_line_color = 'black'
     p.axis.major_tick_line_color = None
     p.axis.major_label_standoff = 0
-    p.legend.orientation = "vertical"
-    p.legend.click_policy="hide"
+    p.legend.orientation = 'vertical'
+    p.legend.click_policy='hide'
     p.add_layout(p.legend[0], 'right') 
     save(p)
```

### Comparing `anospp_analysis-0.2.1/anospp_analysis/nn.py` & `anospp_analysis-0.3.0/anospp_analysis/nn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
-from collections import OrderedDict
+import matplotlib.patches as mpatches
 import os
 import argparse
 import itertools
 
-from .util import *
+from anospp_analysis.util import *
 
 def recompute_haplotype_coverage(hap_df):
-    hap_df = hap_df.drop(["total_reads", "reads_fraction", "nalleles"], axis=1)
+    hap_df = hap_df.drop(['total_reads', 'reads_fraction', 'nalleles'], axis=1)
 
     hap_df['total_reads'] = hap_df.groupby(by=['sample_id', 'target']) \
             ['reads'].transform('sum')
 
     hap_df['reads_fraction'] = hap_df['reads'] / hap_df['total_reads']
 
     hap_df['nalleles'] = hap_df.groupby(by=['sample_id', 'target']) \
@@ -27,18 +27,22 @@
     change targets to integers
     returns haplotype dataframe
     '''
 
     logging.info('preparing mosquito haplotypes')
 
     hap_df = hap_df.astype({'target': str})
-    filtered_hap_df = hap_df[(hap_df.reads>=int(rc_threshold)) & (hap_df.reads_fraction>=float(rf_threshold))]
+    filtered_hap_df = hap_df[
+        (hap_df.reads >= rc_threshold) & (hap_df.reads_fraction >= rf_threshold)
+        ]
     if filtered_hap_df.shape[0] < hap_df.shape[0]:
-        logging.warning(f'Removed {hap_df.shape[0] - filtered_hap_df.shape[0]} haplotypes \
-                    with fewer than {rc_threshold} reads or lower fracion than {rf_threshold} of reads')
+        logging.info(
+            f'removed {hap_df.shape[0] - filtered_hap_df.shape[0]} haplotypes '
+            f'with fewer than {rc_threshold} reads or fraction lower than {rf_threshold} of reads'
+        )
     mosq_hap_df = filtered_hap_df[filtered_hap_df.target.isin(MOSQ_TARGETS)]
     mosq_hap_df = mosq_hap_df.astype({'target': int})
 
     #recompute reads coverage after filtering
     mosq_hap_df = recompute_haplotype_coverage(mosq_hap_df)
 
     return mosq_hap_df
@@ -50,40 +54,40 @@
 
     logging.info(f'importing reference index {reference_version}')
 
     reference_path = f'{path_to_refversion}/{reference_version}/'
 
     assert os.path.isdir(reference_path), f'reference version {reference_version} does not exist at {reference_path}'
 
-    assert os.path.isfile(f'{reference_path}/haplotypes.tsv'), f'reference version {reference_version} at {reference_path} \
-        does not contain required haplotypes.tsv file'
+    assert os.path.isfile(f'{reference_path}/haplotypes.tsv'), \
+        f'reference version {reference_version} at {reference_path} does not contain required haplotypes.tsv file'
     ref_hap_df = pd.read_csv(f'{reference_path}/haplotypes.tsv', sep='\t')
 
-    assert os.path.isfile(f'{reference_path}/multiallelism.tsv'), f'reference version {reference_version} at {reference_path} \
-        does not contain required multiallelism.tsv file'
+    assert os.path.isfile(f'{reference_path}/multiallelism.tsv'), \
+        f'reference version {reference_version} at {reference_path} does not contain required multiallelism.tsv file'
     true_multi_targets = pd.read_csv(f'{reference_path}/multiallelism.tsv', sep='\t')
 
     if os.path.isfile(f'{reference_path}/version.txt'):
         with open(f'{reference_path}/version.txt', 'r') as fn:
             for line in fn:
                 version_name = line.strip()
     else:
         logging.warning('No version.txt file present for reference version {reference_version} at {reference_path}')
         version_name = 'unknown'
 
     allele_freqs = dict()
     colors = dict()
     for level in ['coarse', 'int', 'fine']:
-        assert os.path.isfile(f'{reference_path}/allele_freq_{level}.npy'), f'reference version {reference_version} at {reference_path} \
-            does not contain required allele_freq_{level}.npy file'
+        assert os.path.isfile(f'{reference_path}/allele_freq_{level}.npy'), \
+            f'reference version {reference_version} at {reference_path} does not contain required allele_freq_{level}.npy file'
         af = np.load(f'{reference_path}/allele_freq_{level}.npy')
         allele_freqs[level] = af
 
-        assert os.path.isfile(f'{reference_path}/sgp_{level}.txt'), f'reference version {reference_version} at {reference_path} \
-            does not contain required sgp_{level}.txt file'
+        assert os.path.isfile(f'{reference_path}/sgp_{level}.txt'), \
+            f'reference version {reference_version} at {reference_path} does not contain required sgp_{level}.txt file'
         sgp = []
         with open(f'{reference_path}/sgp_{level}.txt', 'r') as fn:
             for line in fn:
                 sgp.append(line.strip())
 
         ref_hap_df[f'{level}_sgp'] = pd.Categorical(ref_hap_df[f'{level}_sgp'], sgp, ordered=True)
 
@@ -146,52 +150,54 @@
     '''
 
     logging.info('translating unique sequences to k-mers')
 
     kmerdict = construct_kmer_dict(k)
     #subset to unique haplotypes
     uniqueseq = mosq_hap_df[['seqid', 'consensus']].drop_duplicates()
-    #determine shape of table by highest seqid
+    #determine shape of table by top seqid
     parsed_seqids = parse_seqids_series(uniqueseq.seqid)
-    maxid = parsed_seqids['uidx'].max()+1
+    maxid = parsed_seqids['uidx'].max() + 1
 
     #initiate table to store kmer counts
     kmer_table = np.zeros((len(MOSQ_TARGETS), maxid, 4**k), dtype='int')
     #translate each unique haplotype to kmer counts
     for idx, seq in uniqueseq.iterrows():
-        tgt = parsed_seqids.loc[idx,'target']
-        id = parsed_seqids.loc[idx,'uidx']
+        tgt = parsed_seqids.loc[idx, 'target']
+        uid = parsed_seqids.loc[idx, 'uidx']
         consensus = seq.consensus
-        for i in np.arange(len(consensus)-(k-1)):
-            kmer_table[tgt,id,kmerdict[consensus[i:i+k]]] += 1
+        for i in np.arange(len(consensus) - (k - 1)):
+            kmer_table[tgt, uid, kmerdict[consensus[i:i+k]]] += 1
     return kmer_table
 
 def identify_error_seqs(mosq_hap_df, kmers, k, n_error_snps):
     '''
     Identify haplotypes resulting from sequencing/PCR errors
     Cannot distinguish between true heterozygote, contaminated homozygote and homozygote with error sequence
     So only look for errors for unique sequences at multiallelic targets
     '''
 
     logging.info('identifying haplotypes resulting from sequencing/PCR errors')
     #set the k-mer threshold for the number of snps allowed for errors
-    threshold=n_error_snps*k+1
+    threshold = n_error_snps * k + 1
     seqid_size = mosq_hap_df.groupby('seqid').size()
-    singleton_seqids = seqid_size[seqid_size==1].index
+    singleton_seqids = seqid_size[seqid_size == 1].index
     error_candidates = mosq_hap_df.query('(seqid in @singleton_seqids) & (nalleles>2)')
 
     error_seqs = []
     for _, cand in error_candidates.iterrows():
-        possible_sources = mosq_hap_df.query('(sample_id == @cand.sample_id) & (target == @cand.target) & \
-                                             (not seqid in @error_seqs) & (seqid != @cand.seqid)')
+        possible_sources = mosq_hap_df.query(
+            '(sample_id == @cand.sample_id) & (target == @cand.target) & (seqid != @cand.seqid)')
         cand_parsed_seqid = parse_seqid(cand.seqid)
         possible_sources_parsed_seqids = parse_seqids_series(possible_sources.seqid)
         for possible_source in possible_sources_parsed_seqids['uidx']:
-            abs_kmer_dist = np.abs(kmers[cand.target,cand_parsed_seqid[1],:] - kmers[cand.target,possible_source,:]).sum()
-            if abs_kmer_dist<threshold:
+            abs_kmer_dist = np.abs(
+                kmers[cand.target, cand_parsed_seqid[1], :] - kmers[cand.target, possible_source, :]
+                ).sum()
+            if abs_kmer_dist < threshold:
                 error_seqs.append(cand.seqid)
                 break
     
     logging.info(f'identified {len(error_seqs)} error sequences')
 
     return error_seqs
 
@@ -217,15 +223,15 @@
     '''
     #get idxs occupied for each target
     parsed_ref_seqids = parse_seqids_series(ref_hap_df.seqid.drop_duplicates())
     ref_idxs_per_target = parsed_ref_seqids.groupby('target')['uidx'].unique()
 
     nndict = dict()
 
-    logging.info(f"identifying nearest neighbours for {non_error_hap_df.seqid.nunique()} unique haplotypes")
+    logging.info(f'identifying nearest neighbours for {non_error_hap_df.seqid.nunique()} unique haplotypes')
     
     #loop through unique haplotypes
     unique_seqids = non_error_hap_df.seqid.unique()
     for seqid in unique_seqids:
         tgt, qidx = parse_seqid(seqid)
         #compute distance between focal hap and all same target haps in ref index
         dist, norm_dist = compute_kmer_distance(kmers, ref_kmers, tgt, qidx, ref_idxs_per_target[tgt])
@@ -241,280 +247,614 @@
     #lookup nearest neighbour identifiers
     nnids = nndict[q_seqid][0]
     #lookup allele frequencies of nnids
     af_nn = allele_frequencies[tgt, nnids, :]
     #sum allele frequencies over nnids
     summed_af_nn = np.sum(af_nn, axis=0)
     #normalise proportion and weigth in number of alleles
-    assignment_proportion = weight*summed_af_nn/np.sum(summed_af_nn)
+    assignment_proportion = weight * summed_af_nn / np.sum(summed_af_nn)
     return assignment_proportion
 
-def perform_nn_assignment_samples(hap_df, ref_hap_df, nndict, allele_freqs,\
-                                  normalisation):
+def perform_nn_assignment_samples(hap_df, ref_hap_df, nndict, allele_freqs, normalisation):
     '''
     The main NN assignment function
     it outputs three dataframes containing the assignment proportions to each species-group for the three levels
     '''
     #get samples with at least 10 targets
-    test_samples = hap_df.groupby('sample_id').filter(lambda x: x['target'].nunique() >=10)['sample_id'].unique()
+    test_samples = hap_df \
+        .groupby('sample_id') \
+        .filter(lambda x: x['target'].nunique() >= 10)['sample_id'] \
+        .unique()
 
     logging.info(f'performing NN assignment for {len(test_samples)} samples with >=10 mosquito targets')
 
     #set up data-output as numpy arrays (will be made into dataframes later)
-    results = dict({'coarse': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['coarse'].shape[2])), \
-                    'int': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['int'].shape[2])), \
-                    'fine': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['fine'].shape[2]))})
+    results = {
+        'coarse': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['coarse'].shape[2])),
+        'int': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['int'].shape[2])),
+        'fine': np.zeros((len(MOSQ_TARGETS), len(test_samples), allele_freqs['fine'].shape[2]))
+    }
 
     for i, sample in enumerate(test_samples):
         #Restrict to targets amplified in focal sample
         targets = hap_df.loc[hap_df.sample_id == sample, 'target'].unique()
         
         #Per amplified target
         for tgt in targets:
             #Identify the unique IDs of the focal sample's haplotypes at target t
-            alleles = hap_df.loc[(hap_df.sample_id == sample) & (hap_df.target == tgt), ['seqid', 'reads_fraction']]
+            alleles = hap_df.loc[
+                (hap_df.sample_id == sample) & (hap_df.target == tgt),
+                ['seqid', 'reads_fraction']]
             #for each haplotype
             for _, allele in alleles.iterrows():
                 #for each assignment level
                 for level in ['coarse', 'int', 'fine']:
                     if normalisation == 'n_alleles':
                     #lookup assignment proportion
-                        assignment_proportion = lookup_assignment_proportion(allele.seqid, allele_freqs[level], \
-                                                    tgt, nndict, 1/alleles.shape[0])
+                        assignment_proportion = lookup_assignment_proportion(
+                            allele.seqid,
+                            allele_freqs[level],
+                            tgt,
+                            nndict,
+                            1 / alleles.shape[0]
+                            )
                     elif normalisation == 'reads_fraction':
-                        assignment_proportion = lookup_assignment_proportion(allele.seqid, allele_freqs[level], \
-                                                    tgt, nndict, allele.reads_fraction)
+                        assignment_proportion = lookup_assignment_proportion(
+                            allele.seqid,
+                            allele_freqs[level],
+                            tgt,
+                            nndict,
+                            allele.reads_fraction
+                        )
                     else:
-                        logging.error("Not a valid allelism_normalisation method.")
+                        logging.error('Not a valid allelism_normalisation method.')
                     #table[tgt,nsmp,:] += assignment_proportion
-                    results[level][tgt,i,:] += assignment_proportion
+                    results[level][tgt, i, :] += assignment_proportion
 
     #print(f'shape of results arrays is {results_coarse.shape}, {results_int.shape} and {results_fine.shape}')
-    results_df = dict()
+    results_dfs = dict()
     for level in ['coarse', 'int', 'fine']:
         #Average assignment results over amplified targets
         res = np.nansum(results[level], axis=0)/np.sum(np.nansum(results[level], axis=0), axis=1)[:,None]
         #Convert results to dataframes
-        results_df[level] = pd.DataFrame(res, index=test_samples, columns=ref_hap_df[f'{level}_sgp'].cat.categories)  
-    return results_df, test_samples
+        results_dfs[level] = pd.DataFrame(
+            res, 
+            index=test_samples, 
+            columns=ref_hap_df[f'{level}_sgp'].cat.categories
+        )  
+    return results_dfs, test_samples
 
 def recompute_sample_coverage(comb_stats_df, non_error_hap_df):
     '''
     recompute coverage stats after filtering and error removal
     '''
     logging.info('recompute coverage stats')
     comb_stats_df.set_index('sample_id', inplace=True)
 
     #recompute multiallelic calls after filtering and error removal
-    comb_stats_df['multiallelic_mosq_targets'] = (non_error_hap_df.groupby('sample_id')['target'].value_counts() > 2 \
+    comb_stats_df['multiallelic_mosq_targets'] = (
+        non_error_hap_df.groupby('sample_id')['target'].value_counts() > 2
         ).groupby(level='sample_id').sum()
-    comb_stats_df['multiallelic_mosq_targets'] = comb_stats_df['multiallelic_mosq_targets'].fillna(0)
 
     #recompute read counts after filtering and error removal
     comb_stats_df['mosq_reads'] = non_error_hap_df.groupby('sample_id')['reads'].sum()
-    comb_stats_df['mosq_reads'] = comb_stats_df['mosq_reads'].fillna(0)
 
     #recompute targets recovered after filtering and error removal
     comb_stats_df['mosq_targets_recovered'] = non_error_hap_df.groupby('sample_id')['target'].nunique()
-    comb_stats_df['mosq_targets_recovered'] = comb_stats_df['mosq_targets_recovered'].fillna(0)
+
+    for col in ['multiallelic_mosq_targets', 'mosq_reads', 'mosq_targets_recovered']:
+        comb_stats_df[col] = comb_stats_df[col].fillna(0).astype(int)
 
     comb_stats_df.reset_index(inplace=True)
 
     return comb_stats_df
 
-def estimate_contamination(comb_stats_df, non_error_hap_df, true_multi_targets, \
-                           rc_med_threshold, ma_med_threshold, ma_hi_threshold):
+def estimate_contamination(comb_stats_df, non_error_hap_df, true_multi_targets,
+                           rc_med_threshold, ma_med_threshold, ma_hi_threshold, ma_vh_threshold):
     '''
     estimate contamination from read counts and multiallelic targets
     '''
     logging.info('estimating contamination risk')
 
     #Read in exceptions from true_multi_targets file
     for idx, item in true_multi_targets.iterrows():
-        potentially_affected_samples = comb_stats_df.loc[comb_stats_df[f'res_{item.level}'] == item.sgp, 'sample_id']
-        affected_samples = non_error_hap_df.query('sample_id in @potentially_affected_samples & target == @item.target') \
-            .groupby('sample_id').filter(lambda x: x['seqid'].nunique() > 2 & \
-                                         x['seqid'].nunique() < item.admissable_alleles)['sample_id'].unique()
+        potentially_affected_samples = comb_stats_df.loc[comb_stats_df[f'nn_{item.level}'] == item.sgp, 'sample_id']
+        affected_samples = non_error_hap_df \
+            .query('(sample_id in @potentially_affected_samples) & (target == @item.target)') \
+            .groupby('sample_id') \
+            .filter(
+                lambda x: (x['seqid'].nunique() > 2) & (x['seqid'].nunique() <= item.admissable_alleles)
+                ) \
+            ['sample_id'].unique()
         comb_stats_df.loc[comb_stats_df.sample_id.isin(affected_samples), 'multiallelic_mosq_targets'] -= 1
 
-    comb_stats_df.loc[comb_stats_df.multiallelic_mosq_targets>int(ma_hi_threshold), 'contamination_risk'] = 'high'
-    comb_stats_df.loc[((comb_stats_df.multiallelic_mosq_targets>int(ma_med_threshold)) & \
-                       (comb_stats_df.multiallelic_mosq_targets<=int(ma_hi_threshold))) |\
-        (comb_stats_df.mosq_reads<int(rc_med_threshold)), 'contamination_risk'] = 'medium'
-    comb_stats_df.loc[comb_stats_df.contamination_risk.isnull(), 'contamination_risk'] = 'low'
-
-    logging.info(f"Identified {(comb_stats_df.contamination_risk=='high').sum()} samples with high contamination risk, \
-        \n {(comb_stats_df.contamination_risk=='medium').sum()} samples with medium contamination risk \
-        \n and {(comb_stats_df.contamination_risk=='low').sum()} samples with low contamination risk")
+    comb_stats_df['contamination_risk'] = 'low'
+    comb_stats_df.loc[
+        comb_stats_df.mosq_reads < rc_med_threshold,
+        'contamination_risk'
+    ] = 'medium'
+    comb_stats_df.loc[
+        comb_stats_df.multiallelic_mosq_targets > ma_med_threshold,
+        'contamination_risk'
+    ] = 'medium'
+    comb_stats_df.loc[
+        comb_stats_df.multiallelic_mosq_targets > ma_hi_threshold,
+        'contamination_risk'
+    ] = 'high'
+    comb_stats_df.loc[
+        comb_stats_df.multiallelic_mosq_targets > ma_vh_threshold,
+        'contamination_risk'
+    ] = 'very_high'
+
+    logging.info(
+        f'identified {(comb_stats_df.contamination_risk == "very_high").sum()} samples with very high contamination risk, '
+        f'{(comb_stats_df.contamination_risk == "high").sum()} samples with high contamination risk, '
+        f'{(comb_stats_df.contamination_risk == "medium").sum()} samples with medium contamination risk '
+        f'and {(comb_stats_df.contamination_risk == "low").sum()} samples with low contamination risk'
+        )
 
     return comb_stats_df
 
-def generate_hard_calls(comb_stats_df, non_error_hap_df, test_samples, results_df, \
-                        true_multi_targets, nn_asgn_threshold, \
-                        rc_med_threshold, ma_med_threshold, ma_hi_threshold):
+def generate_hard_calls(comb_stats_df, non_error_hap_df, test_samples, results_dfs,
+                        true_multi_targets, nn_asgn_threshold,
+                        rc_med_threshold, ma_med_threshold, ma_hi_threshold, ma_vh_threshold):
 
     logging.info('generating NN calls from assignment info')
 
     #Account for filtering and error removal
     comb_stats_df = recompute_sample_coverage(comb_stats_df, non_error_hap_df)
 
     #Record whether NN assignment was performed
-    comb_stats_df.loc[comb_stats_df.sample_id.isin(test_samples), 'NN_assignment'] = 'yes'
-    comb_stats_df.loc[comb_stats_df.NN_assignment.isnull(), 'NN_assignment'] = 'no'
+    comb_stats_df.loc[comb_stats_df.sample_id.isin(test_samples), 'nn_assignment'] = 'yes'
+    comb_stats_df.loc[comb_stats_df.nn_assignment.isnull(), 'nn_assignment'] = 'no'
 
     #Generate assignment hard calls if the threshold is met
     for level in ['coarse', 'int', 'fine']:
-        asgn_dict = dict(results_df[level].loc[(results_df[level]>=float(nn_asgn_threshold)).any(axis=1)].apply(\
-            lambda row: results_df[level].columns[row>=float(nn_asgn_threshold)][0], axis=1))
-        comb_stats_df[f'res_{level}'] = comb_stats_df.sample_id.map(asgn_dict)
+        asgn_dict = dict(results_dfs[level] \
+            .loc[(results_dfs[level] >= nn_asgn_threshold).any(axis=1)] \
+            .apply(
+                lambda row: results_dfs[level].columns[row >= nn_asgn_threshold][0],
+                axis=1))
+        comb_stats_df[f'nn_{level}'] = comb_stats_df.sample_id.map(asgn_dict)
+
+    comb_stats_df = estimate_contamination(
+        comb_stats_df,
+        non_error_hap_df,
+        true_multi_targets,
+        rc_med_threshold,
+        ma_med_threshold,
+        ma_hi_threshold,
+        ma_vh_threshold
+    )
+
+    comb_stats_df['nn_species_call'] = None
+    comb_stats_df['nn_call_method'] = None
+    # NN hierarchical assignment by level
+    for level in ['fine', 'int', 'coarse']:
+        leveldict = dict(zip(comb_stats_df.sample_id, comb_stats_df[f'nn_{level}']))
+        is_id_on_level = (comb_stats_df.nn_species_call.isnull() & ~comb_stats_df[f'nn_{level}'].isnull())
+        comb_stats_df.loc[is_id_on_level, 'nn_call_method'] = f'NN_{level}'
+        comb_stats_df.loc[is_id_on_level, 'nn_species_call'] = comb_stats_df.loc[
+            comb_stats_df.nn_call_method == f'NN_{level}', 'sample_id'
+            ].map(leveldict)
+    
+    #Rainbow samples
+    is_rainbow = (comb_stats_df.nn_species_call.isnull() & (comb_stats_df.nn_assignment == 'yes'))
+    comb_stats_df.loc[is_rainbow, 'nn_call_method'] = 'NN'
+    comb_stats_df.loc[is_rainbow, 'nn_species_call'] = 'RAINBOW_SAMPLE'
+
+    #Samples with too few targets
+    is_not_id = (comb_stats_df.nn_assignment == 'no')
+    comb_stats_df.loc[is_not_id, 'nn_call_method'] = 'TOO_FEW_TARGETS'
+    comb_stats_df.loc[is_not_id, 'nn_species_call'] = 'TOO_FEW_TARGETS'
 
-    comb_stats_df = estimate_contamination(comb_stats_df, non_error_hap_df, true_multi_targets, \
-                                           rc_med_threshold, ma_med_threshold, ma_hi_threshold)
+    assert not comb_stats_df.nn_species_call.isnull().any(), 'some samples not assigned'
+    assert not comb_stats_df.nn_call_method.isnull().any(), 'some samples not assigned'
 
     return comb_stats_df
 
 def generate_summary(comb_stats_df, version_name):
 
-    summary = []
-    summary.append(f'Nearest Neighbour assignment using reference version {version_name}')
-    summary.append(f'On run containing {comb_stats_df.sample_id.nunique()} samples')
-    summary.append(f'{(comb_stats_df.contamination_risk=="high").sum()} samples have high contamination risk')
-    summary.append(f'{(comb_stats_df.contamination_risk=="medium").sum()} samples have medium contamination risk')
-    summary.append(f'{(comb_stats_df.contamination_risk=="low").sum()} samples have low contamination risk')
-    summary.append(f'{(comb_stats_df.NN_assignment=="no").sum()} samples with < 10 targets lack NN assignment')
-    summary.append(f'{(~comb_stats_df.res_coarse.isnull()).sum()} samples are assigned at coarse level')
-    summary.append(f'to {comb_stats_df.res_coarse.nunique()} different species groups')
-    summary.append(f'{(~comb_stats_df.res_int.isnull()).sum()} samples are assigned at intermediate level')
-    summary.append(f'to {comb_stats_df.res_int.nunique()} different species groups')
-    summary.append(f'{(~comb_stats_df.res_fine.isnull()).sum()} samples are assigned at fine level')
-    summary.append(f'to {comb_stats_df.res_fine.nunique()} different species groups')
-    summary.append(f'{comb_stats_df.loc[(comb_stats_df.NN_assignment=="yes") & (comb_stats_df.res_int.isnull()), "sample_id"].nunique()} \
-    samples with sufficient coverage could not be assigned at intermediate level')
-    summary.append(f'{comb_stats_df.loc[(comb_stats_df.NN_assignment=="yes") & (comb_stats_df.res_int.isnull()) & (comb_stats_df.contamination_risk != "low"), "sample_id"].nunique()} \
-    of those have medium or high contamination risk')
-    summary.append(f'{comb_stats_df.loc[(comb_stats_df.NN_assignment=="yes") & (comb_stats_df.res_coarse.isnull()), "sample_id"].nunique()} \
-    samples with sufficient coverage could not be assigned at coarse level')
-    summary.append(f'{comb_stats_df.loc[(comb_stats_df.NN_assignment=="yes") & (comb_stats_df.res_coarse.isnull()) & (comb_stats_df.contamination_risk != "low"), "sample_id"].nunique()} \
-    of those have medium or high contamination risk')
-    
+    summary = [
+        f'Nearest Neighbour assignment using reference version {version_name}',
+        f'On run containing {comb_stats_df.sample_id.nunique()} samples',
+        f'{(comb_stats_df.contamination_risk == "very_high").sum()} samples have very high contamination risk',
+        f'{(comb_stats_df.contamination_risk == "high").sum()} samples have high contamination risk',
+        f'{(comb_stats_df.contamination_risk == "medium").sum()} samples have medium contamination risk',
+        f'{(comb_stats_df.contamination_risk == "low").sum()} samples have low contamination risk',
+        f'{(comb_stats_df.nn_assignment=="no").sum()} samples with < 10 targets lack NN assignment',
+        f'{(~comb_stats_df.nn_coarse.isnull()).sum()} samples are assigned at coarse level',
+        f'to {comb_stats_df.nn_coarse.nunique()} different species groups',
+        f'{(~comb_stats_df.nn_int.isnull()).sum()} samples are assigned at intermediate level',
+        f'to {comb_stats_df.nn_int.nunique()} different species groups',
+        f'{(~comb_stats_df.nn_fine.isnull()).sum()} samples are assigned at fine level',
+        f'to {comb_stats_df.nn_fine.nunique()} different species groups',
+        f'{comb_stats_df.loc[comb_stats_df.nn_call_method == "NN_int", "sample_id"].nunique()} '
+         'samples with sufficient coverage could not be assigned at intermediate level',
+        f'{comb_stats_df.loc[(comb_stats_df.nn_call_method == "NN_int") & (comb_stats_df.contamination_risk != "low"), "sample_id"].nunique()} '
+         'of those have medium or higher contamination risk',
+        f'{comb_stats_df.loc[comb_stats_df.nn_call_method == "NN_coarse", "sample_id"].nunique()} '
+         'samples with sufficient coverage could not be assigned at coarse level',
+        f'{comb_stats_df.loc[(comb_stats_df.nn_call_method == "NN_coarse") & (comb_stats_df.contamination_risk != "low"), "sample_id"].nunique()} '
+         'of those have medium or higher contamination risk'
+    ]
     return '\n'.join(summary)
 
-def plot_assignment_proportions(nn_level_result_df, level_label, colors, nn_asgn_threshold):
+def plot_assignment_proportions(comb_stats_df, nn_level_result_df, level_label, level_colors, nn_asgn_threshold, run_id, 
+                                plasm_assignment_fn, plasm_colors_fn, read_count_threshold, legend_cutoff):
     
-    logging.info(f'Generate {level_label} level plots')
+    logging.info(f'generating {level_label} level plots')
     #Generate bar plots at given assignment level
-    width = min(20, .5*nn_level_result_df.shape[0])
-    fig, ax = plt.subplots(figsize=(width,7))
-    nn_level_result_df.plot(kind='bar', stacked=True, width=1, ax=ax, color=colors)
-    ax.set_xticklabels('')
-    ax.set_xticks([])
-    ax.set_title(f"{level_label} level assignment")
-    ax.hlines(float(nn_asgn_threshold), -.5, nn_level_result_df.shape[0]-.5, color='k', ls = ':', linewidth=1)
-    box = ax.get_position()
-    ax.set_position([box.x0, box.y0+3/7*box.height, box.width, box.height*4/7])
-    leg1 = ax.legend(loc='upper center', ncol=7, bbox_to_anchor=(0.5, -.05), fontsize=8.7)
-    ax.margins(y=0)
-    return fig, ax
+    #Get row and col info from well_id for ordering samples
+    comb_stats_df['row_id'] = comb_stats_df.well_id.str[0]
+    comb_stats_df['col_id'] = comb_stats_df.well_id.str[1:].astype(int)
+    comb_stats_df['well_id'] = well_ordering(comb_stats_df['well_id'])
+    # comb_stats_df.sort_values(by=['plate_id', 'col_id', 'well_id'], inplace=True)
+    #add samples with <10 targets
+    nn_level_result_df = pd.concat([
+        nn_level_result_df, pd.DataFrame(
+            index=comb_stats_df.loc[
+                ~comb_stats_df.sample_id.isin(nn_level_result_df.index), 'sample_id'
+                ]
+            )
+        ]).fillna(0)
+
+    # contamination color scheme - applied to top ticks 
+    contam_colors = {
+        'low':'#808080',
+        'medium':'#FF9900',
+        'high':'#cc00FF',
+        'very_high':'#FF0000'
+    }
+
+    # plasm color scheme - applied to bottom ticks
+    if plasm_assignment_fn is not None and plasm_colors_fn is not None:
+        logging.info(f'using plasm predictions to colour sample labels')
+        plasm_df = pd.read_csv(plasm_assignment_fn, sep='\t')
+        plasm_df['plasmodium_species'] = plasm_df['plasmodium_species'].fillna('')
+        plasm_spp = plasm_df.set_index('sample_id')['plasmodium_species'].to_dict()
+        assert set(plasm_spp.keys()) == set(comb_stats_df.sample_id), \
+            'plasmodium assignment samples do not match nn samples'
+
+        plasm_colors = pd.read_csv(plasm_colors_fn).set_index('species')['color']
+        # named species in legend - remove genus name
+        plasm_legend_colors = {sp[11:]:color for sp, color in plasm_colors.iloc[:6].to_dict().items()}
+        # other species collapsed
+        assert plasm_colors.iloc[6:].nunique() == 1, \
+            'plasmodium species color scheme not matching nn plot expectation'
+        plasm_legend_colors['other'] = plasm_colors['unknown']
+        # mixed/uninfected inferred during plotting
+        plasm_legend_colors['mixed'] = '#000000'
+        plasm_legend_colors['none'] = '#808080'
+
+    # plot
+    plates = comb_stats_df.plate_id.unique()
+    nplates = comb_stats_df.plate_id.nunique()
+    fig, axs = plt.subplots(nplates, 1, figsize=(20, 4 * nplates))
+    if nplates == 1:
+        axs = [axs]
+    for plate, ax in zip(plates, axs):
+        plot_df = comb_stats_df[comb_stats_df.plate_id == plate].copy().reset_index()
+        plot_df['well_id'] = well_ordering(plot_df['well_id'])
+        plot_samples = plot_df['sample_id']
+        nn_level_result_df.loc[plot_samples].plot(
+            kind='bar', stacked=True, width=1, ax=ax, color=level_colors
+        )
+        ax.axhline(nn_asgn_threshold, color='k', ls=':', linewidth=1)
+        ax.set_ylim(0, 1)
+        ax.set_yticks([])
+        ax.set_ylabel(plate, fontsize=16)
+        handles, labels = ax.get_legend_handles_labels()
+        ax.get_legend().remove()
+        
+        ax.set_xticks(range(plot_df.shape[0]))
+        ax.set_xticklabels(plot_df['sample_name'])
+        if plasm_assignment_fn is not None and plasm_colors_fn is not None:
+            for i, r in plot_df.iterrows():
+                sample_plasm_sp = plasm_spp[r.sample_id]
+                # multiple species infection
+                if len(sample_plasm_sp.split(';')) > 1:
+                    ax.get_xticklabels()[i].set_color('black')
+                # species in index
+                elif sample_plasm_sp in plasm_colors.keys():
+                    ax.get_xticklabels()[i].set_color(plasm_colors[sample_plasm_sp])
+                # no infection
+                else:
+                    ax.get_xticklabels()[i].set_color('grey')
+        ax.tick_params(axis='x', rotation=90)
+        
+        ax2 = ax.twiny()
+        ax2.set_xticks(range(plot_df.shape[0]))
+        ax2.set_xticklabels(plot_df['mosq_targets_recovered'])
+        for i, r in plot_df.iterrows():
+            ax2.get_xticklabels()[i].set_color(contam_colors[r.contamination_risk])
+            if r.mosq_reads < read_count_threshold:
+                ax2.get_xticklabels()[i].set_fontstyle('oblique')
+        ax2.tick_params(axis='x', rotation=90)
+        ax2.set_xlim(ax.get_xlim())
+    plt.tight_layout()
+
+    # add legends after adjusting layout so that they span multiple subplots
+    contam_artist = axs[0].legend(
+        handles=[mpatches.Patch(color=color, label=label) for label, color in contam_colors.items()],
+        title='Total target count (top number) colored\nby contamination risk',
+        alignment='left',
+        bbox_to_anchor=(1,1.1),
+        fontsize=10,
+        ncols=2
+    )
+    axs[0].add_artist(contam_artist)
+
+    if plasm_assignment_fn is not None and plasm_colors_fn is not None:
+        plasm_artist = axs[0].legend(
+            handles=[mpatches.Patch(color=color, label=label) for label, color in plasm_legend_colors.items()],
+            title='Specimen ID label (bottom) colored by\nPlasmodium species detected',
+            bbox_to_anchor=(1,0.725),
+            alignment='left',
+            fontsize=10,
+            ncols=2
+        )
+        axs[0].add_artist(plasm_artist)
+
+    # subset legend to values observed over the cutoff
+    if legend_cutoff > 0:
+        logging.info(f'subsetting legend to observed labels at min frequency {legend_cutoff}')
+    flt_handles = []
+    flt_labels = []
+    for handle, label in zip(handles, labels):
+        max_freq = nn_level_result_df[label].max()
+        if max_freq >= legend_cutoff:
+            flt_handles.append(handle)
+            flt_labels.append(label)
+    # consistent legend title
+    leg_title_labels = {
+        'coarse':'Coarse',
+        'int':'Intermediate',
+        'fine':'Fine'
+    }
+    leg_title = f'{leg_title_labels[level_label]} level assignments'
+    if legend_cutoff > 0:
+        leg_title += f'\nwith observed proportion over {legend_cutoff}'
+    # reverse species legend order to match barplot order
+    axs[0].legend(
+        flt_handles[::-1], flt_labels[::-1], 
+        title=leg_title,
+        loc='upper left',
+        alignment='left',
+        bbox_to_anchor=(1,0.1), 
+        fontsize=10
+        )
+    # adding title in post - handling margins by savefig's bbox_inches='tight' at this point
+    axs[0].set_title(f'NN assignment {level_label} level for run {run_id}', fontsize=20)
+
+    return fig, axs
 
 
 def nn(args):
 
     setup_logging(verbose=args.verbose)
 
     os.makedirs(args.outdir, exist_ok =True)
 
     logging.info('ANOSPP NN data import started')
 
     hap_df = prep_hap(args.haplotypes)
-    samples_df = prep_samples(args.manifest)
+    run_id, samples_df = prep_samples(args.manifest)
     stats_df = prep_stats(args.stats)
 
     comb_stats_df = combine_stats(stats_df, hap_df, samples_df)
-    logging.info(f'starting NN assignment for {comb_stats_df.sample_id.nunique()} samples on current run')
-    mosq_hap_df = prep_mosquito_haps(hap_df, args.hap_read_count_threshold, \
-                                     args.hap_reads_fraction_threshold)
-
-    ref_hap_df, allele_freqs, true_multi_targets, \
-        colors, version_name = prep_reference_index(\
-        args.reference_version, path_to_refversion=args.path_to_refversion)
-
-    kmers = construct_unique_kmer_table(mosq_hap_df, int(args.kmer_length))
-    ref_kmers = construct_unique_kmer_table(ref_hap_df, int(args.kmer_length))
-
-    error_seqs = identify_error_seqs(mosq_hap_df, kmers, int(args.kmer_length), int(args.n_error_snps))
-    non_error_hap_df = mosq_hap_df[~mosq_hap_df.seqid.isin(error_seqs)]
-    non_error_hap_df = recompute_haplotype_coverage(non_error_hap_df)
-    non_error_hap_df.to_csv(f'{args.outdir}/non_error_haplotypes.tsv', index=False, sep='\t')
     
-    nndict = find_nn_unique_haps(non_error_hap_df, kmers, ref_hap_df, ref_kmers)
-    nn_df = pd.DataFrame.from_dict(nndict, orient='index', columns=['nn_id_array', 'nn_dist'])
-    nn_df['nn_id'] = ['|'.join(map(str, l)) for l in nn_df.nn_id_array]
-    nn_df[['nn_id', 'nn_dist']].to_csv(f'{args.outdir}/nn_dictionary.tsv', sep='\t')
-
-    results_df, test_samples = perform_nn_assignment_samples(\
-        non_error_hap_df, ref_hap_df, nndict, allele_freqs, args.allelism_normalisation)
-    for level in ['coarse', 'int', 'fine']:
-        results_df[level].to_csv(f"{args.outdir}/assignment_{level}.tsv", sep='\t')
+    logging.info(f'starting NN assignment for {comb_stats_df.sample_id.nunique()} samples in run {run_id}')
+    mosq_hap_df = prep_mosquito_haps(
+        hap_df,
+        args.hap_read_count_threshold,
+        args.hap_reads_fraction_threshold
+        )
+
+    ref_hap_df, allele_freqs, true_multi_targets, colors, version_name = prep_reference_index(
+        args.reference_version, 
+        path_to_refversion=args.path_to_refversion
+        )
+        
+    non_error_hap_fn = f'{args.outdir}/non_error_haplotypes.tsv'
+    nndict_fn = f'{args.outdir}/nn_dist_to_ref.tsv'
+    if args.resume and os.path.isfile(non_error_hap_fn) and os.path.isfile(nndict_fn):
+        logging.warning(f'reading non error haplotype data from {non_error_hap_fn}')
+        non_error_hap_df = pd.read_csv(non_error_hap_fn, sep='\t')
+
+        logging.warning(f'reading nndict from {nndict_fn}')
+        nndict = {}
+        with open(nndict_fn) as f:
+            next(f)
+            for line in f:
+                ll = line.strip().split('\t')
+                if len(ll) == 3:
+                    nndict[ll[0]] = ([int(i) for i in ll[1].split('|')], float(ll[2]))
+    else:
+        kmers = construct_unique_kmer_table(mosq_hap_df, args.kmer_length)
+        ref_kmers = construct_unique_kmer_table(ref_hap_df, args.kmer_length)
 
-    comb_stats_df = generate_hard_calls(comb_stats_df, non_error_hap_df, test_samples, \
-        results_df, true_multi_targets, args.nn_assignment_threshold, \
-            args.medium_contamination_read_count_threshold, \
-            args.medium_contamination_multi_allelic_threshold, \
-            args.high_contamination_multi_allelic_threshold)
+        error_seqs = identify_error_seqs(mosq_hap_df, kmers, args.kmer_length, args.n_error_snps)
+        non_error_hap_df = mosq_hap_df[~mosq_hap_df.seqid.isin(error_seqs)]
+        non_error_hap_df = recompute_haplotype_coverage(non_error_hap_df)
+        non_error_hap_df[[
+            'sample_id',
+            'target',
+            'consensus',
+            'reads',
+            'seqid',
+            'total_reads',
+            'reads_fraction',
+            'nalleles'
+        ]].to_csv(non_error_hap_fn, index=False, sep='\t')
+
+        nndict = find_nn_unique_haps(non_error_hap_df, kmers, ref_hap_df, ref_kmers)
+        nn_df = pd.DataFrame.from_dict(nndict, orient='index', columns=['nn_id_array', 'nn_dist'])
+        nn_df['nn_id'] = ['|'.join(map(str, l)) for l in nn_df.nn_id_array]
+        nn_df.index.name = 'seqid'
+        nn_df[['nn_id', 'nn_dist']].to_csv(
+            nndict_fn, 
+            sep='\t',
+            index=True
+            )
+
+    nn_assignment_fn = f'{args.outdir}/nn_assignment.tsv'
+    if args.resume and os.path.isfile(nn_assignment_fn):
+        logging.warning(f'reading nn assignments from {nn_assignment_fn}')
+        nn_stats_df = pd.read_csv(nn_assignment_fn, sep='\t')
+        comb_stats_df = pd.merge(comb_stats_df, nn_stats_df, on='sample_id', how='left')
+        results_dfs = {}
+        for level in ['coarse', 'int', 'fine']:
+            level_assignment_fn = f'{args.outdir}/assignment_{level}.tsv'
+            logging.warning(f'reading {level} assignments from {level_assignment_fn}')
+            # TODO fix heterogeneity in use of sample_id as index
+            results_dfs[level] = pd.read_csv(level_assignment_fn, sep='\t', index_col=0)
+    else:
+        results_dfs, test_samples = perform_nn_assignment_samples(
+            non_error_hap_df, 
+            ref_hap_df, 
+            nndict, 
+            allele_freqs, 
+            args.allelism_normalisation
+        )
+        for level in ['coarse', 'int', 'fine']:
+            results_dfs[level].to_csv(f'{args.outdir}/assignment_{level}.tsv', sep='\t')
 
-    logging.info(f'writing assignment results to {args.outdir}')
-    comb_stats_df.to_csv(f'{args.outdir}/nn_assignment.tsv', index=False, sep='\t')
+        comb_stats_df = generate_hard_calls(
+            comb_stats_df, 
+            non_error_hap_df, 
+            test_samples,
+            results_dfs, 
+            true_multi_targets, 
+            nn_asgn_threshold=args.nn_assignment_threshold,
+            rc_med_threshold=args.medium_contamination_read_count_threshold,
+            ma_med_threshold=args.medium_contamination_multi_allelic_threshold,
+            ma_hi_threshold=args.high_contamination_multi_allelic_threshold,
+            ma_vh_threshold=args.very_high_contamination_multi_allelic_threshold
+        )
+
+        comb_stats_df['nn_ref'] = args.reference_version
+        logging.info(f'writing assignment results to {nn_assignment_fn}')
+        comb_stats_df[[
+            'sample_id',
+            'run_id',
+            'multiallelic_mosq_targets',
+            'mosq_reads',
+            'mosq_targets_recovered',
+            'nn_assignment',
+            'nn_coarse',
+            'nn_int',
+            'nn_fine',
+            'contamination_risk',
+            'nn_species_call',
+            'nn_call_method',
+            'nn_ref'
+        ]].to_csv(nn_assignment_fn, index=False, sep='\t')
     
     summary_text = generate_summary(comb_stats_df, version_name)
-    logging.info(f'writing summary file to {args.outdir}')
-    with open(f'{args.outdir}/summary.txt', 'w') as fn:
+    summary_fn = f'{args.outdir}/nn_summary.txt'
+    logging.info(f'writing summary file to {summary_fn}')
+    with open(summary_fn, 'w') as fn:
         fn.write(summary_text)
 
-    if not bool(args.no_plotting):
+    if not args.no_plotting:
         for level in ['coarse', 'int', 'fine']:
-            fig, _ = plot_assignment_proportions(results_df[level], level, colors[level], args.nn_assignment_threshold)
-            fig.savefig(f'{args.outdir}/{level}_assignment.png')
+            fig_fn = f'{args.outdir}/{level}_assignment.png'
+            if args.resume and os.path.isfile(fig_fn):
+                logging.warning(f'nn figure {fig_fn} exists, not re-genrating')
+            else:
+                fig, _ = plot_assignment_proportions(
+                    comb_stats_df, 
+                    results_dfs[level], 
+                    level, 
+                    colors[level], 
+                    args.nn_assignment_threshold,
+                    run_id,
+                    args.plasm_assignment,
+                    args.plasm_colors,
+                    args.medium_contamination_read_count_threshold,
+                    args.legend_cutoff
+                    )
+                fig.savefig(fig_fn, bbox_inches='tight')
 
     logging.info('ANOSPP NN complete')
 
     
 def main():
     
-    parser = argparse.ArgumentParser("NN assignment for ANOSPP sequencing data")
+    parser = argparse.ArgumentParser('NN assignment for ANOSPP sequencing data')
     parser.add_argument('-a', '--haplotypes', help='Haplotypes tsv file', required=True)
     parser.add_argument('-m', '--manifest', help='Samples manifest tsv file', required=True)
     parser.add_argument('-s', '--stats', help='DADA2 stats tsv file', required=True)
-    parser.add_argument('-r', '--reference_version', help='Reference index version - currently a directory name.\
-         Default: nnv1', default='nnv1')
     parser.add_argument('-o', '--outdir', help='Output directory. Default: nn', default='nn')
-    parser.add_argument('--path_to_refversion', help='path to reference index version.\
-         Default: ref_databases', default='ref_databases')
-    parser.add_argument('--no_plotting', help='Do not generate plots. Default: False', \
+    parser.add_argument('-r', '--reference_version', 
+                        help='Reference index version - currently a directory name. Default: nnv1',
+                        default='nnv1')
+    parser.add_argument('-p', '--path_to_refversion',
+                        help='Path to reference index version. Default: ref_databases',
+                        default='ref_databases')
+    parser.add_argument('--no_plotting', help='Do not generate plots. Default: False',
+                        action='store_true',
                         default=False)
-    parser.add_argument('--allelism_normalisation', help='Normalisation method over multiple alleles. Options: \
-                         [n_alleles,reads_fraction]. Default: n_alleles', default='n_alleles')
-    parser.add_argument('--hap_read_count_threshold', help='minimum number of reads for supported haplotypes. \
-         Default: 10', default=10)
-    parser.add_argument('--hap_reads_fraction_threshold', help='minimum fraction of reads for supported haplotypes. \
-         Default: 0.1', default=0.1)
-    parser.add_argument('--medium_contamination_read_count_threshold', help='samples with fewer than this number \
-                        of reads get medium contamination risk. Default: 1000', default=1000)
-    parser.add_argument('--medium_contamination_multi_allelic_threshold', help='samples with more than this number \
-                        of multiallelic targets get medium contamination risk. Default: 0', default=0)
-    parser.add_argument('--high_contamination_multi_allelic_threshold', help='samples with more than this number \
-                        of multiallelic targets get high contamination risk. Default: 2', default=2)
-    parser.add_argument('--nn_assignment_threshold', help='required fraction for calling assignment. \
-                        Default: 0.8', default=0.8)
-    parser.add_argument('--n_error_snps', help='Maximum number of snps for a multi-allelic sequence to be \
-                        considered a sequencing or PCR error. Default: 2', default=2)
-    parser.add_argument('-k', '--kmer_length', help='Length of k-mers to use. Note that NNoVAE has been developed \
-                        and tested for k=8, so accuracy of results cannot be guaranteed with other values of k. \
-                        Default: k=8', default=8)
-    parser.add_argument('-v', '--verbose', 
-                        help='Include INFO level log messages', action='store_true')
+    parser.add_argument('--allelism_normalisation',
+                        help='Normalisation method over multiple alleles. Options: [n_alleles,reads_fraction]. '
+                        'Default: n_alleles',
+                        choices=['n_alleles', 'reads_fraction'],
+                        default='n_alleles')
+    parser.add_argument('--hap_read_count_threshold',
+                        help='Minimum number of reads for supported haplotypes.  Default: 10',
+                        default=10, type=int)
+    parser.add_argument('--hap_reads_fraction_threshold',
+                        help='Minimum fraction of reads for supported haplotypes. Default: 0.1',
+                        default=0.1, type=float)
+    parser.add_argument('--medium_contamination_read_count_threshold',
+                        help='Samples with fewer than this number of reads get medium contamination risk. Default: 1000',
+                        default=1000, type=int)
+    parser.add_argument('--medium_contamination_multi_allelic_threshold',
+                        help='Samples with more than this number of multiallelic targets get medium contamination risk. Default: 0',
+                        default=0, type=int)
+    parser.add_argument('--high_contamination_multi_allelic_threshold',
+                        help='Samples with more than this number of multiallelic targets get high contamination risk. Default: 2',
+                        default=2, type=int)
+    parser.add_argument('--very_high_contamination_multi_allelic_threshold',
+                        help='Samples with more than this number of multiallelic targets get very high contamination risk. Default: 4',
+                        default=4, type=int)
+    parser.add_argument('--nn_assignment_threshold',
+                        help='Required fraction for calling assignment. Default: 0.8',
+                        default=0.8, type=float)
+    parser.add_argument('--n_error_snps',
+                        help='Maximum number of snps for a multi-allelic sequence to be considered a sequencing or PCR error. Default: 2',
+                        default=2, type=int)
+    parser.add_argument('-k', '--kmer_length',
+                        help='Length of k-mers to use. Note that NNoVAE has been developed and tested for k=8, '
+                        'so accuracy of results cannot be guaranteed with other values of k. Default: k=8',
+                        default=8, type=int)
+    parser.add_argument('--plasm_assignment',
+                        help='Path to plasm_assignment.tsv file used for sample label colouring '
+                        'in nn plots. Default: None - colouring not applied',
+                        default=None)
+    parser.add_argument('--plasm_colors',
+                        help='Path to species_colours.csv from plasm reference directory '
+                        'used for sample label colouring in nn plots. '
+                        'Default: None - colouring not applied',
+                        default=None)
+    parser.add_argument('--legend_cutoff',
+                        help='Minimum observed NN assignment proportion '
+                        'for species label to be added to the legend '
+                        'Default: 0 - include all species in reference index',
+                        default=0, type=float)
+    parser.add_argument('--resume',
+                        help='Do not re-generate nn_dist_to_ref.tsv and nn_assignment.tsv '
+                        'if those are present in the output directory',
+                        action='store_true', default=False)
+    parser.add_argument('-v', '--verbose',
+                        help='Include INFO level log messages',
+                        action='store_true')
 
     args = parser.parse_args()
     args.outdir=args.outdir.rstrip('/')
+
     nn(args)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `anospp_analysis-0.2.1/anospp_analysis/prep.py` & `anospp_analysis-0.3.0/anospp_analysis/prep.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,58 +41,70 @@
     seqid, target, trimmed sequence
     '''
     logging.info('parsing deplexed sequences')
 
     deplex_dict = dict()
     # iterate over deplexed fasta files
     for fa in sorted(glob.glob(f'{deplex_dir}/ASV_*.fa')):
-        target = fa.split('/')[-1].split('.')[0].split('_')[1]
-        if target not in CUTADAPT_TARGETS:
-            logging.warning(f'Target {target} not recognised for {fa}, skipping')
-            continue
+        target = fa.split('/')[-1].split('.')[0].split('_', maxsplit=1)[1]
         # basic parser
         with open(fa) as f:
             for line in f:
                 line = line.strip()
                 if line.startswith('>'):
                     seqid = line[1:]
                 else:
                     deplex_dict[seqid] = {'target':target,'trimmed_sequence':line}
         # proper parser
         # for record in SeqIO.parse(fa, format='fasta'):
         #     deplex_dict[record.name] = {'target':target,'trimmed_sequence':str(record.seq)}
     deplex_df = pd.DataFrame(deplex_dict).T
     dup_seqid = deplex_df.index.duplicated()
     if dup_seqid.any():
-        raise ValueError(f'Duplicate seqids generated by dada2: {deplex_df.index[dup_seqid]}')
+        raise ValueError(f'duplicate seqids generated by dada2: {deplex_df.index[dup_seqid]}')
     return deplex_df
 
 def get_hap_df(dada_table, demult_dir):
 
     deplex_df = get_deplex_df(demult_dir)
 
     logging.info('combining dada output with deplexing info')
 
     dada_df = pd.read_csv(dada_table, sep='\t', index_col=0)
 
     dada_deplex_df = pd.merge(dada_df, deplex_df, left_index=True, right_index=True)
     dada_deplex_df.index.name = 'dada2_id'
     assert dada_deplex_df.shape[0] == dada_df.shape[0] == deplex_df.shape[0], \
-        'Lost some sequences in combining deplexing and original DADA2 data'
+        'lost some sequences in combining deplexing and original DADA2 data'
     
     hap_df = pd.melt(dada_deplex_df.reset_index(), 
-            id_vars=['dada2_id','sequence','target','trimmed_sequence'],
+            id_vars=['dada2_id', 'sequence', 'target', 'trimmed_sequence'],
             var_name='sample_id',
             value_name='reads')
-    hap_df = hap_df[hap_df.reads > 0].copy()
     hap_df['target'] = hap_df.target.astype(str)
+    if not hap_df['target'].isin(CUTADAPT_TARGETS).all():
+        logging.warning('non-ANOSPP targets detected in demultiplexing')
     hap_df.rename(columns={
         'sequence':'untrimmed_sequence',
         'trimmed_sequence':'consensus'
     }, inplace=True)
+    # collapse identical sequences
+    hap_df = hap_df.groupby(['sample_id', 'target', 'consensus'])['reads'].sum().reset_index()
+    # remove unsupported sequences
+    hap_df = hap_df.query('reads > 0').copy()
+
+    hap_df['total_reads'] = hap_df.groupby(by=['sample_id', 'target']) \
+        ['reads'].transform('sum')
+    
+    hap_df['reads_fraction'] = hap_df['reads'] / hap_df['total_reads']
+
+    hap_df['nalleles'] = hap_df.groupby(by=['sample_id', 'target']) \
+        ['consensus'].transform('nunique')
+
+    hap_df = seqid_generator(hap_df)
 
     return hap_df
 
 def prep_dada2(args):
 
     setup_logging(verbose=args.verbose)
     
@@ -102,23 +114,27 @@
 
     hap_df = get_hap_df(args.dada_table, args.work_dir)
 
     hap_df[[
         'sample_id',
         'target',
         'consensus',
-        'reads'
+        'reads',
+        'total_reads',
+        'reads_fraction',
+        'nalleles',
+        'seqid'
     ]].to_csv(args.out_haps, sep='\t', index=False)
 
     logging.info('ANOSPP data prep complete')
 
 def main():
     
     parser = argparse.ArgumentParser("Convert DADA2 output to ANOSPP haplotypes tsv")
-    parser.add_argument('-t', '--dada_table', help='DADA2 stats tsv file', required=True)
+    parser.add_argument('-t', '--dada_table', help='dada2 output table, in ampliseq pipeline it is called DADA2_table.tsv', required=True)
     parser.add_argument('-a', '--adapters', help='adapters fasta file for deplexing with cutadapt', required=True)
     parser.add_argument('-o', '--out_haps', help='output haplotypes tsv file. Default: haps.tsv', default='haps.tsv')
     parser.add_argument('-w', '--work_dir', help='working directory for intermediate files. Default: work',
                         default='work')
     parser.add_argument('-v', '--verbose', 
                         help='Include INFO level log messages', action='store_true')
```

### Comparing `anospp_analysis-0.2.1/anospp_analysis/test_functions_vae.py` & `anospp_analysis-0.3.0/anospp_analysis/test_functions_vae.py`

 * *Files identical despite different names*

### Comparing `anospp_analysis-0.2.1/anospp_analysis/util.py` & `anospp_analysis-0.3.0/anospp_analysis/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pandas as pd
 import numpy as np
 import logging
 
 MOSQ_TARGETS = [str(i) for i in range(62)]
-PLASM_TARGETS = ['P1','P2']
-TARGETS = MOSQ_TARGETS + PLASM_TARGETS
-CUTADAPT_TARGETS = TARGETS + ['unknown']
+PLASM_TARGETS = ['P1', 'P2']
+ANOSPP_TARGETS = MOSQ_TARGETS + PLASM_TARGETS
+CUTADAPT_TARGETS = ANOSPP_TARGETS + ['unknown']
 
 def setup_logging(verbose=False):
     try: 
         del logging.root.handlers[:]
     except:
         pass
     if verbose:
-        logging.basicConfig(level=logging.INFO, format='[%(levelname)s] %(message)s')
+        logging.basicConfig(level=logging.INFO, format='[%(levelname)s] [%(asctime)s] %(message)s')
     else:
-        logging.basicConfig(level=logging.WARNING, format='[%(levelname)s] %(message)s')
+        logging.basicConfig(level=logging.WARNING, format='[%(levelname)s] [%(asctime)s] %(message)s')
 
 def well_id_mapper():
     '''
     Yields mapping of tag_index 1,2...96 
     to well id A1,B1...H12.
     N.B. subsequent plates can be mapped using
     tag_index % 96, thus last well is inserted at 0
@@ -73,74 +73,102 @@
     # edge case
     lims_well_ids[0] = 'P24'
 
     return lims_well_ids
 
 def seqid_generator(hap_df):
     '''
-    assign identifyer to unique haplotypes
-    used in nn/construct_unique_kmer_table
+    assign identifiers to unique haplotypes
     '''
 
     seqids = dict()
     for tgt, group in hap_df.groupby('target'):
         for (i, cons) in enumerate(group['consensus'].unique()):
             seqids[tgt + cons] = '{}-{}'.format(tgt, i)
     hap_df['seqid'] = (hap_df.target + hap_df.consensus).replace(seqids)
 
     return hap_df
 
-def prep_hap(hap_fn):
+def human_format(num):
+    if num is None:
+        return ''
+    magnitude = 0
+    while abs(num) >= 1000:
+        magnitude += 1
+        num /= 1000.0
+    # 1 though 999
+    if magnitude == 0:
+        return '%.0f' % (num)
+    # 1.0k through 99.9k
+    elif num < 100:
+        return '%.1f%s' % (num, ['', 'K', 'M', 'G', 'T', 'P'][magnitude])
+    # 100k through 999k
+    else:
+        return '%.0f%s' % (num, ['', 'K', 'M', 'G', 'T', 'P'][magnitude])
+
+def well_ordering(well_series):
+
+    # well order for plotting - A1, B1, ...
+    well_sequence = []
+    for col in range(1,13):
+        for row in 'ABCDEFGH': 
+            well_sequence.append(f'{row}{col}')
+
+    return pd.Categorical(well_series, categories=well_sequence)
+
+def prep_hap(hap_fn, anospp=True):
     '''
     load haplotypes table
     '''
 
     logging.info(f'preparing haplotypes table from {hap_fn}')
 
-    hap_df = pd.read_csv(hap_fn, sep='\t')
+    hap_df = pd.read_csv(hap_fn, sep='\t', dtype={'target':'str'})
 
     # compatibility with old style haplotype column names
     hap_df.rename(columns=({
         's_Sample':'sample_id',
         'frac_reads':'reads_fraction'
         }), 
     inplace=True)
 
     for col in ('sample_id',
                 'target',
                 'consensus',
                 'reads'):
         assert col in hap_df.columns, f'hap column {col} not found'
 
-    if 'reads_log10' not in hap_df.columns:
-        hap_df['reads_log10'] = hap_df['reads'].apply(lambda x: np.log10(x))
-
+    # duplicates anospp_analysis.prep.get_hap_df
     if 'total_reads' not in hap_df.columns:
         hap_df['total_reads'] = hap_df.groupby(by=['sample_id', 'target']) \
             ['reads'].transform('sum')
 
     if 'reads_fraction' not in hap_df.columns:
         hap_df['reads_fraction'] = hap_df['reads'] / hap_df['total_reads']
 
+    if 'seqid' not in hap_df.columns:
+        hap_df = seqid_generator(hap_df)
+
     if 'nalleles' not in hap_df.columns:
         hap_df['nalleles'] = hap_df.groupby(by=['sample_id', 'target']) \
-            ['consensus'].transform('nunique')
+            ['seqid'].transform('nunique')
 
     hap_df['consensus'] = hap_df['consensus'].str.upper()
-        
-    hap_df = seqid_generator(hap_df)
-
-    hap_df['target'] = pd.Categorical(hap_df['target'], 
-                                    categories=CUTADAPT_TARGETS, 
-                                    ordered=True)
+    
+    if hap_df['target'].isin(CUTADAPT_TARGETS).all():
+        hap_df['target'] = pd.Categorical(hap_df['target'], 
+                                        categories=CUTADAPT_TARGETS, 
+                                        ordered=True)
+    else:
+        logging.warning('non-ANOSPP targets detected in haps, targets order might be unstable')
     
     hap_df.sort_values(by=[
         'sample_id',
         'target'
-    ], inplace=True)
+        ], inplace=True)
 
     return hap_df
 
 def prep_samples(samples_fn):
     '''
     load sample manifest used for anospp pipeline
     '''
@@ -154,18 +182,20 @@
             'Run':'run_id',
             'Lane':'lane_index',
             'Tag':'tag_index',
             'Replicate':'replicate_id'
             }), 
             inplace=True)
     elif samples_fn.endswith('tsv'):
-        logging.info(f'preparing sample manifest from new file {samples_fn}')
+        logging.info(f'preparing sample manifest from new style file {samples_fn}')
         samples_df = pd.read_csv(samples_fn, sep='\t', dtype='str')
         samples_df.rename(columns=({'derived_sample_id':'sample_id'}), inplace=True)
-        assert samples_df.irods_path.str.match('/seq/\d{5}/\d{5}_\d#\d+.cram').all()
+        assert samples_df.irods_path.str.match('/seq/\d{5}/\d{5}_\d#\d+.cram').all(), \
+            ('tsv sample manifest input requires irods_path column to be present '
+             'and match "/seq/12345/12345_1#123.cram"')
         samples_df['run_id'] = samples_df.irods_path.str.split('/').str.get(2)
         samples_df[['lane_index', 'tag_index']] = samples_df.irods_path \
             .str.split('/').str.get(3) \
             .str.split('_').str.get(1) \
             .str.split('.').str.get(0) \
             .str.split('#', expand=True)
     else:
@@ -184,84 +214,131 @@
     if 'plate_id' in samples_df.columns and 'well_id' in samples_df.columns:
         pass
     else:
         # sample_id as `{plate_id}_{well_id}-{sanger_sample_id}` 
         try:
             plate_well_ids = samples_df['sample_id'].str.rsplit('-', n = 1).str.get(0)
             samples_df[['plate_id', 'well_id']] = plate_well_ids.str.rsplit('_', n = 1, expand=True)
+            # do not allow for non-standard well IDs
             assert samples_df.well_id.isin(well_id_mapper().values()).all()
+            # do not allow for duplicate plate IDs - issues with plotting
+            assert (samples_df.plate_id.value_counts() <= 96).all()
+            logging.info('inferring plate_id and well_id from sample_id')
         except:
+            logging.info('inferring plate_id and well_id from tags')
             samples_df['plate_id'] = samples_df.apply(lambda r: f'p_{r.run_id}_{(r.tag_index - 1) // 96 + 1}',
                 axis=1)
             samples_df['well_id'] = (samples_df.tag_index % 96).replace(well_id_mapper())
     
     assert ~samples_df.plate_id.isna().any(), 'Could not infer plate_id for all samples'
     assert ~samples_df.well_id.isna().any(), 'Could not infer well_id for all samples'
     assert samples_df.well_id.isin(well_id_mapper().values()).all(), 'Found well_id outside A1...H12'
     # id_library_lims as `{lims_plate_id}:{lims_well_id}`
     if ('id_library_lims' in samples_df.columns and
         samples_df.id_library_lims.str.contains(':').all()):
-            samples_df[['lims_plate_id','lims_well_id']] = samples_df.id_library_lims.str.split(':', 
-                                                                                                n = 1, 
-                                                                                                expand=True)
+            logging.info('inferring lims_plate_id from id_library_lims')
+            samples_df[['lims_plate_id', 'lims_well_id']] = samples_df.id_library_lims.str.split(
+                ':', n = 1, expand=True
+                )
     else:
-        samples_df['lims_plate_id'] = samples_df.apply(lambda r: f'lp_{r.run_id}_{(r.tag_index - 1) // 384 + 1}',
-            axis=1)
+        logging.info('inferring lims_plate_id from tags')
+        samples_df['lims_plate_id'] = samples_df.apply(
+            lambda r: f'lp_{r.run_id}_{(r.tag_index - 1) // 384 + 1}',
+            axis=1
+            )
         samples_df['lims_well_id'] = (samples_df.tag_index % 384).replace(lims_well_id_mapper())
     assert ~samples_df.lims_plate_id.isna().any(), 'Could not infer plate_id for all samples'
     assert ~samples_df.lims_well_id.isna().any(), 'Could not infer well_id for all samples'
     assert samples_df.lims_well_id.isin(lims_well_id_mapper().values()).all(), 'Found well_id outside A1...H12'
+    
+    # sample_name - short sample id for plotting
+    # works if sanger_sample_id does not contain dashes
+    # and if sample ID is a concatenation of sample_name and sanger_sample_id
+    samples_df['sample_name'] = samples_df['sample_id'].str.rsplit('-', n=1).str.get(0)
+
+    # first run record assumed to be the run ID for plot titles
+    run_id = samples_df['run_id'].iloc[0]
 
-    return samples_df
+    return run_id, samples_df
 
 def prep_stats(stats_fn):
     '''
-    load DADA2 stats table
+    load DADA2 stats table from either DADA2_stats.tsv
+    or overall_summary.txt file of ampliseq pipeline
     
     For legacy stats table, summarise across targets
     '''
 
     logging.info(f'preparing DADA2 statistics from {stats_fn}')
 
     stats_df = pd.read_csv(stats_fn, sep='\t')
 
     stats_df.rename(columns={
         # compatibility with legacy format
         's_Sample':'sample_id',
+        'final':'dada2_postfilter_reads',
         # compatibility with new format 
         'sample':'sample_id',
-        'DADA2_input':'input'
+        # generic renaming
+        'DADA2_input':'dada2_input_reads',
+        'filtered':'dada2_filtered_reads',
+        'denoised':'dada2_denoised_reads',
+        'denoisedF':'dada2_denoisedf_reads',
+        'denoisedR':'dada2_denoisedr_reads',
+        'merged':'dada2_merged_reads',
+        'nonchim':'dada2_nonchim_reads'
         },
         inplace=True)
     
     for col in ('sample_id',
-                'input',
-                'filtered',
-                'denoisedF',
-                'denoisedR',
-                'merged',
-                'nonchim'):
+                'dada2_input_reads',
+                'dada2_filtered_reads',
+                'dada2_nonchim_reads'):
         assert col in stats_df.columns, f'stats column {col} not found'
 
     # denoising happens for F and R reads independently, we take minimum of those 
-    # as an estimate for retained read count
-    stats_df['denoised'] = stats_df[['denoisedF','denoisedR']].min(axis=1)
+    # as an estimate for denoised read count
+    if 'dada2_denoisedf_reads' in stats_df.columns and 'dada2_denoisedr_reads' in stats_df.columns:
+        logging.info('found DADA2 stats for paired end reads')
+        stats_df['dada2_denoised_reads'] = stats_df[[
+            'dada2_denoisedf_reads',
+            'dada2_denoisedr_reads'
+            ]].min(axis=1)
+        assert 'dada2_merged_reads' in stats_df.columns, f'stats column dada2_merged_reads not found'
+    else:
+        logging.info('found DADA2 stats for single end reads')
+        assert 'dada2_denoised_reads' in stats_df.columns, f'stats column dada2_denoised_reads not found'
+        # fake merged - same as denoised
+        stats_df['dada2_merged_reads'] = stats_df['dada2_denoised_reads']
     # legacy stats calculated separately for each target, merging
     if 'target' in stats_df.columns:
         logging.info(f'summarising legacy DADA2 statistics across targets')
         stats_df = stats_df.groupby('sample_id').sum(numeric_only=True).reset_index()
-    # add final read counts for comatibility with legacy pipeline
-    # that had a post-filtering step
-    if 'final' not in stats_df.columns:
-        stats_df['final'] = stats_df['nonchim']
-    # logscale read counts, placeholder value for zero - -1
-    for col in stats_df.columns.drop(['sample_id']):
-        stats_df[f'{col}_log10'] = stats_df[col].replace(0,0.1).apply(lambda x: np.log10(x))
-    # filter rate 
-    stats_df['filter_rate'] = stats_df['nonchim'] / stats_df['input']
+    # overall_summary.txt
+    if 'cutadapt_total_processed' in stats_df.columns:
+        stats_df.rename(columns={
+            'cutadapt_total_processed':'total_reads',
+            'cutadapt_passing_filters':'readthrough_pass_reads'
+        },
+        inplace=True)
+        # cutadapt stats recorded with thousands comma separator
+        for col in ('total_reads', 'readthrough_pass_reads'):
+            stats_df[col] = stats_df[col].astype(str).str.replace(',', '').astype(int)
+        stats_df.drop(
+            columns=['cutadapt_reverse_complemented', 'cutadapt_passing_filters_percent'],
+            inplace=True
+            )
+    # DADA2_stats
+    else:
+        logging.warning(
+            'DADA2_stats.tsv provided instead of overall_summary.txt, '
+            'cutadapt readthrough stats will be missing'
+            )
+        stats_df['total_reads'] = stats_df['dada2_input_reads']
+        stats_df['readthrough_pass_reads'] = stats_df['dada2_input_reads']
     
     return stats_df
 
 def combine_stats(stats_df, hap_df, samples_df):
     '''
     Combined per-sample statistics
     '''
@@ -271,32 +348,51 @@
     # some samples can be missing from stats due to DADA2 filtering
     if set(stats_df.sample_id) - set(samples_df.sample_id) != set():
         logging.error('sample_id mismatch between samples and stats, QC results will be compromised')
     # some samples can be missing from haps due to DADA2 & post-processing filtering
     elif set(hap_df.sample_id) - set(samples_df.sample_id) != set():
         logging.error('sample_id mismatch between haps and samples, QC results will be compromised')
 
-    comb_stats_df = pd.merge(stats_df, samples_df, on='sample_id', how='inner')
+    comb_stats_df = pd.merge(stats_df, samples_df, on='sample_id', how='outer')
+    for col in comb_stats_df.columns:
+        if col.endswith('_reads'):
+            comb_stats_df[col] = comb_stats_df[col].fillna(0).astype(int)
     comb_stats_df.set_index('sample_id', inplace=True)
-    comb_stats_df['targets_recovered'] = hap_df.groupby('sample_id') \
-        ['target'].nunique()
-    comb_stats_df['targets_recovered'] = comb_stats_df['targets_recovered'].fillna(0)
+    
+    comb_stats_df['target_reads'] = hap_df[hap_df.target != 'unknown'] \
+        .groupby('sample_id')['reads'].sum()
+    comb_stats_df['target_reads'] = comb_stats_df['target_reads'].fillna(0).astype(int)
+
+    comb_stats_df['overall_filter_rate'] = comb_stats_df['target_reads'] / comb_stats_df['total_reads']
+    comb_stats_df['overall_filter_rate'] = comb_stats_df['overall_filter_rate'].fillna(0)
+
+    comb_stats_df['unassigned_asvs'] = hap_df[hap_df.target == 'unknown'] \
+        .groupby('sample_id')['consensus'].nunique()
+    comb_stats_df['unassigned_asvs'] = comb_stats_df['unassigned_asvs'].fillna(0).astype(int)
+    
+    comb_stats_df['targets_recovered'] = hap_df[hap_df.target != 'unknown'] \
+        .groupby('sample_id')['target'].nunique()
+    comb_stats_df['targets_recovered'] = comb_stats_df['targets_recovered'].fillna(0).astype(int)
+    
     comb_stats_df['raw_mosq_targets_recovered'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
         .groupby('sample_id')['target'].nunique()
-    comb_stats_df['raw_mosq_targets_recovered'] = comb_stats_df['raw_mosq_targets_recovered'].fillna(0)
+    comb_stats_df['raw_mosq_targets_recovered'] = comb_stats_df['raw_mosq_targets_recovered'].fillna(0).astype(int)
+
+    comb_stats_df['raw_multiallelic_mosq_targets'] = (
+        hap_df[hap_df.target.isin(MOSQ_TARGETS)].groupby('sample_id')['target'].value_counts() > 2
+        ).groupby(level='sample_id').sum()
+    comb_stats_df['raw_multiallelic_mosq_targets'] = comb_stats_df['raw_multiallelic_mosq_targets'].fillna(0).astype(int)
+    
     comb_stats_df['raw_mosq_reads'] = hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
         .groupby('sample_id')['reads'].sum()
-    comb_stats_df['raw_mosq_reads'] = comb_stats_df['raw_mosq_reads'].fillna(0)
-    comb_stats_df['raw_mosq_log10_reads'] = comb_stats_df['raw_mosq_reads'] \
-        .replace(0,0.1).apply(lambda x: np.log10(x))
+    comb_stats_df['raw_mosq_reads'] = comb_stats_df['raw_mosq_reads'].fillna(0).astype(int)
+    
     for pt in PLASM_TARGETS:
-        comb_stats_df[f'{pt}_reads'] = hap_df[hap_df.target == pt] \
+        ptl = pt.lower()
+        comb_stats_df[f'{ptl}_reads'] = hap_df[hap_df.target == pt] \
             .groupby('sample_id')['reads'].sum()
-        comb_stats_df[f'{pt}_reads'] = comb_stats_df[f'{pt}_reads'].fillna(0)
-        comb_stats_df[f'{pt}_log10_reads'] = comb_stats_df[f'{pt}_reads'] \
-            .replace(0,0.1).apply(lambda x: np.log10(x))
-    comb_stats_df['raw_multiallelic_mosq_targets'] = (hap_df[hap_df.target.isin(MOSQ_TARGETS)] \
-        .groupby('sample_id')['target'].value_counts() > 2).groupby(level='sample_id').sum()
-    comb_stats_df['raw_multiallelic_mosq_targets'] = comb_stats_df['raw_multiallelic_mosq_targets'].fillna(0)
+        comb_stats_df[f'{ptl}_reads'] = comb_stats_df[f'{ptl}_reads'].fillna(0).astype(int)
+    
     comb_stats_df.reset_index(inplace=True)
+    comb_stats_df.sort_values(by='tag_index', inplace=True)
         
     return comb_stats_df
```

### Comparing `anospp_analysis-0.2.1/anospp_analysis/vae.py` & `anospp_analysis-0.3.0/anospp_analysis/vae.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
-from collections import OrderedDict
 import os
 import argparse
 import keras
 from scipy.spatial import ConvexHull, Delaunay
 
-from .util import *
-from .nn import parse_seqids_series, construct_unique_kmer_table
+from anospp_analysis.util import *
+from anospp_analysis.nn import parse_seqids_series, construct_unique_kmer_table
 
 #Variables
 K = 8
 LATENTDIM = 3
 SEED = 374173
 WIDTH = 128
 DEPTH = 6
@@ -23,72 +22,75 @@
     Read in standardised reference index files from database (currently directory)
     '''
 
     logging.info(f'importing reference index {reference_version}')
 
     reference_path = f'{path_to_refversion}/{reference_version}/'
 
-    assert os.path.isdir(reference_path), f'reference version {reference_version} does not \
-        exist at {reference_path}'
+    assert os.path.isdir(reference_path), \
+        f'reference version {reference_version} does not exist at {reference_path}'
 
-    assert os.path.isfile(f'{reference_path}/selection_criteria.txt'), f'reference version \
-        {reference_version} at {reference_path} does not contain required \
-        selection_criteria.txt file'
+    assert os.path.isfile(f'{reference_path}/selection_criteria.txt'), \
+        f'reference version {reference_version} at {reference_path} does not contain required selection_criteria.txt file'
     selection_criteria_file = f'{reference_path}/selection_criteria.txt'
 
-    assert os.path.isfile(f'{reference_path}/_weights.hdf5'), f'reference version \
-        {reference_version} at {reference_path} does not contain required \
-        _weights.hdf5 file'
+    assert os.path.isfile(f'{reference_path}/_weights.hdf5'), \
+        f'reference version {reference_version} at {reference_path} does not contain required _weights.hdf5 file'
     vae_weights_file = f'{reference_path}/_weights.hdf5'
 
-    assert os.path.isfile(f'{reference_path}/convex_hulls.tsv'), f'reference version \
-        {reference_version} at {reference_path} does not contain required \
-        convex_hulls.tsv file'
+    assert os.path.isfile(f'{reference_path}/convex_hulls.tsv'), \
+        f'reference version {reference_version} at {reference_path} does not contain required convex_hulls.tsv file'
     convex_hulls_df = pd.read_csv(f'{reference_path}/convex_hulls.tsv', sep='\t')
 
     if not os.path.isfile(f'{reference_path}/colors.tsv'):
-            logging.warning('No colors defined for plotting.')
-            colorsdict = dict()
+        logging.warning('No colors defined for plotting.')
+        colorsdict = dict()
     else:
         colors = pd.read_csv(f'{reference_path}/colors.tsv',sep='\t', index_col=0)
         colorsdict = dict(colors.color)
 
     if not os.path.isfile(f'{reference_path}/latent_coordinates.tsv'):
-            logging.warning('No reference coordinates defined for plotting.')
-            ref_coord = pd.DataFrame()
+        logging.warning('No reference coordinates defined for plotting.')
+        ref_coord = pd.DataFrame()
     else:
         ref_coord = pd.read_csv(f'{reference_path}/latent_coordinates.tsv',sep='\t')
 
     if os.path.isfile(f'{reference_path}/version.txt'):
         with open(f'{reference_path}/version.txt', 'r') as fn:
             for line in fn:
                 version_name = line.strip()
     else:
-        logging.warning(f'No version.txt file present for reference version {reference_version} \
-                        at {reference_path}')
+        logging.warning(f'No version.txt file present for reference version {reference_version} at {reference_path}')
         version_name = 'unknown'
         
-    return (selection_criteria_file, vae_weights_file, convex_hulls_df, colorsdict, \
-        ref_coord, version_name)
+    return (selection_criteria_file, vae_weights_file, convex_hulls_df, colorsdict, ref_coord, version_name)
 
-def read_selection_criteria(selection_criteria_file, comb_stats_df, hap_df):
+# def read_selection_criteria(selection_criteria_file, nn_stats_df, nn_hap_df):
     
-    level, sgp, n_targets = open(selection_criteria_file).read().split('\t')
-    return select_samples(comb_stats_df, hap_df, level, sgp, int(n_targets))
+#     level, sgp, n_targets = open(selection_criteria_file).read().split('\t')
+#     return select_samples(nn_stats_df, nn_hap_df, level, sgp, int(n_targets))
 
-def select_samples(comb_stats_df, hap_df, level, sgp, n_targets):
+def select_samples(selection_criteria_file, nn_stats_df, nn_hap_df):
     '''
     Select the samples meeting the criteria for VAE assignment
     Based on NN assignment and number of targets
     '''
     #identify samples meeting selection criteria
-    vae_samples = comb_stats_df.loc[(comb_stats_df[f'res_{level}'] == sgp) & \
-                        (comb_stats_df['mosq_targets_recovered'] >= n_targets), 'sample_id']
+    selection_criteria = pd.read_csv(selection_criteria_file, sep='\t')
+    vae_samples = []
+    for _, r in selection_criteria.iterrows():
+        crit_vae_samples = nn_stats_df.loc[
+            (nn_stats_df[f'nn_{r.level}'] == r.sgp) & (nn_stats_df['mosq_targets_recovered'] >= r.n_targets), 
+            'sample_id'
+            ]
+        vae_samples.append(crit_vae_samples)
+    vae_samples = pd.concat(vae_samples)
+    
     #subset haplotype df
-    vae_hap_df = hap_df.query('sample_id in @vae_samples')
+    vae_hap_df = nn_hap_df.query('sample_id in @vae_samples')
     
     logging.info(f'selected {len(vae_samples)} samples to be run through VAE')
 
     return vae_samples, vae_hap_df
 
 def prep_sample_kmer_table(kmers_unique_seqs, parsed_seqids):
     '''
@@ -123,55 +125,63 @@
     logging.info('generating k-mer tables for selected samples')
 
     #set up k-mer table
     kmers_samples = np.zeros((len(vae_samples), 4**k))
 
     #fill in table for samples
     for n, sample in enumerate(vae_samples):
-        parsed_seqids = parse_seqids_series(vae_hap_df.loc[vae_hap_df.sample_id == sample, 
-                                                           'seqid'])
+        parsed_seqids = parse_seqids_series(
+            vae_hap_df.loc[vae_hap_df.sample_id == sample, 'seqid']
+            )
         kmers_samples[n,:] = prep_sample_kmer_table(kmers_unique_seqs, parsed_seqids)
 
     return(kmers_samples)
 
 def latent_space_sampling(args):
     
     #Add noise to encoder output
     z_mean, z_log_var = args
-    epsilon = keras.backend.random_normal(shape=(keras.backend.shape(z_mean)[0], LATENTDIM),
-                                          mean=0, stddev=1., seed=SEED)
+    epsilon = keras.backend.random_normal(
+        shape=(keras.backend.shape(z_mean)[0], LATENTDIM),
+        mean=0, 
+        stddev=1., 
+        seed=SEED
+        )
     
     return z_mean + keras.backend.exp(z_log_var) * epsilon
 
 def define_vae_input(k):
     input_seq = keras.Input(shape=(4**k,))
 
     return input_seq
 
 def define_encoder(k):
     input_seq = define_vae_input(k)
     x = keras.layers.Dense(WIDTH, activation = 'elu')(input_seq)
-    for i in range(DEPTH-1):
+    for i in range(DEPTH - 1):
         x = keras.layers.Dense(WIDTH, activation = 'elu')(x)
     z_mean = keras.layers.Dense(LATENTDIM)(x)
     z_log_var = keras.layers.Dense(LATENTDIM)(x)
-    z = keras.layers.Lambda(latent_space_sampling, output_shape=(LATENTDIM,), \
-                            name = 'z')([z_mean, z_log_var])
-    encoder = keras.models.Model(input_seq, [z_mean,z_log_var,z], name = 'encoder')
+    z = keras.layers.Lambda(
+        latent_space_sampling, 
+        output_shape=(LATENTDIM,),
+        name = 'z'
+        )([z_mean, z_log_var])
+    encoder = keras.models.Model(input_seq, [z_mean, z_log_var, z], name = 'encoder')
 
     return encoder
 
 def define_decoder(k):
     #Check whether you need the layer part here
     decoder_input = keras.layers.Input(shape=(LATENTDIM,), name='ls_sampling')
-    x = keras.layers.Dense(WIDTH, activation = "linear")(decoder_input)
-    for i in range(DEPTH-1):
-        x = keras.layers.Dense(WIDTH, activation = "elu")(x)
-    output = keras.layers.Dense(4**k, activation = "softplus")(x)
-    decoder=keras.models.Model(decoder_input, output, name = 'decoder')
+    x = keras.layers.Dense(WIDTH, activation='linear')(decoder_input)
+    for i in range(DEPTH - 1):
+        x = keras.layers.Dense(WIDTH, activation='elu')(x)
+    output = keras.layers.Dense(4**k, activation='softplus')(x)
+    decoder = keras.models.Model(decoder_input, output, name='decoder')
 
     return decoder
 
 def define_vae(k):
     input_seq = define_vae_input(k)
     encoder = define_encoder(k)
     decoder = define_decoder(k)
@@ -187,31 +197,35 @@
     '''
 
     vae, encoder = define_vae(k)
 
     vae.load_weights(vae_weights_file)
     predicted_latent_pos = encoder.predict(kmer_table)
 
-    predicted_latent_pos_df = pd.DataFrame(index=vae_samples, columns=['mean1', 'mean2', 'mean3',\
-                                                                       'sd1', 'sd2', 'sd3'])
+    predicted_latent_pos_df = pd.DataFrame(
+        index=vae_samples, 
+        columns=['mean1', 'mean2', 'mean3', 'sd1', 'sd2', 'sd3']
+        )
     for i in range(3):
-        predicted_latent_pos_df[f'mean{i+1}'] = predicted_latent_pos[0][:,i]
-        predicted_latent_pos_df[f'sd{i+1}'] = predicted_latent_pos[1][:,i]
+        predicted_latent_pos_df[f'mean{i + 1}'] = predicted_latent_pos[0][:,i]
+        predicted_latent_pos_df[f'sd{i + 1}'] = predicted_latent_pos[1][:,i]
 
     return predicted_latent_pos_df
 
 def generate_convex_hulls(convex_hulls_df):
     '''
     Read in pre-computed points for convex hulls for each species
     '''
     logging.info('setting up convex hulls from reference database')
     hull_dict = dict()
     for species in convex_hulls_df.species.unique():
-        pos = convex_hulls_df.loc[convex_hulls_df.species==species, ['mean1', 'mean2', \
-                                                                     'mean3']].values
+        pos = convex_hulls_df.loc[
+            convex_hulls_df.species==species, 
+            ['mean1', 'mean2', 'mean3']
+            ].values
         hull = ConvexHull(pos)
         hull_dict[species] = (pos, hull)
 
     return hull_dict
 
 def check_half_space(p, n, o):
     '''
@@ -231,33 +245,33 @@
     centered on a
     oriented s.t. positive points into the simplex
     '''
     #the normal vector of the plane of the simplex
     #centered on a
     z = np.cross(b - a, c - a)
     #normalised
-    u = z/np.sqrt(np.dot(z, z))
+    u = z / np.sqrt(np.dot(z, z))
     #the edge ab normalised and centered on a
-    e = (b - a)/np.sqrt(np.dot(b - a, b - a))
+    e = (b - a) / np.sqrt(np.dot(b - a, b - a))
     #the unit normal of plane C
     n = np.cross(u, e)
     
     return n, a
 
 def check_edge_projection(p, v, w):
     '''
     check whether p lies above the edge vw
     '''
     #let vw be the normal vector defining plane U
     #through v
     e = w - v
     #length of vw
-    le = np.sqrt(np.dot(e,e))
+    le = np.sqrt(np.dot(e, e))
     #unit vector along the edge, centered on v
-    n = e/le
+    n = e / le
     #project p along the edge vw
     q = np.dot(p - v, n)
     
     return q, le
 
 def check_edge_partition(p, vertices):
     '''
@@ -266,18 +280,18 @@
     or one of the vertices
     '''
     v, w = vertices
     #get lenght of projection q of p along the edge
     #and the lenght l of the edge
     q, l = check_edge_projection(p, v, w)
     
-    if q<0:
+    if q < 0:
         #vertex v is closest
         return compute_distance_to_vertex(p, v)
-    elif q>l:
+    elif q > l:
         #vertex w is closest
         return compute_distance_to_vertex(p, w)
     else:
         #edge vw is closest
         return compute_distance_to_edge(p, v, w)
 
 def check_vertex_partition(p, v, verts):
@@ -306,26 +320,26 @@
             return compute_distance_to_vertex(p, w2)
         else:
             #edge vw2 is closest
             return compute_distance_to_edge(p, v, w2)
     else:
         #vertex v is closest
         return compute_distance_to_vertex(p, v)
-   
+
 def compute_distance_to_plane(p, vertices):
     '''
     compute distance point p to the plane defined 
     by the vertices of the simplex
     '''
     a, b, c = vertices
     #find a vector perpendicular to the simplex
     #centered on a
-    z = np.cross(b-a, c-a)
+    z = np.cross(b - a, c - a)
     #unit vector perpendicular to the plane
-    u = z/np.sqrt(np.dot(z, z))
+    u = z / np.sqrt(np.dot(z, z))
     #distance of p to the plane
     h = np.abs(np.dot(p - a, u))
     
     return h
 
 def compute_distance_to_vertex(p, v):
     '''
@@ -339,34 +353,34 @@
     '''
     compute the distance of p to the edge vw
     '''
     #let vw be the normal vector defining plane U
     #through v
     e = w - v
     #let n be unit vector along the edge
-    n = e/np.sqrt(np.dot(e,e))
+    n = e / np.sqrt(np.dot(e, e))
     #let q be the projection of p along the edge vw
-    q = np.dot(p - v, n)*n
+    q = np.dot(p - v, n) * n
     #distance is the length of the difference between p and q
     d = np.sqrt(np.dot(p - v - q, p - v - q))
     
     return d
 
 def compute_distance_to_simplex(p, vertices):
     '''
     Compute the 3d distance of point p to the triangle
     defined by the vertices
     '''
     a, b, c = vertices
     
     #get normal vectors to the planes containing the 
     #edges of the triangles and perpendicular to the simplex
-    Cn, Co = find_normal_edge_simplex(a,b,c)
-    Bn, Bo = find_normal_edge_simplex(c,a,b)
-    An, Ao = find_normal_edge_simplex(b,c,a)
+    Cn, Co = find_normal_edge_simplex(a, b, c)
+    Bn, Bo = find_normal_edge_simplex(c, a, b)
+    An, Ao = find_normal_edge_simplex(b, c, a)
     
     #for each of the edge planes, check whether p lies
     #in the same halfplane of the simplex
     Cs = check_half_space(p, Cn, Co)
     Bs = check_half_space(p, Bn, Bo)
     As = check_half_space(p, An, Ao)
     
@@ -378,318 +392,343 @@
     elif np.sum(partition) == 2:
         #p lies in a part bordering an edge
         return check_edge_partition(p, vertices[partition])
     elif np.sum(partition) == 1:
         #p lies in a part bordering a vertex
         return check_vertex_partition(p, vertices[partition][0], vertices[~partition])
     else:
-        logging.error("Something thought to be impossible happened in the convex hull computation - \
-        tell Marilou to retake her linear algebra exam")
+        logging.error(
+            'Something thought to be impossible happened in the convex hull computation - '
+            'tell Marilou to retake her linear algebra exam'
+            )
 
 def compute_distance_to_hull(hull, positions):
     '''
     compute the distance of all given positions
     to the given convex hull
     in 3d
     '''
     #array to store distances to all simplices
     dists = np.zeros((positions.shape[0], hull.simplices.shape[0]))
     for i, s in enumerate(hull.simplices):
         #compute distance to each simplex in turn
-        dists[:,i] = np.array([compute_distance_to_simplex(p, hull.points[s]) for p in positions])
+        dists[:, i] = np.array([compute_distance_to_simplex(p, hull.points[s]) for p in positions])
     #get the distance to the closest simplex for each point
     distances = dists.min(axis=1)
 
     return distances
 
 def check_is_in_hull(hull_pos, positions):
     '''
     Check whether a set of positions lies inside the specified hull
     '''
     if not isinstance(hull_pos,Delaunay):
         hull = Delaunay(hull_pos)
 
-    in_hull = hull.find_simplex(positions)>=0
+    in_hull = hull.find_simplex(positions) >= 0
 
     return in_hull
 
 def get_unassigned_samples(latent_positions_df):
-    unassigned = latent_positions_df.loc[latent_positions_df.VAE_species.isnull()].index
+    unassigned = latent_positions_df.loc[latent_positions_df.vae_species_call.isnull()].index
     n_unassigned = len(unassigned)
     return unassigned, n_unassigned
 
 def generate_hull_dist_df(hull_dict, latent_positions_df, unassigned):
 
     dist_df = pd.DataFrame(index=unassigned)
-    positions = latent_positions_df.loc[unassigned,['mean1','mean2','mean3']].values
+    positions = latent_positions_df.loc[unassigned ,['mean1', 'mean2', 'mean3']].values
     for species in hull_dict.keys():
         dist_df[species] = compute_distance_to_hull(hull_dict[species][1], positions)
     return dist_df 
 
 def get_closest_hulls(hull_dict, latent_positions_df, unassigned):
 
     dist_df = generate_hull_dist_df(hull_dict, latent_positions_df, unassigned)
     summary_dist_df = pd.DataFrame(index=dist_df.index)
     summary_dist_df['dist1'] = dist_df.min(axis=1)
     summary_dist_df['species1'] = dist_df.idxmin(axis=1)
-    summary_dist_df['dist2'] = dist_df.apply(lambda x: x.sort_values()[1], axis=1)
+    summary_dist_df['dist2'] = dist_df.apply(lambda x: x.sort_values().iloc[1], axis=1)
     summary_dist_df['species2'] = dist_df.apply(lambda x: x.sort_values().index[1], axis=1)
     return summary_dist_df, dist_df
 
 def assign_gam_col_band(latent_positions_df, summary_dist_df):
     #Determine which samples are in gamcol band
-    gamcol_band = summary_dist_df.loc[(summary_dist_df.species1.isin(['Anopheles_gambiae', \
-                            'Anopheles_coluzzii'])) & (summary_dist_df.species2.isin([\
-                            'Anopheles_gambiae', 'Anopheles_coluzzii'])) & \
-                            (summary_dist_df.dist2<14)].copy()
+    gamcol_band = summary_dist_df.loc[
+        (summary_dist_df.species1.isin(['Anopheles_gambiae', 'Anopheles_coluzzii'])) & \
+        (summary_dist_df.species2.isin(['Anopheles_gambiae', 'Anopheles_coluzzii'])) & \
+        (summary_dist_df.dist2 < 14)
+        ].copy()
     #Make assignments for the samples in gamcol band
-    if gamcol_band.shape[0]>0:
-        gamcol_dict = dict(gamcol_band.apply(lambda row: 'Uncertain_'+row.species1.split('_')[1]+\
-                                             '_'+row.species2.split('_')[1], axis=1))
-        latent_positions_df.loc[gamcol_band.index, 'VAE_species'] = latent_positions_df.loc[\
-            gamcol_band.index].index.map(gamcol_dict)
+    if gamcol_band.shape[0] > 0:
+        gamcol_dict = dict(gamcol_band.apply(
+            lambda row: 'Uncertain_' + row.species1.split('_')[1] + '_' + row.species2.split('_')[1],
+            axis=1))
+        latent_positions_df.loc[gamcol_band.index, 'vae_species_call'] = latent_positions_df.loc[\
+            gamcol_band.index
+            ].index.map(gamcol_dict)
     return latent_positions_df, gamcol_band.shape[0]
 
 def assign_to_closest_hull(latent_positions_df, summary_dist_df, unassigned):
     '''
     Assign samples that are much closer to one hull than to all others to that hull
     Currently defined as a distance 7 times smaller than all others
     '''
-    fuzzy_hulls = summary_dist_df.loc[(DISTRATIO*summary_dist_df.dist1 < \
-        summary_dist_df.dist2)&(summary_dist_df.index.isin(unassigned))].copy()
-    if fuzzy_hulls.shape[0]>0:
+    fuzzy_hulls = summary_dist_df.loc[
+        (DISTRATIO*summary_dist_df.dist1 < summary_dist_df.dist2) & \
+        summary_dist_df.index.isin(unassigned)
+        ].copy()
+    if fuzzy_hulls.shape[0] > 0:
         fuzzy_hulls_dict = dict(fuzzy_hulls.species1)
-        latent_positions_df.loc[unassigned, 'VAE_species'] = latent_positions_df.loc[\
-            unassigned].index.map(fuzzy_hulls_dict)
+        latent_positions_df.loc[unassigned, 'vae_species_call'] = latent_positions_df.loc[
+            unassigned
+            ].index.map(fuzzy_hulls_dict)
     return latent_positions_df, fuzzy_hulls.shape[0]
 
 def assign_to_multiple_hulls(latent_positions_df, dist_df, unassigned):
     '''
     Assign samples in between hulls to multiple hulls in order of closeness
     '''
     between_hulls = dist_df.loc[dist_df.index.isin(unassigned)].copy()
-    between_hulls_dict = dict(between_hulls.apply(lambda row: 'Uncertain_'+'_'.join(\
-        label.split('_')[1] for label in row.sort_values().index[row.sort_values()<\
-                                                            DISTRATIO*row.min()]), axis=1))
-    latent_positions_df.loc[unassigned, 'VAE_species'] = latent_positions_df.loc[\
-        unassigned].index.map(between_hulls_dict)
+    between_hulls_dict = dict(between_hulls.apply(
+        lambda row: 'Uncertain_'+'_'.join(
+            label.split('_')[1] for label in row.sort_values().index[
+                row.sort_values() < DISTRATIO * row.min()
+                ]
+            ),
+        axis=1))
+    latent_positions_df.loc[unassigned, 'vae_species_call'] = latent_positions_df.loc[
+        unassigned
+        ].index.map(between_hulls_dict)
     return latent_positions_df, between_hulls.shape[0]
 
 def perform_convex_hull_assignments(hull_dict, latent_positions_df):
     '''
     Perform convex hull assignments based on latent space positions
     '''
     logging.info('performing convex hull assignment')
     positions = latent_positions_df[['mean1', 'mean2', 'mean3']].values
     
     #first check which samples fall inside convex hulls
     for label in hull_dict.keys():
         is_in_hull = check_is_in_hull(hull_dict[label][0], positions)
-        latent_positions_df.loc[is_in_hull, 'VAE_species'] = label
+        latent_positions_df.loc[is_in_hull, 'vae_species_call'] = label
     
     #Record unassigned samples 
     unassigned, n_unassigned = get_unassigned_samples(latent_positions_df)
-    logging.info(f'{latent_positions_df.shape[0] - n_unassigned} samples fall inside convex hulls; \
-{n_unassigned} samples still to be assigned')
+    logging.info(
+        f'{latent_positions_df.shape[0] - n_unassigned} samples fall inside convex hulls; '
+        f'{n_unassigned} samples still to be assigned'
+        )
     
     #for the unassigned samples, get distances to two closest hulls
     if n_unassigned > 0:
         summary_dist_df, dist_df = get_closest_hulls(hull_dict, latent_positions_df, unassigned)
-        latent_positions_df, n_newly_assigned = assign_gam_col_band(latent_positions_df, \
-                                                                    summary_dist_df)
+        latent_positions_df, n_newly_assigned = assign_gam_col_band(
+            latent_positions_df, 
+            summary_dist_df
+            )
         unassigned, n_unassigned = get_unassigned_samples(latent_positions_df)
-        logging.info(f'{n_newly_assigned} samples assigned to uncertain_gambiae_coluzzii or \
-uncertain_coluzzii_gambiae; {n_unassigned} samples still to be assigned')
+        logging.info(
+            f'{n_newly_assigned} samples assigned to uncertain_gambiae_coluzzii or uncertain_coluzzii_gambiae; '
+            f'{n_unassigned} samples still to be assigned'
+            )
     if n_unassigned > 0:
-        latent_positions_df, n_newly_assigned = assign_to_closest_hull(latent_positions_df, \
-                                                                summary_dist_df, unassigned)
+        latent_positions_df, n_newly_assigned = assign_to_closest_hull(
+            latent_positions_df, 
+            summary_dist_df, 
+            unassigned
+            )
         unassigned, n_unassigned = get_unassigned_samples(latent_positions_df)
-        logging.info(f'{n_newly_assigned} additional samples assigned to a single species; \
-{n_unassigned} samples still to be assigned')
+        logging.info(
+            f'{n_newly_assigned} additional samples assigned to a single species; '
+            f'{n_unassigned} samples still to be assigned')
     if n_unassigned > 0:
-        latent_positions_df, n_newly_assigned = assign_to_multiple_hulls(latent_positions_df,\
-                                                                        dist_df, unassigned)
+        latent_positions_df, n_newly_assigned = assign_to_multiple_hulls(
+            latent_positions_df,
+            dist_df, 
+            unassigned
+            )
         logging.info(f'{n_newly_assigned} samples assigned to multiple hulls.')
     logging.info(f'finished assigning {latent_positions_df.shape[0]} samples')
 
     return latent_positions_df
 
-def plot_VAE_assignments(ch_assignments, ref_coordinates, colordict):
+def plot_vae_assignments(ch_assignments, ref_coordinates, colordict, run_id):
 
     logging.info('generating VAE plots')
     #get assignment categories
     single, double, multi = [], [], []
-    species_dict = dict(ch_assignments.groupby('VAE_species').size())
+    species_dict = dict(ch_assignments.groupby('vae_species_call').size())
     for key in species_dict.keys():
         #for single species assignment
         if key.startswith('Anopheles_'):
             single.append(key)
         #for uncertain between two species
         elif len(key.split('_')) == 3:
             double.append(key)
         #for uncertain between more than two species
         else:
             multi.append(key)
 
-    fig, ax = plt.subplots(figsize=(8,8))
+    fig, ax = plt.subplots(figsize=(8, 8), constrained_layout=True)
+
+    fig.suptitle(f'An. gambiae complex VAE assignment for run {run_id}')
 
     #Plot reference dataset
-    ref_coordinates['color'] = ref_coordinates.VAE_species.map(colordict)
-    ax.scatter(ref_coordinates.mean1, ref_coordinates.mean3, \
-               c=ref_coordinates.color.values, alpha=.6, zorder=1)
+    ref_coordinates['color'] = ref_coordinates.vae_species_call.map(colordict)
+    ax.scatter(
+        ref_coordinates.mean1, 
+        ref_coordinates.mean3, 
+        c=ref_coordinates.color.values, 
+        alpha=.6, 
+        zorder=1
+        )
     
-    if len(single)>0:
-        #Plot samples assigned to single species
+    #Plot samples assigned to single species
+    if len(single) > 0:
         for species in single:
-            sub = ch_assignments.query('VAE_species == @species')
-            if species=='Anopheles_bwambae-fontenillei':
-                label= f'Anopheles_bwambae-\nfontenillei: {species_dict[species]}'
+            sub = ch_assignments.query('vae_species_call == @species')
+            if species == 'Anopheles_bwambae-fontenillei':
+                label = f'Anopheles_bwambae-\nfontenillei: {species_dict[species]}'
             else:
                 label = f'{species}: {species_dict[species]}'
-            ax.scatter(sub.mean1, sub.mean3, color=colordict[species], marker='^', \
-                   edgecolor='k', label=label, zorder=2)
+            ax.scatter(
+                sub.mean1, 
+                sub.mean3, 
+                color=colordict[species], 
+                marker='^', 
+                edgecolor='k', 
+                label=label, 
+                zorder=2
+                )
 
+    #Plot samples assigned to two species
     if len(double)>0:    
-        #Plot samples assigned to two species
         for species in double:
-            sub = ch_assignments.query('VAE_species == @species')
+            sub = ch_assignments.query('vae_species_call == @species')
             _, sp1, sp2 = species.split('_')
             #multiple lines on the legend
             if sp1 == 'bwambae-fontenillei':
                 label = f'Uncertain_bwambae-\nfontenillei_{sp2}: {species_dict[species]}'
             else:
                 label = f'Uncertain_{sp1}_\n{sp2}: {species_dict[species]}'
-            ax.scatter(sub.mean1, sub.mean3, marker='s', edgecolor=colordict[f'Anopheles_{sp1}'], \
-                   facecolor=colordict[f'Anopheles_{sp2}'], linewidth=1.5, zorder=2, label=label)
+            ax.scatter(
+                sub.mean1, 
+                sub.mean3, 
+                marker='s', 
+                edgecolor=colordict[f'Anopheles_{sp1}'], 
+                facecolor=colordict[f'Anopheles_{sp2}'], 
+                linewidth=1.5, 
+                zorder=2, 
+                label=label
+                )
 
+    #Plot remaining samples
     if len(multi)>0:    
-        #Plot remaining samples:
-        sub = ch_assignments.query('VAE_species in @multi')
-        ax.scatter(sub.mean1, sub.mean3, color='k', marker='s', zorder=3, \
-                   label=f'other: {sub.shape[0]}')
+        sub = ch_assignments.query('vae_species_call in @multi')
+        ax.scatter(
+            sub.mean1, 
+            sub.mean3,
+            color='k', 
+            marker='s', 
+            zorder=3, 
+            label=f'other: {sub.shape[0]}'
+            )
 
     ax.set_xlabel('LS1')
     ax.set_ylabel('LS3')
         
     legend = ax.legend(loc='lower right', prop={'size': 9})
 
     return fig, ax
 
-def finalise_assignments(comb_stats_df, ch_assignments_df):
-
-    logging.info('finalising mosquito species assignments')
-
-    #Add VAE columns
-    m1dict = dict(ch_assignments_df.mean1)
-    m2dict = dict(ch_assignments_df.mean2)
-    m3dict = dict(ch_assignments_df.mean3)
-    vaespeciesdict = dict(ch_assignments_df.VAE_species)
-
-    comb_stats_df['LS1'] = comb_stats_df.sample_id.map(m1dict)
-    comb_stats_df['LS2'] = comb_stats_df.sample_id.map(m2dict)
-    comb_stats_df['LS3'] = comb_stats_df.sample_id.map(m3dict)
-    comb_stats_df['VAE_species'] = comb_stats_df.sample_id.map(vaespeciesdict)
-
-    #Get final species call
-    #Samples assigned by VAE
-    comb_stats_df['species_call'] = comb_stats_df.VAE_species
-    comb_stats_df.loc[~comb_stats_df.species_call.isnull(), 'call_method'] = 'VAE'
-    
-    #Samples assigned by NN
-    for level in ['fine', 'int', 'coarse']:
-        leveldict = dict(zip(comb_stats_df.sample_id, comb_stats_df[f'res_{level}']))
-        comb_stats_df.loc[(comb_stats_df.species_call.isnull()) & \
-            (~comb_stats_df[f'res_{level}'].isnull()), 'call_method'] = f'NN_{level}'
-        comb_stats_df.loc[comb_stats_df.call_method == f'NN_{level}', \
-            'species_call'] = comb_stats_df.loc[comb_stats_df.call_method == \
-            f'NN_{level}', 'sample_id'].map(leveldict)
-        
-    #Rainbow samples
-    comb_stats_df.loc[(comb_stats_df.species_call.isnull()) & \
-        (comb_stats_df.NN_assignment=='yes'), 'call_method'] = 'NN'
-    comb_stats_df.loc[comb_stats_df.call_method=='NN', 'species_call'] = 'RAINBOW_SAMPLE'
-
-    #Samples with too few targets
-    comb_stats_df.loc[comb_stats_df.NN_assignment=='no', 'call_method'] = 'TOO_FEW_TARGETS'
-    comb_stats_df.loc[comb_stats_df.NN_assignment=='no', 'species_call'] = 'TOO_FEW_TARGETS'
-
-    assert not comb_stats_df.species_call.isnull().any(), 'some samples not assigned'
-    assert not comb_stats_df.call_method.isnull().any(), 'some samples not assigned'
-
-    return comb_stats_df
-
-def generate_summary(ch_assignments, comb_stats_df, version_name):
-    summary = []
-    summary.append(f'Convex hull assignment assignment using reference version {version_name}')
-    summary.append(f'On run containing {comb_stats_df.sample_id.nunique()} samples')
-    summary.append(f'{ch_assignments.index.nunique()} samples met the VAE selection criteria')
-    summary.append(f'Samples are assigned to the following labels:')
-    assignment_dict = dict(ch_assignments.groupby('VAE_species').size())
+def generate_summary(ch_assignments, nn_stats_df, version_name):
+    summary = [
+        f'Convex hull assignment assignment using reference version {version_name}',
+        f'On run containing {nn_stats_df.sample_id.nunique()} samples',
+        f'{ch_assignments.index.nunique()} samples met the VAE selection criteria',
+        f'Samples are assigned to the following labels:'
+    ]
+    assignment_dict = dict(ch_assignments.groupby('vae_species_call').size())
     for key in assignment_dict.keys():
         summary.append(f'{key}:\t {assignment_dict[key]}')
 
     return '\n'.join(summary)
 
 
 def vae(args):
 
     setup_logging(verbose=args.verbose)
 
     os.makedirs(args.outdir, exist_ok =True)
 
     logging.info('ANOSPP VAE data import started')
 
-    hap_df = pd.read_csv(args.haplotypes, sep='\t')
-    comb_stats_df = pd.read_csv(args.manifest, sep='\t')
+    nn_hap_df = pd.read_csv(args.nn_haplotypes, sep='\t')
+    nn_stats_df = pd.read_csv(args.nn_manifest, sep='\t')
+    run_id = nn_stats_df['run_id'].iloc[0]
 
     selection_criteria_file, vae_weights_file, convex_hulls_df, colordict, ref_coordinates, \
         version_name = prep_reference_index(args.reference_version, args.path_to_refversion)
-    vae_samples, vae_hap_df = read_selection_criteria(selection_criteria_file,\
-                                 comb_stats_df, hap_df)
+    vae_samples, vae_hap_df = select_samples(
+        selection_criteria_file,
+        nn_stats_df,
+        nn_hap_df
+        )
     if len(vae_samples) == 0:
-        logging.info("No samples to be run through VAE - skipping to finalising assignments")
-        ch_assignment_df = pd.DataFrame(columns = ['mean1','mean2','mean3','sd1','sd2','sd3','VAE_species'])
+        logging.info('No samples to be run through VAE - skipping to finalising assignments')
+        ch_assignment_df = pd.DataFrame(columns = [
+            'mean1', 'mean2', 'mean3', 'sd1', 'sd2', 'sd3', 'vae_species_call'
+            ])
+        ch_assignment_df.index.name = 'sample_id'
 
     else:
         kmer_table = prep_kmers(vae_hap_df, vae_samples, K)
         latent_positions_df = predict_latent_pos(kmer_table, vae_samples, K, vae_weights_file)
         hull_dict = generate_convex_hulls(convex_hulls_df)
         ch_assignment_df = perform_convex_hull_assignments(hull_dict, latent_positions_df)
-        ch_assignment_df.to_csv(f'{args.outdir}/ch_assignments.tsv', sep='\t')
-        if not bool(args.no_plotting):
-            fig, _ = plot_VAE_assignments(ch_assignment_df, ref_coordinates, colordict)
-            fig.savefig(f'{args.outdir}/VAE_assignment.png')
-    
-    final_assignments = finalise_assignments(comb_stats_df, ch_assignment_df)
-    final_assignments.to_csv(f'{args.outdir}/final_assignments.tsv', sep='\t', index=False)
+        if not args.no_plotting:
+            fig, _ = plot_vae_assignments(ch_assignment_df, ref_coordinates, colordict, run_id)
+            fig.savefig(f'{args.outdir}/vae_assignment.png')
+
+    ch_assignment_df['vae_ref'] = args.reference_version
+    ch_assignment_df.to_csv(f'{args.outdir}/vae_assignment.tsv', sep='\t')
 
-    summary_text = generate_summary(ch_assignment_df, comb_stats_df, version_name)
+    summary_text = generate_summary(ch_assignment_df, nn_stats_df, version_name)
     logging.info(f'writing summary file to {args.outdir}')
     with open(f'{args.outdir}/summary.txt', 'w') as fn:
         fn.write(summary_text)
 
-    logging.info('All done!')
+    logging.info('ANOSPP VAE complete')
 
     
 def main():
     
-    parser = argparse.ArgumentParser("VAE assignment for samples in gambiae complex")
-    parser.add_argument('-a', '--haplotypes', help='Haplotypes tsv file with errors removed \
-                        as generated by anospp-nn', required=True)
-    parser.add_argument('-m', '--manifest', help='Sample assignment tsv file as generated by\
-                        anospp-nn', required=True)
-    parser.add_argument('-r', '--reference_version', help='Reference index version - \
-                        currently a directory name. Default: gcrefv1', default='gcrefv1')
-    parser.add_argument('-o', '--outdir', help='Output directory. Default: nn', default='vae')
-    parser.add_argument('--path_to_refversion', help='path to reference index version.\
-         Default: ref_databases', default='ref_databases')
-    parser.add_argument('--no_plotting', help='Do not generate plots. Default: False', \
-                        default=False)
+    parser = argparse.ArgumentParser('VAE assignment for samples in Anopheles gambiae complex')
+    parser.add_argument('-a', '--nn_haplotypes',
+                        help=f'Haplotypes tsv file with errors removed as generated by anospp-nn with k={K}',
+                        required=True)
+    parser.add_argument('-m', '--nn_manifest',
+                        help=f'Sample assignment tsv file as generated by anospp-nn with k={K}',
+                        required=True)
+    parser.add_argument('-r', '--reference_version',
+                        help='Reference index version - currently a directory name. Default: gcrefv1',
+                        default='gcrefv1')
+    parser.add_argument('-o', '--outdir', help='Output directory. Default: vae', default='vae')
+    parser.add_argument('-p', '--path_to_refversion', 
+                        help='Path to reference index version. Default: ref_databases', 
+                        default='ref_databases')
+    parser.add_argument('--no_plotting', 
+                        help='Do not generate plots. Default: False',
+                        action='store_true', default=False)
     parser.add_argument('-v', '--verbose', 
                         help='Include INFO level log messages', action='store_true')
 
     args = parser.parse_args()
     args.outdir=args.outdir.rstrip('/')
+
     vae(args)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `anospp_analysis-0.2.1/pyproject.toml` & `anospp_analysis-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "anospp-analysis"
-version = "0.2.1"
+version = "0.3.0"
 description = "ANOSPP data analysis"
 authors = ["Alex Makunin <am60@sanger.ac.uk>",]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "anospp_analysis"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.11"
 pandas = "*"
 numpy = "*"
 seaborn = "*"
 BioPython = "*"
 cutadapt = "*"
-keras = "*"
-tensorflow = "*"
+keras = "^2.12"
+tensorflow = "^2.12"
 bokeh = "*"
 
 [tool.poetry.group.dev.dependencies]
+jupyter = "*"
 
 [tool.poetry.scripts]
 anospp-prep = "anospp_analysis.prep:main"
 anospp-qc = "anospp_analysis.qc:main"
 anospp-plasm = "anospp_analysis.plasm:main"
 anospp-nn = "anospp_analysis.nn:main"
 anospp-vae = "anospp_analysis.vae:main"
+anospp-agg = "anospp_analysis.agg:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `anospp_analysis-0.2.1/PKG-INFO` & `anospp_analysis-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: anospp-analysis
-Version: 0.2.1
+Version: 0.3.0
 Summary: ANOSPP data analysis
 License: MIT
 Author: Alex Makunin
 Author-email: am60@sanger.ac.uk
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: BioPython
 Requires-Dist: bokeh
 Requires-Dist: cutadapt
-Requires-Dist: keras
+Requires-Dist: keras (>=2.12,<3.0)
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: seaborn
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow (>=2.12,<3.0)
 Description-Content-Type: text/markdown
 
 # anospp-analysis
 
 Python package for ANOSPP data analysis
 
 ANOSPP is the multiplexed amplicon sequencing assay for Anopheles mosquito species identification and Plasmodium detection. This repository contains the code for analysis of the sequencing results pre-processed with [nf-core ampliseq](https://nf-co.re/ampliseq) pipeline.
```

