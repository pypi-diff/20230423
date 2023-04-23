# Comparing `tmp/sprint2-0.0.17.tar.gz` & `tmp/sprint2-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint2-0.0.17.tar", last modified: Thu Apr 20 19:34:05 2023, max compression
+gzip compressed data, was "sprint2-0.0.19.tar", last modified: Sun Apr 23 17:15:15 2023, max compression
```

## Comparing `sprint2-0.0.17.tar` & `sprint2-0.0.19.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.385189 sprint2-0.0.17/
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.250200 sprint2-0.0.17/MaskAGref/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-20 19:33:49.000000 sprint2-0.0.17/MaskAGref/MaskAGref.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-20 19:33:49.000000 sprint2-0.0.17/MaskAGref/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:34:10.383189 sprint2-0.0.17/PKG-INFO
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.296196 sprint2-0.0.17/getDsRNA/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9741 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step1_transcript_blat.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step2_transcript_dspair.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step3_bedtools_sorted_rmLC.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step4_combine_by_chr.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step5_merge_dsRNA.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2464 2023-04-20 19:33:44.000000 sprint2-0.0.17/getDsRNA/step6_dsRNA.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.324194 sprint2-0.0.17/getRES/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2034 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    45388 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step1_SNVcalling.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    20538 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step2_annotation_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    19408 2023-04-20 19:33:47.000000 sprint2-0.0.17/getRES/step3_dsRNA_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-20 19:34:10.386189 sprint2-0.0.17/setup.cfg
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-20 19:33:54.000000 sprint2-0.0.17/setup.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-20 19:34:10.376189 sprint2-0.0.17/sprint2.egg-info/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/PKG-INFO
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      565 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/SOURCES.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/dependency_links.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/entry_points.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/requires.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-20 19:34:10.000000 sprint2-0.0.17/sprint2.egg-info/top_level.txt
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.339593 sprint2-0.0.19/
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:20.904630 sprint2-0.0.19/MaskAGref/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-23 13:54:07.000000 sprint2-0.0.19/MaskAGref/MaskAGref.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-23 13:54:07.000000 sprint2-0.0.19/MaskAGref/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-23 17:15:21.337593 sprint2-0.0.19/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     8510 2023-04-23 13:54:07.000000 sprint2-0.0.19/README.md
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.058617 sprint2-0.0.19/getDsRNA/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9630 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step1_transcript_blat.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step2_transcript_dspair.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step3_bedtools_sorted_rmLC.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step4_combine_by_chr.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step5_merge_dsRNA.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2450 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step6_dsRNA.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.194605 sprint2-0.0.19/getRES/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     7678 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    45394 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step1_SNVcalling.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    21192 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step2_annotation_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    17443 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step3_dsRNA_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-23 17:15:21.340592 sprint2-0.0.19/setup.cfg
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-23 13:54:08.000000 sprint2-0.0.19/setup.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.330593 sprint2-0.0.19/sprint2.egg-info/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      575 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/SOURCES.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/dependency_links.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/entry_points.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/requires.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/top_level.txt
```

### Comparing `sprint2-0.0.17/MaskAGref/MaskAGref.py` & `sprint2-0.0.19/MaskAGref/MaskAGref.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/PKG-INFO` & `sprint2-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.17
+Version: 0.0.19
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.17/getDsRNA/__init__.py` & `sprint2-0.0.19/getDsRNA/__init__.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/getDsRNA/step1_transcript_blat.py` & `sprint2-0.0.19/getDsRNA/step1_transcript_blat.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,28 +139,27 @@
 
     OUT_DIR = OUT_DIR_BASE+"/"
     if not os.path.isdir(OUT_DIR):
         os.mkdir(OUT_DIR)
     ##----------------------------------------------------------------------------------------------------------
     ##load reference genome fasta file and compute time
     ##running time is:40 seconds
-    print("1.Start load reference genome file...")
+    print("1.Loading reference genome file...")
     global chrom
     chrom=SeqIO.to_dict(SeqIO.parse(ref_in_path, "fasta"))
     #print(list(chrom.keys())[0:50])
-    print("\t\tReference genome file is OK!")
+    #print("\t\tReference genome file is OK!")
     global all_chroms,all_chroms_new
     ##print number of bases in each chrom
     all_chroms=list(chrom.keys())###640 sequences
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##split each chrom seqence
-    print("2.Start split each chrom seqence...")
     all_chroms_new={}
     fi=open(trans_path)
     while 1 :
         lines=fi.readlines(10000)
         if not lines:
             break
         for line in lines:
@@ -178,15 +177,14 @@
     chrom=all_chroms_new
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##split reference sequence by chromosome
     ##running time is:4 seconds
-    print("3.Start split each transcript sequence...")
     global ref_out_dir
     ref_out_dir=OUT_DIR+"/reference"
     if not os.path.isdir(ref_out_dir):
         os.mkdir(ref_out_dir)
 
     pool_size = CPU
     pool1 = Pool(pool_size)  
@@ -198,15 +196,15 @@
 
     ##----------------------------------------------------------------------------------------------------------
 
     ##----------------------------------------------------------------------------------------------------------
     ##find all Query sequences in all hg38 reference file with multiprocessing pool
     ##running time is:334 seconds (5.6 minutes)
     ## all sequence query finder 
-    print("4.Start find query sequences....")
+    print("2.Findind query sequences....")
     global fa_out_dir
     fa_out_dir=OUT_DIR+"/query"
     if not os.path.isdir(fa_out_dir):
         os.mkdir(fa_out_dir)
 
     pool_size = int(CPU)
     pool1 = Pool(pool_size)  
@@ -225,15 +223,15 @@
     ##running time is : ~ 3 days
     ## all BLAT
     global blat_out_dir
     blat_out_dir=OUT_DIR+"/BLAT"
     CPU=CPU
     if not os.path.isdir(blat_out_dir):
         os.mkdir(blat_out_dir)
-    print("5.Start run BLAT....")     
+    print("3.Running BLAT....")     
     time_start = int(time.perf_counter())
 
     querys=os.listdir(OUT_DIR+"/query")
     pool_size = CPU
     pool1 = Pool(pool_size)  
     for qu in querys:
         this_chr=qu.split("_id_")[0]
```

### Comparing `sprint2-0.0.17/getDsRNA/step2_transcript_dspair.py` & `sprint2-0.0.19/getDsRNA/step2_transcript_dspair.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/getDsRNA/step3_bedtools_sorted_rmLC.py` & `sprint2-0.0.19/getDsRNA/step3_bedtools_sorted_rmLC.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/getDsRNA/step4_combine_by_chr.py` & `sprint2-0.0.19/getDsRNA/step4_combine_by_chr.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/getDsRNA/step5_merge_dsRNA.py` & `sprint2-0.0.19/getDsRNA/step5_merge_dsRNA.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.17/getDsRNA/step6_dsRNA.py` & `sprint2-0.0.19/getDsRNA/step6_dsRNA.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         ds_path = ds_dir + f
         file_out = outdir + f
         ARG = [ds_path, file_out, add_num]
         pool1.apply_async(dspair_add, (ARG,))
 
     pool1.close() 
     pool1.join()     
-    '''
+
     subprocess.Popen("rm -r " + base_path + "*rev/", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "BLAT", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "query", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "reference", shell=True).wait()
     subprocess.Popen("rm -r " + base_path + "ds_files/", shell=True).wait()
-    '''
+
     time_end = int(time.perf_counter())
     run_time = str(time_end - time_start)
     print("Processing running time is: " + run_time + " seconds" + "\n")
```

### Comparing `sprint2-0.0.17/getRES/step1_SNVcalling.py` & `sprint2-0.0.19/getRES/step1_SNVcalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,15 +807,15 @@
 
     ##----------------------------------------------------------------------------------------------------------
     ##genome
     print("\tStart mapping genome ...")
     if not os.path.isdir(tmp+"genome/"):
         os.mkdir(tmp+"genome/")
     TAG="genome"
-    fq2bam(tmp+"genome/",True,TAG,read1,read2,refgenome,bwa,samtools,mapcpu)
+    fq2bam(tmp+"genome/",paired_end,TAG,read1,read2,refgenome,bwa,samtools,mapcpu)
     subprocess.Popen(samtools+" index "+tmp+"genome/all.bam",shell=True).wait()
 
     os.remove(tmp+"cut_read1.fastq")
     if os.path.exists(tmp+"cut_read2.fastq"):
         os.remove(tmp+"cut_read2.fastq")
 
     subprocess.Popen(samtools+" view -f4 "+tmp+"genome/all.bam > "+tmp+"genome_unmapped.sam",shell=True).wait()
```

### Comparing `sprint2-0.0.17/getRES/step2_annotation_based.py` & `sprint2-0.0.19/getRES/step2_annotation_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     for i in range(len(all_num)):
         this_line=str(all_type[i])+"\t"+str(all_num[i])+"\t"+str(all_ratio[i])+"\n"
         fo.write(this_line)
     fo.close()
 
 ##----------------------------------------------------------------------------------------------------------
 
-def getRES():
+def getRES1():
     subprocess.Popen("cp " + ori_tmp+"regular.snv" + " " + tmp+"regular.snv",shell=True).wait() 
     subprocess.Popen("cp " + ori_tmp+"hyper_mskAG.snv" + " " + tmp+"hyper_mskAG.snv",shell=True).wait() 
     subprocess.Popen("cp " + ori_tmp+"hyper_mskTC.snv" + " " + tmp+"hyper_mskTC.snv",shell=True).wait() 
     annotate(tmp+"regular.snv",repeat,tmp+"regular.snv.anno")    
     seperate(tmp+"regular.snv.anno",tmp+"regular.snv.anno.alu",tmp+"regular.snv.anno.nalurp",tmp+"regular.snv.anno.nrp","Alu")
     get_snv_with_ad(tmp+"regular.snv.anno.alu",tmp+"regular.snv.anno.alu.ad2",2)
     snv_cluster(tmp+"regular.snv.anno.alu",tmp+"regular_alu.res.ad1", cluster_distance, cluster_size_alu_ad1)
@@ -426,35 +426,48 @@
     o2b(tmp+"regular.res_tmp",tmp+"regular.res") 
 
     snv_cluster(tmp+"hyper_mskTC.snv",tmp+"hyper_mskTC.res",cluster_distance,cluster_size_hp)
     snv_cluster(tmp+"hyper_mskAG.snv",tmp+"hyper_mskAG.res",cluster_distance,cluster_size_hp)
     snv_or(tmp+"hyper_mskTC.res",tmp+"hyper_mskAG.res",tmp+"hyper.res")
 
 ##----------------------------------------------------------------------------------------------------------
+def getRES2():
+    subprocess.Popen("cp " + ori_tmp+"hyper_mskAG.snv" + " " + tmp+"hyper_mskAG.snv",shell=True).wait() 
+    subprocess.Popen("cp " + ori_tmp+"hyper_mskTC.snv" + " " + tmp+"hyper_mskTC.snv",shell=True).wait() 
+    snv_cluster(tmp+"hyper_mskTC.snv",tmp+"hyper_mskTC.res", cluster_distance, cluster_size_nrp_hp)
+    snv_cluster(tmp+"hyper_mskAG.snv",tmp+"hyper_mskAG.res", cluster_distance, cluster_size_nrp_hp)
+    snv_or(tmp+"hyper_mskTC.res",tmp+"hyper_mskAG.res",tmp+"hyper.res")
+
+
 ##----------------------------------------------------------------------------------------------------------
 
 def main(args):
 
     parser = argparse.ArgumentParser(description="python3 step2_annotation_based.py")
     parser.add_argument("-o", "--output",default = str(os.getcwd()),  help="path to Output Directory (defalt:Working Directory)")
     parser.add_argument("-s", "--snv",default = str(os.getcwd()),  help="path to SNV Directory (defalt:Working Directory)")
-    parser.add_argument("-rp", "--repeat",default = str(os.getcwd())+"repeat.bed",  help="path to repeat file (defalt:~/repeat.bed)")
+    parser.add_argument("-rp", "--repeat",help="path to repeat file #Optional")
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
 
     global ori_tmp,tmp,repeat
     ori_tmp=str(args.snv)+"/"
     tmp=str(args.output)+"/"
     repeat=str(args.repeat)
 
+    if args.repeat:
+        repeat=str(args.repeat)
+    else:
+        repeat=False
+
     global cluster_distance,cluster_size_alu_ad1,cluster_size_alu_ad2,cluster_size_nalurp,cluster_size_nrp
     global cluster_size_rg,cluster_size_hp,cluster_size_alu_hp,cluster_size_nalurp_hp,cluster_size_nrp_hp
     global strand_specify,var_limit,poly_limit,rm_multi
     cluster_distance=200
     cluster_size_alu_ad1 = 3
     cluster_size_alu_ad2 = 2
     cluster_size_nalurp = 5
@@ -471,27 +484,33 @@
 
     ##----------------------------------------------------------------------------------------------------------
 
     print("Step2 Identifying RESs based repeat annotation...")
     time_start = int(time.perf_counter())
     if not os.path.isdir(tmp):
         os.mkdir(tmp)
-    getRES()    
-    if not os.path.isdir(tmp+"regular"):
-        os.mkdir(tmp+"anno_regular")
+    if repeat != False:
+        getRES1()    
+        if not os.path.isdir(tmp+"anno_regular"):
+            os.mkdir(tmp+"anno_regular")
+        subprocess.Popen("mv " + tmp+"regular* " + tmp+"anno_regular/",shell=True).wait() 
+        cmd="awk -F '\t' '{print $1\"\t\"$2\"\t\"$3\"\t\"$4\"\t\"$5}' "
+        subprocess.Popen(cmd + tmp+"anno_regular/regular.res > " + tmp+"anno_regular.res",shell=True).wait() 
+        ARG=[tmp+"anno_regular.res",tmp+"anno_regular_res.stat"]
+        stat_res(ARG)
+
+    else:
+        getRES2()
+
     if not os.path.isdir(tmp+"hyper"):
         os.mkdir(tmp+"hyper")
-    subprocess.Popen("mv " + tmp+"regular* " + tmp+"anno_regular/",shell=True).wait() 
+    
     subprocess.Popen("mv " + tmp+"hyper_* " + tmp+"hyper/",shell=True).wait() 
     subprocess.Popen("mv " + tmp+"hyper.* " + tmp+"hyper/",shell=True).wait() 
-    cmd="awk -F '\t' '{print $1\"\t\"$2\"\t\"$3\"\t\"$4\"\t\"$5}' "
-    subprocess.Popen(cmd + tmp+"anno_regular/regular.res > " + tmp+"anno_regular.res",shell=True).wait() 
     subprocess.Popen("cp " + tmp+"hyper/hyper.res " + tmp+"hyper.res",shell=True).wait() 
 
-    ARG=[tmp+"anno_regular.res",tmp+"anno_regular_res.stat"]
-    stat_res(ARG)
     ARG=[tmp+"hyper.res",tmp+"SPRINT2_Hyper_RES.stat"]
     stat_res(ARG)
     time_end = int(time.perf_counter())
     run_time = str(time_end-time_start)
 
-    print("Processing Step2 running time is:" + run_time + " seconds" + "\n")     
+    print("Repeat-based RES calling running time is:" + run_time + " seconds" + "\n")
```

### Comparing `sprint2-0.0.17/getRES/step3_dsRNA_based.py` & `sprint2-0.0.19/getRES/step3_dsRNA_based.py`

 * *Files 13% similar despite different names*

```diff
@@ -368,25 +368,25 @@
 
 ##----------------------------------------------------------------------------------------------------------
 def main(args):
 
     parser = argparse.ArgumentParser(description="python3 step3_dsRNA_based.py")
     parser.add_argument("-o", "--output",default = str(os.getcwd()),  help="path to Output Directory (defalt:Working Directory)")
     parser.add_argument("-s", "--snv",default = str(os.getcwd()),  help="path to SNV Directory (defalt:Working Directory)")
-    parser.add_argument("-ds", "--dsrna",default = str(os.getcwd()),  help="path to candidate dsRNA Directory (defalt:Working Directory)")
+    parser.add_argument("-ds", "--dsrna",default = str(os.getcwd())+"/dsRNA_file/",  help="path to candidate dsRNA Directory (defalt:~/dsRNA_file/)")
     parser.add_argument("-b", "--bedtools",default = str(os.getcwd())+"bedtools",  help="path to bedtools (defalt:~/bedtools)")
     parser.add_argument("-p", "--cpu",default = 1,  help="CPU number (defalt=1)")
 
     try:
         args = parser.parse_args(args.split())
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
 
-
+    global allsnv_path,outpath1,bedtools_path,ds_path,snv_path,outpath0
     outpath0=str(args.output)+"/"
     snv_path=str(args.snv)+"/"
     ds_path=str(args.dsrna)+"/"
     bedtools_path=str(args.bedtools)
     CPU=int(args.cpu)
 
     #print("Step3 Identifying RESs based dsRNA... ") 
@@ -421,39 +421,15 @@
 
     ##----------------------------------------------------------------------------------------------------------
 
     subprocess.Popen("cat "+outpath1+"/chr*/ff_res_filter_all.res | "+bedtools_path+" sort -i | uniq > "+outpath0+"ds_regular.res",shell=True).wait()
     ARG=[outpath0+"ds_regular.res",outpath0+"ds_regular_res.stat"]
     stat_res(ARG)
 
-    subprocess.Popen("cat "+outpath0+"ds_regular.res "+outpath0+"anno_regular.res | "+bedtools_path+" sort -i | uniq > "+outpath0+"regular.res",shell=True).wait()
-    ARG=[outpath0+"regular.res",outpath0+"SPRINT2_Regular_RES.stat"]
-    stat_res(ARG)
-
-    subprocess.Popen("cat "+outpath0+"regular.res "+outpath0+"hyper.res | "+bedtools_path+" sort -i | uniq > "+outpath0+"ALL.res",shell=True).wait()
-    ARG=[outpath0+"ALL.res",outpath0+"SPRINT2_ALL_RES.stat"]
-    stat_res(ARG)
-
-    getBedDP(bed_in_path=outpath0+"ALL.res", bam_in_path=snv_path+"genome/all.bam", bed_out_path=outpath0+"ALL.res.dp", bedtools_path=bedtools_path)
-    getBedDP(bed_in_path=outpath0+"regular.res", bam_in_path=snv_path+"genome/all.bam", bed_out_path=outpath0+"regular.res.dp", bedtools_path=bedtools_path)
-    getBedDP(bed_in_path=outpath0+"hyper.res", bam_in_path=snv_path+"genome/all.bam", bed_out_path=outpath0+"hyper.res.dp", bedtools_path=bedtools_path)
-
-    subprocess.Popen('echo "#Chrom\tStart(0base)\tEnd(1base)\tType\tSupporting_reads\tDepth" | cat - '+outpath0 +'/ALL.res.dp   > '+outpath0+'/SPRINT2_identified_all.res',shell=True).wait()
-    subprocess.Popen('echo "#Chrom\tStart(0base)\tEnd(1base)\tType\tSupporting_reads\tDepth" | cat - '+outpath0 +'/regular.res.dp   > '+outpath0+'/SPRINT2_identified_regular.res',shell=True).wait()
-    subprocess.Popen('echo "#Chrom\tStart(0base)\tEnd(1base)\tType\tSupporting_reads\tDepth" | cat - '+outpath0 +'/hyper.res.dp   > '+outpath0+'/SPRINT2_identified_hyper.res',shell=True).wait()
-
-    if not os.path.isdir(outpath0+"RES"):
-        os.mkdir(outpath0+"RES")
-    subprocess.Popen("mv " + outpath0+"regular.res* " + outpath0+"anno_regular/",shell=True).wait() 
-    subprocess.Popen("mv " + outpath0+"hyper.res* " + outpath0+"RES/",shell=True).wait() 
-    subprocess.Popen("mv " + outpath0+"ALL.res* " + outpath0+"RES/",shell=True).wait() 
-    subprocess.Popen("mv " + outpath0+"anno*res* " + outpath0+"RES/",shell=True).wait() 
-    subprocess.Popen("mv " + outpath0+"ds*res* " + outpath0+"RES/",shell=True).wait() 
-
     time_end = int(time.perf_counter())
     run_time = str(time_end-time_start)
-    print("Processing Step3 running time is:" + run_time + " seconds" + "\n")     
+    print("dsRNA-based RES calling running time is:" + run_time + " seconds" + "\n")     
 
 ##----------------------------------------------------------------------------------------------------------
```

### Comparing `sprint2-0.0.17/setup.py` & `sprint2-0.0.19/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 
 setup(
     name='sprint2',
-    version='0.0.17',
+    version='0.0.19',
     packages=find_packages(),
     install_requires=[
         'argparse',
     ],
     entry_points={
         'console_scripts': [
             'MaskAGref=MaskAGref:main',
```

### Comparing `sprint2-0.0.17/sprint2.egg-info/PKG-INFO` & `sprint2-0.0.19/sprint2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.17
+Version: 0.0.19
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.17/sprint2.egg-info/SOURCES.txt` & `sprint2-0.0.19/sprint2.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 MaskAGref/MaskAGref.py
 MaskAGref/__init__.py
 getDsRNA/__init__.py
 getDsRNA/step1_transcript_blat.py
 getDsRNA/step2_transcript_dspair.py
 getDsRNA/step3_bedtools_sorted_rmLC.py
```

