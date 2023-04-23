# Comparing `tmp/tact-0.4.1.tar.gz` & `tmp/tact-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tact-0.4.1.tar", max compression
+gzip compressed data, was "tact-0.5.0.tar", max compression
```

## Comparing `tact-0.4.1.tar` & `tact-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1059 2021-08-03 04:41:06.184099 tact-0.4.1/LICENSE
--rw-r--r--   0        0        0     6401 2021-08-03 04:41:06.184099 tact-0.4.1/README.md
--rw-r--r--   0        0        0    99489 2021-08-03 04:41:06.188099 tact-0.4.1/examples/Carangaria.csv
--rw-r--r--   0        0        0    17020 2021-08-03 04:41:06.188099 tact-0.4.1/examples/Carangaria.tre
--rw-r--r--   0        0        0      778 2021-08-03 04:41:06.188099 tact-0.4.1/examples/README.md
--rw-r--r--   0        0        0      964 2021-08-03 04:42:15.077862 tact-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       19 2021-08-03 04:41:06.188099 tact-0.4.1/tact/__init__.py
--rwxr-xr-x   0        0        0    24608 2021-08-03 04:41:06.188099 tact-0.4.1/tact/cli_add_taxa.py
--rwxr-xr-x   0        0        0     4637 2021-08-03 04:41:06.188099 tact-0.4.1/tact/cli_check_trees.py
--rwxr-xr-x   0        0        0     5127 2021-08-03 04:41:06.188099 tact-0.4.1/tact/cli_taxonomy.py
--rw-r--r--   0        0        0      921 2021-08-03 04:41:06.188099 tact-0.4.1/tact/fastmrca.py
--rw-r--r--   0        0        0     9044 2021-08-03 04:41:06.188099 tact-0.4.1/tact/lib.py
--rw-r--r--   0        0        0     4097 2021-08-03 04:41:06.188099 tact-0.4.1/tact/tree_util.py
--rw-r--r--   0        0        0     7577 2021-08-03 04:42:15.672178 tact-0.4.1/setup.py
--rw-r--r--   0        0        0     7209 2021-08-03 04:42:15.672847 tact-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-23 05:01:17.218186 tact-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2262 2023-04-23 05:01:17.218186 tact-0.5.0/README.md
+-rw-r--r--   0        0        0    99489 2023-04-23 05:01:17.218186 tact-0.5.0/examples/Carangaria.csv
+-rw-r--r--   0        0        0    17020 2023-04-23 05:01:17.218186 tact-0.5.0/examples/Carangaria.tre
+-rw-r--r--   0        0        0      778 2023-04-23 05:01:17.218186 tact-0.5.0/examples/README.md
+-rw-r--r--   0        0        0     1267 2023-04-23 05:02:10.799645 tact-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 05:01:17.218186 tact-0.5.0/tact/__init__.py
+-rwxr-xr-x   0        0        0    20232 2023-04-23 05:01:17.218186 tact-0.5.0/tact/cli_add_taxa.py
+-rwxr-xr-x   0        0        0     9603 2023-04-23 05:01:17.218186 tact-0.5.0/tact/cli_add_toml.py
+-rwxr-xr-x   0        0        0     4924 2023-04-23 05:01:17.218186 tact-0.5.0/tact/cli_check_trees.py
+-rwxr-xr-x   0        0        0     5192 2023-04-23 05:01:17.218186 tact-0.5.0/tact/cli_taxonomy.py
+-rw-r--r--   0        0        0      214 2023-04-23 05:01:17.218186 tact-0.5.0/tact/exceptions.py
+-rw-r--r--   0        0        0      928 2023-04-23 05:01:17.218186 tact-0.5.0/tact/fastmrca.py
+-rw-r--r--   0        0        0      675 2023-04-23 05:01:17.218186 tact-0.5.0/tact/generic_monophyly.py
+-rw-r--r--   0        0        0    10739 2023-04-23 05:01:17.218186 tact-0.5.0/tact/lib.py
+-rw-r--r--   0        0        0     7968 2023-04-23 05:01:17.218186 tact-0.5.0/tact/tree_util.py
+-rw-r--r--   0        0        0     4222 2023-04-23 05:01:17.218186 tact-0.5.0/tact/validation.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 tact-0.5.0/PKG-INFO
```

### Comparing `tact-0.4.1/LICENSE` & `tact-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tact-0.4.1/examples/Carangaria.csv` & `tact-0.5.0/examples/Carangaria.csv`

 * *Files identical despite different names*

### Comparing `tact-0.4.1/examples/Carangaria.tre` & `tact-0.5.0/examples/Carangaria.tre`

 * *Files identical despite different names*

### Comparing `tact-0.4.1/examples/README.md` & `tact-0.5.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `tact-0.4.1/pyproject.toml` & `tact-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 [tool.poetry]
 name = "tact"
-version = "0.4.1"
+version = "0.5.0"
 description = "Taxonomic addition for complete trees: Adds tips to a backbone phylogeny using taxonomy simulated with birth-death models"
 authors = ["Jonathan Chang <me@jonathanchang.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jonchang/tact"
-homepage = "https://github.com/jonchang/tact"
+homepage = "https://tact.jonathanchang.org"
 include = ["examples"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Bio-Informatics"
+]
 
 [tool.poetry.dependencies]
-python = ">= 3.7, < 3.10"
-scipy = "^1.7"
-numpy = "^1.20"
+python = ">= 3.8, < 3.12"
+scipy = "^1.8"
+numpy = "^1.23"
 click = ">=7,<9"
 DendroPy = "^4.5"
+portion = "^2.2"
+toml = "^0.10"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pytest-cov = "^2.12"
 pytest-benchmark = "^3.4"
 pytest-console-scripts = "^1.2"
 hypothesis = "^6.14"
 
 [tool.poetry.scripts]
-tact_build_taxonomic_tree = "tact.cli_taxonomy:main"
 tact_add_taxa = "tact.cli_add_taxa:main"
+tact_add_config = "tact.cli_add_toml:main"
+tact_build_taxonomic_tree = "tact.cli_taxonomy:main"
 tact_check_results = "tact.cli_check_trees:main"
 
-[tool.autopep8]
-max_line_length = 118
-ignore = "E501"
+[tool.black]
+line-length = 118
+target-version = ['py38', 'py39', 'py310', 'py311']
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tact-0.4.1/tact/cli_add_taxa.py` & `tact-0.5.0/tact/cli_add_taxa.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,27 @@
 
 import click
 import dendropy
 
 from . import fastmrca
 from .lib import crown_capture_probability
 from .lib import get_new_times
-from .tree_util import edge_iter
-from .tree_util import ensure_tree_node_depths
 from .tree_util import get_ages
 from .tree_util import get_birth_death_rates
+from .tree_util import get_min_age
 from .tree_util import get_short_branches
 from .tree_util import get_tip_labels
+from .tree_util import graft_node
 from .tree_util import is_binary
-from .tree_util import is_ultrametric
+from .tree_util import is_fully_locked
+from .tree_util import lock_clade
 from .tree_util import update_tree_view
+from .validation import validate_outgroups
+from .validation import validate_taxonomy_tree
+from .validation import BackboneCommand
 
 logger = logging.getLogger(__name__)
 # Speed up logging for PyPy
 logging._srcfile = None
 logging.logThreads = 0
 logging.logProcesses = 0
 logging.logMultiprocessing = 0
@@ -58,15 +62,15 @@
         backbone_node = fastmrca.get(extant_tax)
         seen.append(anc.label)
         computed_ccp = crown_capture_probability(len(full_tax), len(extant_tax))
         if backbone_node is None:
             logger.info(f"    {taxonomy_node.label}: ancestor {anc.label} not monophyletic!")
         elif computed_ccp < ccp:
             logger.info(
-                f"    {taxonomy_node.label}: ancestor {anc.label} fails crown threshold ({computed_ccp:.2f} < {ccp}); using stem"
+                f"    {taxonomy_node.label}: using stem as ancestor {anc.label} ccp {computed_ccp:.2f} < {ccp}"
             )
             taxonomy_target = anc
             backbone_target = backbone_node.parent_node
             break
         else:
             taxonomy_target = anc
             backbone_target = backbone_node
@@ -78,35 +82,33 @@
         sys.exit(1)
     seen.pop()  # ignore last node
     for x in seen:
         invalid_map[x] = taxonomy_target
     return (taxonomy_target, backbone_target)
 
 
-def get_new_branching_times(
-    backbone_node, taxonomy_node, backbone_tree, told=None, tyoung=0, min_ccp=0.8, num_new_times=None
-):
+def get_new_branching_times(backbone_node, taxonomy_node, told=None, tyoung=0, min_ccp=0.8, num_new_times=None):
     """
     Get `n_total` new branching times for a `node`.
     """
     global mrca_rates
     taxon = taxonomy_node.label
-    birth, death, ccp, source = mrca_rates[taxon]
+    birth, death, ccp, _ = mrca_rates[taxon]
     if ccp < min_ccp:
         if backbone_node.parent_node:
             new_told = backbone_node.parent_node.age
             if told is not None:
                 logger.debug(f"    {taxon}: tmax {told:.2f} => {new_told:.2f} because ccp {ccp:.2f} < {min_ccp}")
             else:
                 logger.debug(f"    {taxon}: tmax set to {new_told:.2f} because ccp {ccp:.2f} < {min_ccp}")
         else:
             # TODO: check for a root edge and graft a fake node above that
             new_told = backbone_node.age
             logger.debug(
-                f"    {taxon}: tmax set to {new_told} because even though ccp {ccp:.2f} < {min_ccp} clade is tree root"
+                f"    {taxon}: tmax set to {new_told}; even though ccp {ccp:.2f} < {min_ccp}, clade is tree root"
             )
         told = new_told
     n_extant = len(backbone_node.leaf_nodes())
     n_total = len(taxonomy_node.leaf_nodes())
     if num_new_times is None:
         num_new_times = n_total - n_extant
     ages = get_ages(backbone_node)
@@ -124,15 +126,15 @@
     if len(times) > 5:
         logger.debug(f"    {taxon}: {times[0]:.2f}..{times[-1]:.2f}")
     else:
         logger.debug(f"    {taxon}: " + ", ".join(["{:.2f}" for x in times]).format(*times))
     return times
 
 
-def fill_new_taxa(namespace, node, new_taxa, times, stem=False, excluded_nodes=None):
+def fill_new_taxa(namespace, node, new_taxa, times, stem=False):
     for new_species, new_age in zip(new_taxa, times):
         new_node = dendropy.Node()
         new_node.annotations.add_new("creation_method", "fill_new_taxa")
         new_node.age = new_age
         new_leaf = new_node.new_child(taxon=namespace.require_taxon(new_species), edge_length=new_age)
         new_leaf.annotations.add_new("creation_method", "fill_new_taxa")
         new_leaf.age = 0
@@ -141,87 +143,26 @@
     count_short_branches = len(list(get_short_branches(node)))
     if count_short_branches:
         logger.info(f"{count_short_branches} short branches detected")
 
     return node
 
 
-def graft_node(graft_recipient, graft, stem=False):
-    """
-    Grafts a node `graft` randomly in the subtree below node
-    `graft_recipient`. The attribute `graft.age` must be set so
-    we know where is the best place to graft the node. The node
-    `graft` can optionally have child nodes, in this case the
-    `edge.length` attribute should be set on all child nodes if
-    the tree is to remain ultrametric.
-    """
-
-    # We graft things "below" a node by picking one of the children
-    # of that node and forcing it to be sister to the grafted node
-    # and adjusting the edge lengths accordingly. Therefore, the node
-    # *above* which the graft lives (i.e., the one that will be the child
-    # of the new graft) must fulfill the following requirements:
-    #
-    # 1. Must not be the crown node (cannot graft things above crown node)
-    # 2. Must be younger than the graft node (no negative branches)
-    # 3. Seed node must be older than graft node (no negative branches)
-    # 4. Must not be locked (intruding on monophyly)
-    def filter_fn(x):
-        return x.head_node.age <= graft.age and x.head_node.parent_node.age >= graft.age and x.label != "locked"
-
-    all_edges = list(edge_iter(graft_recipient))
-    if stem:
-        # also include the crown node's subtending edge
-        all_edges.append(graft_recipient.edge)
-    eligible_edges = [x for x in all_edges if filter_fn(x)]
-
-    if not eligible_edges:
-        raise Exception(f"could not place node {graft} in clade {graft_recipient}")
-
-    focal_node = random.choice([x.head_node for x in eligible_edges])
-    seed_node = focal_node.parent_node
-    sisters = focal_node.sibling_nodes()
-
-    # pick a child edge and detach its corresponding node
-    #
-    # DendroPy's Node.remove_child() messes with the edge lengths.
-    # But, Node.clear_child_nodes() simply cuts that bit of the tree out.
-    seed_node.clear_child_nodes()
-
-    # set the correct edge length on the grafted node and make the grafted
-    # node a child of the seed node
-    graft.edge.length = seed_node.age - graft.age
-    if graft.edge.length < 0:
-        raise Exception("negative branch length")
-    sisters.append(graft)
-    seed_node.set_child_nodes(sisters)
-
-    # make the focal node a child of the grafted node and set edge length
-    focal_node.edge.length = graft.age - focal_node.age
-    if focal_node.edge.length < 0:
-        raise Exception("negative branch length")
-    graft.add_child(focal_node)
-
-    # return the (potentially new) crown of the clade
-    if graft_recipient.parent_node == graft:
-        return graft
-    return graft_recipient
-
-
 def create_clade(namespace, species, ages):
     tree = dendropy.Tree(taxon_namespace=namespace)
     species = list(species)
     ages.sort(reverse=True)
     # need to generate the "stem node"
     tree.seed_node.age = ages.pop(0)
     # clade of size 1?
     if not ages:
         node = tree.seed_node.new_child(edge_length=tree.seed_node.age, taxon=namespace.require_taxon(species[0]))
         node.age = 0.0
-        [x.annotations.add_new("creation_method", "create_clade") for x in tree.preorder_node_iter()]
+        for internal_node in tree.preorder_node_iter():
+            internal_node.annotations.add_new("creation_method", "create_clade")
         return tree
     node = tree.seed_node.new_child()
     node.age = ages.pop(0)
     for age in ages:
         valid_nodes = [x for x in tree.nodes() if len(x.child_nodes()) < 2 and age < x.age and x != tree.seed_node]
         assert len(valid_nodes) > 0
         node = random.sample(valid_nodes, 1).pop()
@@ -232,58 +173,33 @@
     for node in tree.preorder_node_iter(filter_fn=lambda x: x.age > 0 and x != tree.seed_node):
         while len(node.child_nodes()) < 2 and len(species) > 0:
             new_species = species.pop()
             new_leaf = node.new_child(taxon=namespace.require_taxon(new_species))
             new_leaf.age = 0.0
     assert n_species == len(tree.leaf_nodes())
     assert len(tree.seed_node.child_nodes()) == 1
-    [x.annotations.add_new("creation_method", "create_clade") for x in tree.preorder_node_iter()]
+    for internal_node in tree.preorder_node_iter():
+        internal_node.annotations.add_new("creation_method", "create_clade")
     assert is_binary(tree.seed_node.child_nodes()[0])
     tree.set_edge_lengths_from_node_ages(error_on_negative_edge_lengths=True)
     # Lock the child of the seed node so that things can still attach to the stem of this new clade
     lock_clade(tree.seed_node.child_nodes()[0])
     if list(get_short_branches(tree.seed_node)):
         logger.info("{} short branches detected".format(len(list(get_short_branches(tree.seed_node)))))
     return tree
 
 
-def lock_clade(node):
-    pre = count_locked(node)
-    for edge in edge_iter(node):
-        edge.label = "locked"
-    post = count_locked(node)
-    if pre != post:
-        logger.debug(f"locking clade: {pre} => {post}")
-
-
-def count_locked(node):
-    sum([x.label == "locked" for x in edge_iter(node)])
-
-
-def is_fully_locked(node):
-    return all([x.label == "locked" for x in edge_iter(node)])
-
-
-def get_min_age(node):
-    try:
-        return min([x.head_node.age for x in edge_iter(node) if x.label != "locked"])
-    except ValueError:
-        return 0.0
-
-
 def fmt_species_list(spp):
     spp = list(spp)
     if len(spp) > 2:
         return f"{spp[0]}, {spp[1]} and {len(spp) - 2} others"
     return " and ".join(spp)
 
 
-def process_node(
-    backbone_tree, backbone_bitmask, all_possible_tips, taxon_node, min_ccp, default_birth, default_death, yule=False
-):
+def process_node(backbone_tree, backbone_bitmask, taxon_node, min_ccp, default_birth, default_death, yule=False):
     # TODO: Fix all the returns and refactor this into something sane
     global mrca_rates
     taxon = taxon_node.label
     parent = taxon_node.parent_node.label
     try:
         birth, death, ccp, _ = mrca_rates[parent]
     except KeyError:
@@ -298,15 +214,17 @@
     extant_bitmask = all_bitmask & backbone_bitmask
     if extant_bitmask is None or extant_bitmask == 0:
         logger.debug(f"MRCA: {taxon} not present in backbone")
         mrca_rates[taxon] = (birth, death, 0.0, f"from {parent} (unsampled)")
         return
     mrca = backbone_tree.mrca(leafset_bitmask=extant_bitmask)
     if not species.issuperset(get_tip_labels(mrca)):
-        logger.debug(f"MRCA: {taxon} not monophyletic in backbone (from {fmt_species_list(get_tip_labels(mrca) - species)})")
+        logger.debug(
+            f"MRCA: {taxon} not monophyletic in backbone (from {fmt_species_list(get_tip_labels(mrca) - species)})"
+        )
         mrca_rates[taxon] = (birth, death, 0.0, f"from {parent} (not monophyletic)")
         return
     extant = len(mrca.leaf_nodes())
     total = len(taxon_node.leaf_nodes())
     if extant > total:
         logger.warning(f"MRCA: {taxon} has {extant} extant species but should have {total} total species")
         mrca_rates[taxon] = (birth, death, 0, f"from {parent} (extant exceeds total)")
@@ -328,15 +246,15 @@
         return
     sf = extant / total
     birth, death = get_birth_death_rates(mrca, sf, yule)
     logger.debug(f"MRCA: {taxon} b={birth:.2f}, d={death:.2f}, sf={sf:.2f} ({extant}/{total}), ccp={ccp:.2f}")
     mrca_rates[taxon] = (birth, death, ccp, "computed")
 
 
-def run_precalcs(taxonomy_tree, backbone_tree, min_ccp=0.8, min_extant=3, yule=False):
+def run_precalcs(taxonomy_tree, backbone_tree, min_ccp=0.8, yule=False):
     global mrca_rates
     tree_tips = get_tip_labels(backbone_tree)
     backbone_bitmask = fastmrca.bitmask(tree_tips)
     all_possible_tips = get_tip_labels(taxonomy_tree)
     nnodes = len(taxonomy_tree.internal_nodes(exclude_seed_node=True))
 
     start_time = time()
@@ -355,107 +273,76 @@
         label="Rates",
         length=nnodes,
         show_pos=True,
         item_show_func=lambda x: x.label if x else None,
     ) as progress:
         for node in progress:
             # updates global mrca_rates as a side effect
-            process_node(
-                backbone_tree, backbone_bitmask, all_possible_tips, node, min_ccp, root_birth, root_death, yule
-            )
+            process_node(backbone_tree, backbone_bitmask, node, min_ccp, root_birth, root_death, yule)
 
     diff = time() - start_time
     if diff > 1:
         logger.debug(f"FastMRCA calculation time: {diff:.1f} seconds")
     return mrca_rates
 
 
-@click.command()
-@click.option("--taxonomy", help="a taxonomy tree", type=click.File("r"), required=True)
+@click.command(cls=BackboneCommand)
+@click.version_option(package_name="tact")
+@click.option(
+    "--taxonomy", help="a taxonomy tree", type=click.File("r"), required=True, callback=validate_taxonomy_tree
+)
 @click.option(
     "--backbone", help="the backbone tree to attach the taxonomy tree to", type=click.File("r"), required=True
 )
-@click.option("--outgroups", help="comma separated list of outgroup taxa to ignore")
+@click.option(
+    "--outgroups",
+    help="comma separated list of outgroup taxa to ignore",
+    type=click.UNPROCESSED,
+    callback=validate_outgroups,
+)
 @click.option("--output", required=True, help="output base name to write out")
 @click.option(
-    "--min-ccp", help="minimum probability to use to say that we've sampled the crown of a clade", default=0.8
+    "--min-ccp",
+    default=0.8,
+    type=click.FloatRange(0, 1, clamp=True),
+    help="minimum probability to use to say that we've sampled the crown of a clade",
 )
 @click.option("--yule", help="assume a Yule pure-birth model (force extinction to be 0)", default=False, is_flag=True)
-@click.option("--ultrametricity-precision", help="precision for ultrametricity checks; by default, checks roughly digits of similarity", default=1e-6)
+@click.option(
+    "--ultrametricity-precision",
+    default=1e-6,
+    type=click.FloatRange(0, 1, clamp=True),
+    help="precision for ultrametricity checks; by default, checks roughly digits of similarity",
+)
 @click.option("-v", "--verbose", help="emit extra information (can be repeated)", count=True)
 def main(taxonomy, backbone, outgroups, output, min_ccp, verbose, yule, ultrametricity_precision):
     """
     Add tips onto a BACKBONE phylogeny using a TAXONOMY phylogeny.
     """
     logger.addHandler(logging.FileHandler(output + ".log.txt"))
     if verbose >= 2:
         logger.setLevel(logging.DEBUG)
     elif verbose == 1:
         logger.setLevel(logging.INFO)
     else:
         logger.setLevel(logging.WARNING)
         logger.addHandler(logging.StreamHandler())
 
-    logger.info("Reading taxonomy")
-    taxonomy = dendropy.Tree.get_from_stream(taxonomy, schema="newick", rooting="default-rooted")
-    tn = taxonomy.taxon_namespace
-    tn.is_mutable = True
-    if outgroups:
-        outgroups = [x.replace("_", " ") for x in outgroups.split(",")]
-        tn.new_taxa(outgroups)
-    tn.is_mutable = False
-
-    # Check for equal depth of all nodes
-    msg = ensure_tree_node_depths(taxonomy)
-    if msg:
-        logger.warning(msg)
-
-    logger.info("Reading backbone")
-
-    try:
-        tree = dendropy.Tree.get_from_stream(backbone, schema="newick", rooting="default-rooted", taxon_namespace=tn)
-    except dendropy.utility.error.ImmutableTaxonNamespaceError as e:
-        logger.error(f"DendroPy error: {e}")
-        print(
-            """
-This usually indicates your backbone has species that are not present in your
-taxonomy. Outgroups not in the taxonomy can be excluded with the argument:
-
-    tact_add_taxa --outgroups outgroup_speciesA,outgroup_speciesB
-
-For more details, run:
-
-    tact_add_taxa --help
-"""
-        )
-        sys.exit(1)
-
-    if not is_binary(tree):
-        logger.error("Backbone tree is not binary!")
-        sys.exit(1)
-
-    update_tree_view(tree)
-
-    ultra, ultra_res = is_ultrametric(tree, ultrametricity_precision)
-    if not ultra:
-        logger.error("Tree is not ultrametric!")
-        logger.error(f"{ultra_res[0][0]} has a root distance of {ultra_res[0][1]}, but {ultra_res[1][0]} has {ultra_res[1][1]}")
-        logger.error("If this is unexpected, consider setting `--ultrametricity-precision` or using phytools::force.ultrametric in R")
-        sys.exit(1)
-
+    tree = backbone
+    tn = tree.taxon_namespace
     tree_tips = get_tip_labels(tree)
     all_possible_tips = get_tip_labels(taxonomy)
 
     logger.info(f"Backbone needs to add {len(tree_tips.symmetric_difference(all_possible_tips))} tips")
 
     full_clades = set()
 
     fastmrca.initialize(tree)
 
-    with open(output + ".rates.csv", "w") as wfile:
+    with open(output + ".rates.csv", "w", encoding="utf-8") as wfile:
         writer = csv.writer(wfile)
         writer.writerow(("taxon", "birth", "death", "ccp", "source"))
         for key, value in run_precalcs(taxonomy, tree, min_ccp, yule=yule).items():
             row = [key]
             row.extend(value)
             writer.writerow(row)
 
@@ -523,42 +410,42 @@
             if tree_tips.issuperset(full_node_species):
                 logger.info(f"    {taxon}: skipping clade {clade} as all species already present in tree")
                 full_clades.remove(clade)
                 continue
             logger.info(f"    {taxon}: adding clade {clade} (n={len(full_node.leaf_nodes())})")
             # Generate all times needed to attach to the main clade
             times = get_new_branching_times(
-                node, taxon_node, tree, tyoung=0, min_ccp=min_ccp, num_new_times=len(full_node_species)
+                node, taxon_node, tyoung=0, min_ccp=min_ccp, num_new_times=len(full_node_species)
             )
 
             if is_fully_locked(node):
                 logger.info(f"    {taxon}: is fully locked, so attaching to stem")
                 # Must attach to stem for this clade, so generate a time on the stem lineage
                 times2 = get_new_branching_times(
                     node,
                     taxon_node,
-                    tree,
                     min_ccp=min_ccp,
                     told=node.parent_node.age,
                     tyoung=node.age,
                     num_new_times=1,
                 )
                 # Drop the oldest time and add on our new time on the stem lineage
                 times.sort()
                 times.pop()
                 times.append(times2.pop())
             else:
                 # Even if the main clade isn't fully locked, it might have a constraint on a valid attachment point
                 min_age = get_min_age(node)
                 if min_age > 0 and max(times) < min_age:
                     logger.info(
-                        f"    {taxon}: has a minimum age constraint {min_age:.2f} but oldest generated time was {max(times):.2f}"
+                        f"    {taxon}: has a minimum age constraint {min_age:.2f}, "
+                        + f"but oldest generated time was {max(times):.2f}"
                     )
                     times2 = get_new_branching_times(
-                        node, taxon_node, tree, tyoung=min_age, min_ccp=min_ccp, num_new_times=1
+                        node, taxon_node, tyoung=min_age, min_ccp=min_ccp, num_new_times=1
                     )
                     # Drop the oldest time and add on our new time on the stem lineage
                     times.sort()
                     times.pop()
                     times.append(times2.pop())
 
             # Generate a new tree
@@ -582,15 +469,15 @@
             continue
         if len(extant_species) == len(species):
             raise ValueError("Enough species are present but mismatched?")
 
         # Taxon spray
         logger.info(f"    {taxon}: adding {len(species.difference(extant_species))} new species")
         node = fastmrca.get(extant_species)
-        times = get_new_branching_times(node, taxon_node, tree, tyoung=get_min_age(node), min_ccp=min_ccp)
+        times = get_new_branching_times(node, taxon_node, tyoung=get_min_age(node), min_ccp=min_ccp)
         node = fill_new_taxa(tn, node, species.difference(tree_tips), times, ccp < min_ccp)
         # Update stuff
         tree_tips = update_tree_view(tree)
         # Since only monophyletic nodes get to here, lock this clade
         lock_clade(node)
         if not is_binary(node):
             # Shouldn't happen
```

### Comparing `tact-0.4.1/tact/cli_check_trees.py` & `tact-0.5.0/tact/cli_check_trees.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 from __future__ import division
 
 import csv
 import functools
 import math
 import multiprocessing
+import os
 
 import click
 import dendropy
 
 from .tree_util import get_birth_death_rates
 from .tree_util import get_monophyletic_node
 from .tree_util import get_tip_labels
 from .tree_util import get_tree
 
 
 def analyze_taxon(bb_tips, st_tips, backbone, simtaxed, taxon_node):
     taxon = taxon_node.label
     if not taxon:
         return None
-    species = set([x.taxon.label for x in taxon_node.leaf_iter()])
+    species = {x.taxon.label for x in taxon_node.leaf_iter()}
 
     notes = []
 
     # does this clade even exist in the backbone?
     bb_species = species.intersection(bb_tips)
     if bb_species:
         bb_mrca = get_monophyletic_node(backbone, bb_species)
@@ -64,27 +65,33 @@
         bb_death,
         st_death,
         ", ".join(notes),
     ]
 
 
 @click.command()
+@click.version_option(package_name="tact")
 @click.argument("simulated", type=click.Path(exists=True, dir_okay=False))
 @click.option("--backbone", type=click.Path(exists=True, dir_okay=False), required=True, help="backbone phylogeny")
 @click.option(
     "--taxonomy",
     type=click.Path(exists=True, dir_okay=False),
     required=True,
     help="taxonomic phylogeny. Possibly created by `tact_build_taxonomic_tree`",
 )
 @click.option(
     "--output", type=click.File("w"), help="Output CSV file report (defaults to standard output)", default="-"
 )
-@click.option("--cores", help="number of parallel cores to use", default=multiprocessing.cpu_count(), type=int)
-@click.option("--chunksize", help="number of tree nodes to allocate to each core", type=int)
+@click.option(
+    "--cores",
+    help="number of parallel cores to use",
+    default=os.cpu_count() or 1,
+    type=click.IntRange(1, os.cpu_count() or 1, clamp=True),
+)
+@click.option("--chunksize", help="number of tree nodes to allocate to each core", type=click.IntRange(1))
 def main(simulated, backbone, taxonomy, output, cores, chunksize):
     """
     Check a SIMULATED phylogeny for consistency with its backbone source tree and a taxonomy.
 
     The SIMULATED phylogeny should have been generated by the tact_add_taxa script.
     All phylogenies should be in Newick format.
     """
@@ -113,15 +120,27 @@
     # We use preorder because the root is going to take the longest to
     # run calculations. Allocating things to cores takes a non-negigible
     # amount of time so we want the root to be running for the longest.
     it = pool.imap_unordered(wrap, taxonomy.preorder_internal_node_iter(exclude_seed_node=True), chunksize=chunksize)
 
     writer = csv.writer(output)
     writer.writerow(
-        "node taxonomy_tips backbone_tips simulated_tips backbone_monophyletic simulated_monophyletic backbone_birth simulated_birth backbone_death simulated_death warnings".split()
+        [
+            "node",
+            "taxonomy_tips",
+            "backbone_tips",
+            "simulated_tips",
+            "backbone_monophyletic",
+            "simulated_monophyletic",
+            "backbone_birth",
+            "simulated_birth",
+            "backbone_death",
+            "simulated_death",
+            "warnings",
+        ]
     )
 
     with click.progressbar(it, width=12, length=nnodes) as prog:
         for result in prog:
             if result:
                 writer.writerow(result)
```

### Comparing `tact-0.4.1/tact/cli_taxonomy.py` & `tact-0.5.0/tact/cli_taxonomy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import collections
 import csv
 
 import click
 import dendropy
 
-from .tree_util import ensure_tree_node_depths
+from .validation import validate_tree_node_depths
 
 
 def fix_file(filename):
     """
     Slurps a file, and does various checks and fixes:
     * Sorts the file
     * Ensures column names are unique
     """
-    with open(filename, "rU") as rfile:
+    with open(filename, "r", encoding="utf-8") as rfile:
         lines = rfile.readlines()
 
     heads = collections.defaultdict(int)
     for item in lines[0].split(","):
         heads[item] += 1
     bad_heads = []
     for key, value in heads.items():
@@ -81,33 +81,33 @@
     row = mangled_row
 
     # Initialize the tree structure
     for col in row:
         ensure(col, ctx=row)
         node = node.new_child(taxon=tn.new_taxon(col))
 
-    to_add = list()
+    to_add = []
     stack = row
-    known_nodes = dict()
+    known_nodes = {}
     with click.progressbar(enumerate(reader), width=12, label="Generating taxonomy", length=len(lines)) as rf:
-        for idx, row in rf:
+        for _, row in rf:
             # Uniquify row names
             row = ["__TAXONOMIC_ROOT__", *row]
             mangled_row = mangle_rank(row, rank_names)
             for orig, new in zip(row, mangled_row):
                 if orig != new:
                     mangled_ranks.add((orig, new))
             row = mangled_row
 
+            prev = None
             for prev, cur in zip(reversed(stack), reversed(row)):
                 ensure(cur, ctx=row)
                 if prev == cur:
                     break
-                else:
-                    to_add.append(cur)
+                to_add.append(cur)
             if prev in known_nodes:
                 node = known_nodes[prev]
             else:
                 node = tree.find_node_with_taxon_label(prev)
                 known_nodes[prev] = node
             while to_add:
                 nt = to_add.pop()
@@ -119,14 +119,15 @@
         click.echo("Note: several rank names were adjusted to ensure uniqueness. These are:")
         for orig, new in mangled_ranks:
             click.echo(f"{orig} => {new}")
     return tree
 
 
 @click.command()
+@click.version_option(package_name="tact")
 @click.argument("taxonomy", type=click.Path(exists=True, dir_okay=False, readable=True))
 @click.option("--output", help="name of the output taxonomic tree", required=True, type=click.Path(writable=True))
 @click.option(
     "--schema",
     help="format of the output taxonomic tree",
     default="newick",
     type=click.Choice(["newick", "nexus", "nexml"]),
@@ -148,12 +149,12 @@
       - NO: Cichlidae,Cichlidae,Cichla temensis
       - NO: Cichlidae,,Cichla temensis
 
     This script makes **many** assumptions about its input for speed. Check
     the example taxonomy in the examples/ folder for guidance.
     """
     taxonomy = build_taxonomic_tree(taxonomy)
-    msg = ensure_tree_node_depths(taxonomy)
+    msg = validate_tree_node_depths(None, None, taxonomy)
     if msg:
         click.echo(msg)
     taxonomy.write_to_path(output, schema=schema)
     click.echo(f"Output written to: {click.format_filename(output)}")
```

### Comparing `tact-0.4.1/tact/fastmrca.py` & `tact-0.5.0/tact/fastmrca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# fastMRCA functions
+"""Singleton object that helps speed up MRCA lookups."""
+
 from __future__ import division
 
 from .tree_util import get_tip_labels
 
 global tree
 
 
@@ -24,20 +25,19 @@
 
 
 def get(labels):
     """Pulls a MRCA node out for the taxa in `labels`."""
     global tree
     labels = set(labels)
     mrca = tree.mrca(leafset_bitmask=bitmask(labels))
-    if not mrca:
-        return None
     if mrca and labels.issuperset(get_tip_labels(mrca)):
         return mrca
+    return None
 
 
 def fastmrca_getter(tn, x):
     """Helper function for submitting stuff."""
     taxa = tn.get_taxa(labels=x)
-    bitmask = 0
+    mask = 0
     for taxon in taxa:
-        bitmask |= tn.taxon_bitmask(taxon)
-    return bitmask
+        mask |= tn.taxon_bitmask(taxon)
+    return mask
```

### Comparing `tact-0.4.1/tact/lib.py` & `tact-0.5.0/tact/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,93 @@
 
 import random
 import sys
 from decimal import Decimal as D
 from math import exp
 from math import log
 
-import dendropy
 import numpy as np
 from scipy.optimize import minimize, minimize_scalar, dual_annealing
 
 # Raise on overflow
 np.seterr(all="raise")
 
 
 def get_bd(r, a):
-    """Converts turnover and relative extinction to birth and death rates."""
+    """
+    Converts turnover and relative extinction to birth and death rates.
+
+    Args:
+        r (float): turnover or net diversification (birth - death)
+        a (float): relative extinction (death / birth)
+
+    Returns:
+        (float, float): birth, death
+    """
     return -r / (a - 1), -a * r / (a - 1)
 
 
 def get_ra(b, d):
-    """Converts birth and death to turnover and relative extinction rates."""
+    """
+    Converts birth and death to turnover and relative extinction rates.
+
+    Args:
+        b (float): birth rate
+        d (float): extinction rate
+
+    Returns:
+        (float, float): turnover, relative extinction
+    """
     return (b - d, d / b)
 
 
 def wrapped_lik_constant(x, sampling, ages):
-    """Wrapper for birth-death likelihood to make optimizing more convenient."""
+    """
+    Wrapper for birth-death likelihood to make optimizing more convenient.
+
+    Args:
+        x (float, float): turnover, relative extinction
+        sampling (float): sampling fraction (0, 1]
+        ages (list): vector of node ages
+
+    Returns:
+        float: a likelihood
+    """
     return lik_constant(get_bd(*x), sampling, ages)
 
 
 def wrapped_lik_constant_yule(x, sampling, ages):
-    """Wrapper for Yule likelihood to make optimizing more convenient."""
+    """
+    Wrapper for Yule likelihood to make optimizing more convenient.
+
+    Args:
+        x (float): birth rate
+        sampling (float): sampling fraction (0, 1]
+        ages (list): vector of node ages
+
+    Returns:
+        float: a likelihood
+    """
     return lik_constant((x, 0.0), sampling, ages)
 
 
 def two_step_optim(func, x0, bounds, args):
-    """Tries to optimize function using the fast L-BFGS-B method, and if that fails, use simulated annealing."""
+    """
+    Conduct a two-step function optimization, first by using the fast L-BFGS-B method,
+    and if that fails, use simulated annealing.
+
+    Args:
+        func (callable): function to optimize
+        x0 (tuple): initial conditions
+        bounds (tuple): boundary conditions
+        args (lsit): additional argumnets to pass to `func`
+
+    Returns:
+        tuple: optimized parameter values
+    """
     try:
         result = minimize(func, x0=x0, bounds=bounds, args=args, method="L-BFGS-B")
         if result["success"]:
             return result["x"].tolist()
     except FloatingPointError:
         pass
 
@@ -51,137 +100,151 @@
     if result["success"]:
         return result["x"].tolist()
 
     raise Exception(f"Optimization failed: {result['message']} (code {result['status']})")
 
 
 def optim_bd(ages, sampling, min_bound=1e-9):
-    """Optimizes birth death using Scipy"""
+    """
+    Optimizes birth and death parameters given a vector of splitting times and sampling fraction.
+
+    Args:
+        ages (list): vector of node ages
+        sampling (float): sampling fraction (0, 1]
+        min_bound (float): minimum birth rate
+
+    Returns:
+        float, float: birth and death rates
+    """
     if max(ages) < 0.000001:
         init_r = 1e-3
     else:
         # Magallon-Sanderson crown estimator
         init_r = (log((len(ages) + 1) / sampling) - log(2)) / max(ages)
         init_r = max(1e-3, init_r)
     bounds = ((min_bound, 100), (0, 1 - min_bound))
     result = two_step_optim(wrapped_lik_constant, x0=(init_r, min_bound), bounds=bounds, args=(sampling, ages))
     return get_bd(*result)
 
 
 def optim_yule(ages, sampling, min_bound=1e-9):
-    """Optimizes a Yule model using Scipy"""
-    if max(ages) < 0.000001:
-        init_r = 1e-3
-    else:
-        # Magallon-Sanderson crown estimator
-        init_r = (log((len(ages) + 1) / sampling) - log(2)) / max(ages)
-        init_r = max(1e-3, init_r)
+    """
+    Optimizes birth parameter under a Yule model, given a vector of splitting times and sampling fraction.
+
+    Args:
+        ages (list): vector of node ages
+        sampling (float): sampling fraction (0, 1]
+        min_bound (float): minimum birth rate
+
+    Returns:
+        float, float: birth and death rates (where death is always 0)
+    """
     bounds = (min_bound, 100)
     result = minimize_scalar(wrapped_lik_constant_yule, bounds=bounds, args=(sampling, ages), method="Bounded")
     if result["success"]:
         return (result["x"], 0.0)
 
     raise Exception(f"Optimization failed: {result['message']} (code {result['status']})")
 
 
-def p0_exact(t, l, m, rho):
+def p0_exact(t, l, m, rho):  # noqa: E741
+    "Exact version of `p0` using Decimal math."
     t = D(t)
-    l = D(l)
+    l = D(l)  # noqa: E741
     m = D(m)
     rho = D(rho)
     return D(1) - rho * (l - m) / (rho * l + (l * (D(1) - rho) - m) * (-(l - m) * t).exp())
 
 
-def p0(t, l, m, rho):
+def p0(t, l, m, rho):  # noqa: E741
     try:
         return 1 - rho * (l - m) / (rho * l + (l * (1 - rho) - m) * exp(-(l - m) * t))
     except FloatingPointError:
         return float(p0_exact(t, l, m, rho))
 
 
-def p1_exact(t, l, m, rho):
-    """Exact version of p1 using Decimal math."""
+def p1_exact(t, l, m, rho):  # noqa: E741
+    """Exact version of `p1` using Decimal math."""
     t = D(t)
-    l = D(l)
+    l = D(l)  # noqa: E741
     m = D(m)
     rho = D(rho)
     num = rho * (l - m) ** D(2) * (-(l - m) * t).exp()
     denom = (rho * l + (l * (1 - rho) - m) * (-(l - m) * t).exp()) ** D(2)
     return num / denom
 
 
-def p1_orig(t, l, m, rho):
-    """Original version of p1, here for testing and comparison purposes."""
+def p1_orig(t, l, m, rho):  # noqa: E741
+    """Original version of `p1`, here for testing and comparison purposes."""
     try:
         num = rho * (l - m) ** 2 * np.exp(-(l - m) * t)
         denom = (rho * l + (l * (1 - rho) - m) * np.exp(-(l - m) * t)) ** 2
         res = num / denom
     except (OverflowError, FloatingPointError):
         res = float(p1_exact(t, l, m, rho))
     if res == 0.0:
         return sys.float_info.min
     return res
 
 
-def p1(t, l, m, rho):
+def p1(t, l, m, rho):  # noqa: E741
     """
-    Optimized version of p1 using common subexpression elimination and strength reduction from
-    exponentiation to multiplication.
+    Optimized version of `p1_orig` using common subexpression elimination and strength reduction
+    from exponentiation to multiplication.
     """
     try:
         ert = np.exp(-(l - m) * t, dtype=np.float64)
         num = rho * (l - m) ** 2 * ert
         denom = (rho * l + (l * (1 - rho) - m) * ert) ** 2
         res = num / denom
     except (OverflowError, FloatingPointError):
         res = float(p1_exact(t, l, m, rho))
     if res == 0.0:
         return sys.float_info.min
     return res
 
 
-def intp1_exact(t, l, m):
-    """Exact version of intp1 using Decimal math."""
-    l = D(l)
+def intp1_exact(t, l, m):  # noqa: E741
+    """Exact version of `intp1` using Decimal math."""
+    l = D(l)  # noqa: E741
     m = D(m)
     t = D(t)
     num = D(1) - (-(l - m) * t).exp()
     denom = l - m * (-(l - m) * t).exp()
     return num / denom
 
 
-def intp1(t, l, m):
+def intp1(t, l, m):  # noqa: E741
     try:
         return (1 - exp(-(l - m) * t)) / (l - m * exp(-(l - m) * t))
     except OverflowError:
         return float(intp1_exact(t, l, m))
 
 
 def lik_constant(vec, rho, t, root=1, survival=1, p1=p1):
     """
     Calculates the likelihood of a constant-rate birth-death process, conditioned
     on the waiting times of a phylogenetic tree and degree of incomplete sampling.
 
-    Based off of the R function TreePar::LikConstant written by Tanja Stadler.
+    Based off of the R function `TreePar::LikConstant` written by Tanja Stadler.
 
     T. Stadler. On incomplete sampling under birth-death models and connections
     to the sampling-based coalescent. Jour. Theo. Biol. 261: 58-66, 2009.
 
-    Positional arguments:
-    vec -- a two element list of birth and death
-    rho -- sampling fraction
-    t -- vector of waiting times
-
-    Keyword arguments:
-    root -- include the root or not? (default: 1)
-    survival -- assume survival of the process (default: 1)
+    Args:
+        vec (float, float): two element tuple of birth and death
+        rho (float): sampling fraction
+        t (list): vector of waiting times
+        root (bool): include the root or not? (default: 1)
+        survival (bool): assume survival of the process? (default: 1)
 
-    Returns a likelihood.
+    Returns:
+        float: a likelihood
     """
-    l = vec[0]
+    l = vec[0]  # noqa: E741
     m = vec[1]
     t.sort(reverse=True)
     lik = (root + 1) * log(p1(t[0], l, m, rho))
     for tt in t[1:]:
         lik += log(l) + log(p1(tt, l, m, rho))
     if survival == 1:
         lik -= (root + 1) * log(1 - p0(t[0], l, m, rho))
@@ -193,66 +256,70 @@
     Calculate the probability that a sample of `k` taxa from a clade
     of `n` total taxa includes a root node, under a Yule process.
 
     This equation is taken from:
 
     Sanderson, M. J. 1996. How many taxa must be sampled to identify
     the root node of a large clade? Systematic Biology 45:168-173
+
+    Args:
+        n (int): total number of taxa
+        k (int): sampled taxa
+
+    Returns:
+        float: probability
     """
     if n < k:
         raise Exception(f"n must be greater than or equal to k (n={n}, k={k})")
     if n == 1 and k == 1:
         return 0  # not technically correct but it works for our purposes
     return 1 - 2 * (n - k) / ((n - 1) * (k + 1))
 
 
 # TODO: This could probably be optimized
 def get_new_times(ages, birth, death, missing, told=None, tyoung=None):
     """
     Simulates new speciation events in an incomplete phylogeny assuming a
-    constnat-rate birth-death process.
+    constant-rate birth-death process.
 
-    Adapted from the R function TreeSim::corsim written by Tanja Stadler.
+    Adapted from the R function `TreeSim::corsim` written by Tanja Stadler.
 
     N. Cusimano, T. Stadler, S. Renner. A new method for handling missing
     species in diversification analysis applicable to randomly or
     non-randomly sampled phylogenies. Syst. Biol., 61(5): 785-792, 2012.
 
-    Positional arguments:
-    ages -- vector of waiting times
-    birth -- birth rate
-    death -- death rate
-    missing -- number of missing taxa to simulate
-
-    Keyword arguments:
-    told -- maximum simulated age (default: `max(ages)`)
-    tyoung -- minimum simulated age bound (default: `0`)
+    Args:
+        ages (list): vector of waiting times
+        birth (float): birth rate
+        death (float): death rate
+        missing (int): number of missing taxa to simulate
+        told (float): maximum simulated age (default: `max(ages)`)
+        tyoung (float): minimum simulated age bound (default: `0`)
 
-    Returns a vector of simulated waiting times.
+    Returns:
+        list: vector of simulated waiting times.
     """
     if told is None:
         told = max(ages)
     if len(ages) > 0:
         if max(ages) > told and abs(max(ages) - told) > sys.float_info.epsilon:
             raise Exception("Zero or negative branch lengths detected in backbone phylogeny")
     if tyoung is None:
         tyoung = 0
 
     ages.sort(reverse=True)
-    times = [x for x in ages if x <= told and x >= tyoung]
+    times = [x for x in ages if told >= x >= tyoung]
     times = [told] + times + [tyoung]
     ranks = range(0, len(times))
-    only_new = list()
+    only_new = []
     while missing > 0:
         if len(ranks) > 2:
-            distrranks = list()
+            distrranks = []
             for i in range(1, len(ranks)):
-                temp = ranks[i] * (
-                    intp1(times[i - 1], birth, death) - intp1(times[i], birth, death)
-                )
+                temp = ranks[i] * (intp1(times[i - 1], birth, death) - intp1(times[i], birth, death))
                 distrranks.append(temp)
             try:
                 dsum = sum(distrranks)
                 distrranks = [x / dsum for x in distrranks]
                 for i in range(1, len(distrranks)):
                     distrranks[i] = distrranks[i] + distrranks[i - 1]
                 r = random.uniform(0, 1)
@@ -265,16 +332,12 @@
             addrank = 0
         r = random.uniform(0, 1)
         const = intp1(times[addrank], birth, death) - intp1(times[addrank + 1], birth, death)
         try:
             temp = intp1(times[addrank + 1], birth, death) / const
         except ZeroDivisionError:
             temp = 0.0
-        xnew = (
-            1
-            / (death - birth)
-            * log((1 - (r + temp) * const * birth) / (1 - (r + temp) * const * death))
-        )
+        xnew = 1 / (death - birth) * log((1 - (r + temp) * const * birth) / (1 - (r + temp) * const * death))
         only_new.append(xnew)
         missing -= 1
     only_new.sort(reverse=True)
     return only_new
```

