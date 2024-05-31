# Comparing `tmp/contourplots-0.3.1.tar.gz` & `tmp/contourplots-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contourplots-0.3.1.tar", last modified: Thu May 30 04:22:42 2024, max compression
+gzip compressed data, was "dist\contourplots-0.3.3.tar", last modified: Fri May 31 05:08:06 2024, max compression
```

## Comparing `contourplots-0.3.1.tar` & `contourplots-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.937276 contourplots-0.3.1/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      704 2024-05-30 04:22:42.936278 contourplots-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.927020 contourplots-0.3.1/contourplots/
--rw-rw-rw-   0        0        0      892 2024-05-30 04:22:20.000000 contourplots-0.3.1/contourplots/__init__.py
--rw-rw-rw-   0        0        0    65056 2024-05-30 04:06:50.000000 contourplots-0.3.1/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 04:22:42.935254 contourplots-0.3.1/contourplots.egg-info/
--rw-rw-rw-   0        0        0      704 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 04:22:42.000000 contourplots-0.3.1/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 04:22:42.938247 contourplots-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-30 04:20:08.000000 contourplots-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      608 2024-05-31 05:08:06.000000 contourplots-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots/
+-rw-rw-rw-   0        0        0      892 2024-05-31 05:07:58.000000 contourplots-0.3.3/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    66631 2024-05-31 04:31:15.000000 contourplots-0.3.3/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      608 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:08:06.000000 contourplots-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-31 05:08:02.000000 contourplots-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `contourplots-0.3.1/LICENSE.txt` & `contourplots-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.3.1/PKG-INFO` & `contourplots-0.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.1
+Version: 0.3.3
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: numpy>=1.23.4
-Requires-Dist: imageio>=2.19.3
```

### Comparing `contourplots-0.3.1/contourplots/__init__.py` & `contourplots-0.3.3/contourplots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 # Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
 # 
 # This module is under the MIT open-source license. See 
 # https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
 # for license details.
 
-__version__ = '0.3.1'
+__version__ = '0.3.3'
 __author__ = 'Sarang S. Bhagwat'
 
 # %% Initialize ContourPlots 
 
 from . import utils
 
 animated_contourplot = utils.animated_contourplot
```

### Comparing `contourplots-0.3.1/contourplots/utils.py` & `contourplots-0.3.3/contourplots/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1169,41 +1169,53 @@
                           values_for_comparison=[],
                           n_minor_ticks=1,
                           y_label='Metric',
                           y_units='units',
                           y_ticks=[],
                           show_x_ticks=False,
                           x_tick_labels=None,
-                          x_tick_fontsize=14,
                           x_tick_wrap_width=6,
                           boxcolor="#A97802",
                           save_file=True,
                           filename='box_and_whiskers_plot',
                           dpi=600,
                           fig_width=1.5,
                           fig_height=5.5,
                           box_width=1.5,
-                          height_ratios = [1, 20],
+                          height_ratios = [1],
+                          width_ratios = [1,5],
                           xlabelpad=5,
                           ylabelpad=5,
                           xticks_fontsize = 17,
                           ylabel_fontsize = 19,
                           yticks_fontsize = 17,
                           default_fontsize = 15,
+                          show=False,
+                          n_cols_subplots=1,
+                          xticks_fontcolor='black',
                           ):
     n_boxes = 1. if not hasattr(uncertainty_data[0], '__iter__') else len(uncertainty_data)
     plt.rcParams['font.sans-serif'] = "Arial Unicode"
     plt.rcParams['font.size'] = str(default_fontsize)
 
-    gridspec_kw={'height_ratios': height_ratios,},
-
-    fig, axs = plt.subplots(1, 1, constrained_layout=True, 
-                            # gridspec_kw=gridspec_kw,
-                            )
-    ax = axs
+    gridspec_kw={
+                'height_ratios': height_ratios,
+                 'width_ratios': width_ratios,
+                 }
+    
+    fig, axs = plt.subplots(1,n_cols_subplots, gridspec_kw=gridspec_kw, constrained_layout = True) if n_cols_subplots>1\
+        else plt.subplots(1,1,constrained_layout = True)
+    
+    ax = axs[0] if n_cols_subplots>1 else axs
+    # ax = plt.subplot(1, 2, 1,
+    #                         # constrained_layout=True, 
+    #                         # gridspec_kw=gridspec_kw,
+    #                         )
+    
+    fig = plt.gcf()
     
     if n_boxes > 1.:
         xrange = [i+0.5 for i in range(n_boxes+1)]
         ax.set_xlim(min(xrange), max(xrange))
         baseline_marker_sizes = [6 for i in range(n_boxes)]
         baseline_marker_colors = ['w' for i in range(n_boxes)]
     # ax.set_facecolor("white")
@@ -1260,16 +1272,19 @@
             top=False,         # ticks along the top edge are off
             direction='inout',
             length=5,
             width=1,
             labelbottom=False if x_tick_labels is None else True)
     
     if show_x_ticks and (x_tick_labels is not None):
-        ax.set_xticks(ticks=list(range(1,n_boxes+1)), labels=x_tick_labels, fontsize=xticks_fontsize)
-        wrap_labels(ax, width=x_tick_wrap_width, fontsize=x_tick_fontsize)
+        ax.set_xticks(ticks=list(range(1,n_boxes+1)), 
+                      labels=x_tick_labels, 
+                      fontsize=xticks_fontsize,
+                      color=xticks_fontcolor)
+        wrap_labels(ax, width=x_tick_wrap_width, fontsize=xticks_fontsize)
     
 
     ax.tick_params(
         axis='y',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction='inout',
         # right=True,
@@ -1342,19 +1357,24 @@
     ax.tick_params(axis='x', which='major', pad=xlabelpad)
     
     # ax.set_ylim(min(y_ticks), max(y_ticks))
 
 
 
     plt.savefig(filename+'.png', dpi=dpi)
+    
+    if show: plt.show()
+    
+    return fig, axs
 
 #%%
 def stacked_bar_plot(dataframe, 
                        y_ticks=[], x_ticks=[], 
                        ylim=[],
+                       ax=None,
                        colors=None, 
                        hatch_patterns=('\\', '//', '|', 'x',),
                        colormap=None,
                        metric_total_values=[], metric_units=[],
                        n_minor_ticks=1,
                        y_label='', y_units='',
                        linewidth=0.8,
@@ -1365,34 +1385,51 @@
                        show_totals=False,
                        totals=[],
                        sig_figs_for_totals=3,
                        units_list=[],
                        totals_label_text=r"$\bfsum:$",
                        xlabelpad=5,
                        ylabelpad=5,
+                       xticks_fontsize = 17,
+                       ylabel_fontsize = 19,
+                       yticks_fontsize = 17,
+                       default_fontsize = 17,
+                       label_wrapsize = 8,
+                       show=False,
+                       subplot_padding = 5,
+                       bar_width=0.6,
+                       xticks_fontcolor='black',
                        ):
+    # axs = plt.subplot(1, 2, 2,
+    #                         # gridspec_kw=gridspec_kw,
+    #                         )
+    
+    fig = plt.gcf()
     
     plt.rcParams['font.sans-serif'] = "Arial Unicode"
-    plt.rcParams['font.size'] = "14"
+    plt.rcParams['font.size'] = str(default_fontsize)
     
-    ax = dataframe.T.plot(kind='bar', stacked=True, edgecolor='k', linewidth=linewidth,
+    ax1 = dataframe.T.plot(kind='bar', stacked=True, edgecolor='k', linewidth=linewidth,
                           color=colors,
                           colormap=colormap,
                           # facecolor="white",
                            # use_index=False,
+                           ax=ax,
                           rot=0,
+                           width=bar_width,
                           )
     
-    
+    if not ax: ax = ax1
     ax.set_facecolor("white")
     
     fig = plt.gcf()
     
     fig.set_figwidth(fig_width)
     fig.set_figheight(fig_height)
+    # fig.tight_layout(pad=subplot_padding)
     
     
     ax.set_yticks(y_ticks,)
     ax.yaxis.set_major_formatter(FuncFormatter(lambda val, pos: f'{val}%'))
     ax.yaxis.set_minor_locator(AutoMinorLocator(n_minor_ticks+1))
     
     
@@ -1437,30 +1474,31 @@
                 if bar_hatch_dict[bar_num] is not None:
                     if curr_facecolor in used_facecolors:
                         patch.set_hatch(bar_hatch_dict[bar_num])
         bar_num+=1
     # print(bar_hatch_dict)
     ax.legend(bbox_to_anchor=(1.05, 1.0), loc='upper left', edgecolor='white')
 
-    ax.set_ylabel(y_label + " [" + y_units + "]", fontsize=14, labelpad=ylabelpad)
+    ax.set_ylabel(y_label + " [" + y_units + "]", fontsize=ylabel_fontsize, labelpad=ylabelpad)
     
     ax.xaxis.labelpad=xlabelpad
     
     # ax.set_xlabel(x_labels, fontsize=14)
     
-    wrap_labels(ax,10)
+    wrap_labels(ax,label_wrapsize)
     
     ax.axhline(y=0,  color='k', linestyle='-', linewidth=linewidth)
     
     ax.tick_params(
         axis='y',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction='inout',
         # right=True,
         width=1,
+        labelsize=yticks_fontsize,
         )
 
     ax.tick_params(
         axis='y',          
         which='major',      
         length=5,
         )
@@ -1474,14 +1512,16 @@
     
     ax.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction='inout',
         # right=True,
         width=1,
+        labelsize=xticks_fontsize,
+        colors=xticks_fontcolor,
         )
     
     
     ax2 = ax.twinx()
     
     
     if not y_ticks==[]:
@@ -1555,15 +1595,17 @@
                      # transform=plt.gcf().transFigure,
                      )
             
     plt.savefig(filename+'.png', dpi=dpi, bbox_inches='tight',
                 facecolor=fig.get_facecolor(),
                 transparent=False)
     
-    plt.show()
+    if show: plt.show()
+    
+    return fig, ax, ax2
     # patterns = [ "/" , "\\" , "|" , "-" , "+" , "x", "o", "O", ".", "*" ]
     # bars = ax.bar([0,5], [0,5])
     # for bar, pattern in zip(bars, patterns):
         # bar.set_hatch(pattern)
     
     # plt.xlabel(list(df.columns), weight='bold')
```

### Comparing `contourplots-0.3.1/contourplots.egg-info/PKG-INFO` & `contourplots-0.3.3/contourplots.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.1
+Version: 0.3.3
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: numpy>=1.23.4
-Requires-Dist: imageio>=2.19.3
```

### Comparing `contourplots-0.3.1/setup.py` & `contourplots-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.3.1',    
+    version='0.3.3',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

