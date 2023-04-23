# Comparing `tmp/sprint2-0.0.19.tar.gz` & `tmp/sprint2-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprint2-0.0.19.tar", last modified: Sun Apr 23 17:15:15 2023, max compression
+gzip compressed data, was "sprint2-0.1.tar", last modified: Sun Apr 23 21:03:52 2023, max compression
```

## Comparing `sprint2-0.0.19.tar` & `sprint2-0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.339593 sprint2-0.0.19/
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:20.904630 sprint2-0.0.19/MaskAGref/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6762 2023-04-23 13:54:07.000000 sprint2-0.0.19/MaskAGref/MaskAGref.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-23 13:54:07.000000 sprint2-0.0.19/MaskAGref/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-23 17:15:21.337593 sprint2-0.0.19/PKG-INFO
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     8510 2023-04-23 13:54:07.000000 sprint2-0.0.19/README.md
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.058617 sprint2-0.0.19/getDsRNA/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1922 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9630 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step1_transcript_blat.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step2_transcript_dspair.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     3241 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step3_bedtools_sorted_rmLC.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     6815 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step4_combine_by_chr.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     5815 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step5_merge_dsRNA.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     2450 2023-04-23 13:54:07.000000 sprint2-0.0.19/getDsRNA/step6_dsRNA.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.194605 sprint2-0.0.19/getRES/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     7678 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/__init__.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    45394 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step1_SNVcalling.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    21192 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step2_annotation_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)    17443 2023-04-23 13:54:07.000000 sprint2-0.0.19/getRES/step3_dsRNA_based.py
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-23 17:15:21.340592 sprint2-0.0.19/setup.cfg
--rw-rw-r--   0 xyx       (1003) xyx       (1003)     1096 2023-04-23 13:54:08.000000 sprint2-0.0.19/setup.py
-drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 17:15:21.330593 sprint2-0.0.19/sprint2.egg-info/
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      621 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/PKG-INFO
--rw-rw-r--   0 xyx       (1003) xyx       (1003)      575 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/SOURCES.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/dependency_links.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/entry_points.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/requires.txt
--rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-23 17:15:19.000000 sprint2-0.0.19/sprint2.egg-info/top_level.txt
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 21:03:57.566022 sprint2-0.1/
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 21:03:57.291046 sprint2-0.1/MaskAGref/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6764 2023-04-23 21:02:55.000000 sprint2-0.1/MaskAGref/MaskAGref.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       24 2023-04-23 21:02:55.000000 sprint2-0.1/MaskAGref/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      618 2023-04-23 21:03:57.563023 sprint2-0.1/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     8510 2023-04-23 21:02:59.000000 sprint2-0.1/README.md
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 21:03:57.373039 sprint2-0.1/getDsRNA/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1925 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9630 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step1_transcript_blat.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     9835 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step2_transcript_dspair.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     3243 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step3_bedtools_sorted_rmLC.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     6816 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step4_combine_by_chr.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     5816 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step5_merge_dsRNA.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     2450 2023-04-23 21:02:39.000000 sprint2-0.1/getDsRNA/step6_dsRNA.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 21:03:57.442033 sprint2-0.1/getRES/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     7897 2023-04-23 21:02:42.000000 sprint2-0.1/getRES/__init__.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    45423 2023-04-23 21:02:42.000000 sprint2-0.1/getRES/step1_SNVcalling.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    21228 2023-04-23 21:02:42.000000 sprint2-0.1/getRES/step2_annotation_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)    17444 2023-04-23 21:02:42.000000 sprint2-0.1/getRES/step3_dsRNA_based.py
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       38 2023-04-23 21:03:57.567022 sprint2-0.1/setup.cfg
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)     1093 2023-04-23 21:03:06.000000 sprint2-0.1/setup.py
+drwxrwxr-x   0 xyx       (1003) xyx       (1003)        0 2023-04-23 21:03:57.556023 sprint2-0.1/sprint2.egg-info/
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      618 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/PKG-INFO
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)      575 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/SOURCES.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        1 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/dependency_links.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       90 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/entry_points.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)        9 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/requires.txt
+-rw-rw-r--   0 xyx       (1003) xyx       (1003)       26 2023-04-23 21:03:56.000000 sprint2-0.1/sprint2.egg-info/top_level.txt
```

### Comparing `sprint2-0.0.19/MaskAGref/MaskAGref.py` & `sprint2-0.1/MaskAGref/MaskAGref.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,18 @@
     step=subprocess.Popen(bwa+' index -a bwtsw '+fa_in_dir,shell=True)
     step.wait()
 
 ##----------------------------------------------------------------------------------------------------------
 
 def main(): 
     parser = argparse.ArgumentParser(description='Mask A with G on reference FASTA file.')
-    parser.add_argument('-r', '--reference',default = str(os.getcwd())+"reference.fa",  help='path to reference FASTA file (default:~/reference.fa)')
+    parser.add_argument('-r', '--reference',default = str(os.getcwd())+"/reference.fa",  help='path to reference FASTA file (default:~/reference.fa)')
     parser.add_argument('-o', '--output',default = str(os.getcwd()),  help='path to output directory (default:~/)')
     parser.add_argument('-t', '--gtf',  help='path to transcript annotation GTF file #Optional')
-    parser.add_argument('-b', '--bwa',default = str(os.getcwd())+"bwa",  help='path to bwa (default:~/bwa)')
+    parser.add_argument('-b', '--bwa',default = str(os.getcwd())+"/bwa",  help='path to bwa (default:~/bwa)')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
 
     try:
         args = parser.parse_args()
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
```

### Comparing `sprint2-0.0.19/PKG-INFO` & `sprint2-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.19
+Version: 0.1
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.19/README.md` & `sprint2-0.1/README.md`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.19/getDsRNA/__init__.py` & `sprint2-0.1/getDsRNA/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 
 def run():
     parser = argparse.ArgumentParser(description='Get candidate double-stranded RNA')
     parser.add_argument('-o', '--OUT_DIR',default = str(os.getcwd()),  help='path to output directory (default:~/)')
     parser.add_argument('-r', '--Reference_file', help='path to reference FASTA file (default:~/reference.fa)')
     parser.add_argument('-t', '--Transcript_file',  help='path to transcript annotation bed file (default:~/transcript.bed)')
-    parser.add_argument('-b', '--Blat_file',default = str(os.getcwd())+"blat",  help='path to blat (default:~/blat)')
-    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"bedtools",  help='path to bedtools (default:~/bedtools)')
-    parser.add_argument('-lc', '--lc_path',default = str(os.getcwd())+"Low_complex.txt",  help='path to output Low_complex.txt (default:~/Low_complex.txt)')
+    parser.add_argument('-b', '--Blat_file',default = str(os.getcwd())+"/blat",  help='path to blat (default:~/blat)')
+    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"/bedtools",  help='path to bedtools (default:~/bedtools)')
+    parser.add_argument('-lc', '--lc_path',default = str(os.getcwd())+"/Low_complex.txt",  help='path to output Low_complex.txt (default:~/Low_complex.txt)')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
     args = parser.parse_args()
 
     step1_transcript_blat.main("-o "+args.OUT_DIR+" -r "+args.Reference_file+" -t "+args.Transcript_file+" -b "+args.Blat_file+" -p "+args.cpu)
     step2_transcript_dspair.main("-o "+args.OUT_DIR+" -t "+args.Transcript_file+" -p "+args.cpu)
     step3_bedtools_sorted_rmLC.main("-o "+args.OUT_DIR+" -B "+args.Bedtools_path+" -lc "+args.lc_path+" -p "+args.cpu)
     step4_combine_by_chr.main("-o "+args.OUT_DIR+" -B "+ args.Bedtools_path+" -t "+args.Transcript_file+" -p "+args.cpu)
```

### Comparing `sprint2-0.0.19/getDsRNA/step1_transcript_blat.py` & `sprint2-0.1/getDsRNA/step1_transcript_blat.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.19/getDsRNA/step2_transcript_dspair.py` & `sprint2-0.1/getDsRNA/step2_transcript_dspair.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.19/getDsRNA/step3_bedtools_sorted_rmLC.py` & `sprint2-0.1/getDsRNA/step3_bedtools_sorted_rmLC.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     rmLC_path=ARG[1]
     subprocess.Popen(bedtools_path + " pairtobed -a "+sorted_path +" -b "+lc_path+" -f 0.5 -type neither > "+rmLC_path,shell=True).wait()
 ##----------------------------------------------------------------------------------------------------------
 
 def main(args):    
     parser = argparse.ArgumentParser(description='python3 step3_bedtools_sorted_rmLC.py')
     parser.add_argument('-o', '--OUT_DIR',default = str(os.getcwd()),  help='path to Output Directory (default:Working Directory)')
-    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
-    parser.add_argument('-lc', '--lc_path',default = str(os.getcwd())+"Low_complexity.txt",  help='path to Low_complexity file (default:~/Low_complexity.txt)')
+    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"/bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
+    parser.add_argument('-lc', '--lc_path',default = str(os.getcwd())+"/Low_complexity.txt",  help='path to Low_complexity file (default:~/Low_complexity.txt)')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
```

### Comparing `sprint2-0.0.19/getDsRNA/step4_combine_by_chr.py` & `sprint2-0.1/getDsRNA/step4_combine_by_chr.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 ##----------------------------------------------------------------------------------------------------------
 def main(args):    
     print("Start step4 combine_by_chr...")     
     parser = argparse.ArgumentParser(description='python3 step4_combine_by_chr.py')
     parser.add_argument('-o', '--OUT_DIR',default = str(os.getcwd()),  help='path to Output Directory (default:Working Directory)')
     parser.add_argument('-t','--Transcript_file',default = str(os.getcwd())+"/transcript.bed", help='path to Transctript Annotation File (BED format) (default:~/transcript.bed)')
-    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
+    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"/bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
 
     try:
         args = parser.parse_args(args.split())
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
```

### Comparing `sprint2-0.0.19/getDsRNA/step5_merge_dsRNA.py` & `sprint2-0.1/getDsRNA/step5_merge_dsRNA.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ##----------------------------------------------------------------------------------------------------------
 
 
 ##----------------------------------------------------------------------------------------------------------
 def main(args):
     parser = argparse.ArgumentParser(description='python3 step5_merge_dsRNA.py')
     parser.add_argument('-o', '--OUT_DIR',default = str(os.getcwd()),  help='path to Output Directory (default:Working Directory)')
-    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
+    parser.add_argument('-B', '--Bedtools_path',default = str(os.getcwd())+"/bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
```

### Comparing `sprint2-0.0.19/getDsRNA/step6_dsRNA.py` & `sprint2-0.1/getDsRNA/step6_dsRNA.py`

 * *Files identical despite different names*

### Comparing `sprint2-0.0.19/getRES/__init__.py` & `sprint2-0.1/getRES/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,27 +56,31 @@
     for i in range(len(all_num)):
         this_line=str(all_type[i])+"\t"+str(all_num[i])+"\t"+str(all_ratio[i])+"\n"
         fo.write(this_line)
     fo.close()
 ##----------------------------------------------------------------------------------------------------------
 
 def getBedDP(bed_in_path=0, bam_in_path=0, bed_out_path=0, bedtools_path=0):
-    this_step =subprocess.Popen(' '.join([bedtools_path,'multicov','-bams',bam_in_path,'-bed',bed_in_path,'| sed -i "s/\b0\b/1/g" >',bed_out_path]),shell=True)
-    this_step.wait()
+    this_step1 = subprocess.Popen(' '.join([bedtools_path,'multicov','-bams',bam_in_path,'-bed',bed_in_path,' >',bed_out_path+"_hp"]),shell=True)
+    this_step1.wait()
+    this_step2 = subprocess.Popen('| sed -i "s/\b0\b/1/g" '+bed_out_path+"_hp"+' > '+bed_out_path,shell=True)
+    this_step2.wait()
+    this_step3 = subprocess.Popen('rm '+bed_out_path+"_hp",shell=True)
+    this_step3.wait()
 def run():
     parser = argparse.ArgumentParser(description='Get candidate double-stranded RNA')
     parser.add_argument('-s', '--SNV_PATH',default = str(os.getcwd())+"/1_SNV_calling/",  help='path to SNV directory (default:~/1_SNV_calling/)')
     parser.add_argument('-o', '--RES_PATH',default = str(os.getcwd())+"/2_RES_calling/",  help='path to output directory (default:~/2_RES_calling/)')
     parser.add_argument('-r1', '--read1',default = str(os.getcwd())+"/test_1.fastq", help='path to sample FASTQ_1 file (default:~/test_1.fastq)')
     parser.add_argument('-r2', '--read2', help='path to reference FASTQ_2 file #Optional')
     parser.add_argument('-r', '--Reference_file',default = str(os.getcwd())+"/reference.fa", help='path to reference FASTA file (default:~/reference.fa)')
     parser.add_argument('-rp', '--Repeat_file',  help='path to repeat BED file #Optional')
-    parser.add_argument('-b', '--bwa',default = str(os.getcwd())+"bwa",  help='path to BWA (default:~/bwa)')
-    parser.add_argument('-B', '--bedtools',default = str(os.getcwd())+"bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
-    parser.add_argument('-S', '--samtools',default = str(os.getcwd())+"samtools",  help='path to SAMTOOLS (default:~/samtools)')
+    parser.add_argument('-b', '--bwa',default = str(os.getcwd())+"/bwa",  help='path to BWA (default:~/bwa)')
+    parser.add_argument('-B', '--bedtools',default = str(os.getcwd())+"/bedtools",  help='path to BEDTOOLS (default:~/bedtools)')
+    parser.add_argument('-S', '--samtools',default = str(os.getcwd())+"/samtools",  help='path to SAMTOOLS (default:~/samtools)')
     parser.add_argument('-ds', '--Candidate_dsRNA',  help='path to candidate dsRNA directory #Optional')
     parser.add_argument('-p', '--cpu',default=1,  help='CPU number (default=1)')
     args = parser.parse_args()
 
     if args.read2:
         step1_SNVcalling.main("-o "+args.SNV_PATH+" -r1 "+args.read1+" -r2 "+args.read2+" -R "+args.Reference_file+" -b "+args.bwa+" -B "+args.bedtools+" -s "+args.samtools+" -p "+args.cpu)
     else:
```

### Comparing `sprint2-0.0.19/getRES/step1_SNVcalling.py` & `sprint2-0.1/getRES/step1_SNVcalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,20 +747,20 @@
 
 
 ##----------------------------------------------------------------------------------------------------------
 def main(args):
 
     parser = argparse.ArgumentParser(description="python3 step1_SNVcalling.py")
     parser.add_argument("-o", "--output",default = str(os.getcwd()),  help="path to Output Directory (defalt:Working Directory)")
-    parser.add_argument("-r1", "--read1",default = str(os.getcwd())+"test_1.fastq",  help="path to read1.fastq (defalt:~/test_1.fastq)")
+    parser.add_argument("-r1", "--read1",default = str(os.getcwd())+"/test_1.fastq",  help="path to read1.fastq (defalt:~/test_1.fastq)")
     parser.add_argument("-r2", "--read2",  help="path to read2.fastq ##optional")
-    parser.add_argument("-R", "--reference",default = str(os.getcwd())+"reference.fa",  help="path to reference FASTA file (defalt:~/reference.fa)")
-    parser.add_argument("-b", "--bwa",default = str(os.getcwd())+"bwa",  help="path to BWA (defalt:~/bwa)")
-    parser.add_argument("-B", "--bedtools",default = str(os.getcwd())+"bedtools",  help="path to BEDTOOLS ((defalt:~/bedtools)")
-    parser.add_argument("-s", "--samtools",default = str(os.getcwd())+"samtools",  help="path to SAMTOOLS  ((defalt:~/samtools)")
+    parser.add_argument("-R", "--reference",default = str(os.getcwd())+"/reference.fa",  help="path to reference FASTA file (defalt:~/reference.fa)")
+    parser.add_argument("-b", "--bwa",default = str(os.getcwd())+"/bwa",  help="path to BWA (defalt:~/bwa)")
+    parser.add_argument("-B", "--bedtools",default = str(os.getcwd())+"/bedtools",  help="path to BEDTOOLS ((defalt:~/bedtools)")
+    parser.add_argument("-s", "--samtools",default = str(os.getcwd())+"/samtools",  help="path to SAMTOOLS  ((defalt:~/samtools)")
     parser.add_argument("-p", "--cpu",default=1,  help="CPU number (defalt=1)")
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
@@ -934,23 +934,23 @@
     print("SNV calling running time is:" + run_time + " seconds" + "\n")        
 
     ##----------------------------------------------------------------------------------------------------------
 
     if os.path.exists(refgenome+".trans.fa"):
         subprocess.Popen("cat "+tmp+"/transcript_all_ad.snv.genome.snv.dedup.snv "+tmp+"/genome_all_ad.snv.dedup | uniq | bedtools sort -i > "+tmp+"/regular.snv",shell=True).wait()
         subprocess.Popen("cat "+tmp+"/transcript_mskTC_all_ad.snv.genome.snv.dedup.snv "+tmp+"/genome_mskTC_all_ad.snv.dedup | uniq | bedtools sort -i > "+tmp+"/hyper_mskTC.snv",shell=True).wait()
-        subprocess.Popen("cat "+tmp+"/transcript_mskAG_all_ad.snv.genome.snv.dedup.snv "+tmp+"/genome_mskAG_all_ad.snv.dedup | uniq | bedtools sort -i > "+tmp+"/hyper_mskAG.snv",shell=True).wait()
+        subprocess.Popen("cat "+tmp+"/transcript_mskAG_all_ad.snv.genome.snv.dedup.snv "+tmp+"/genome_mskAG_all_ad.snv.dedup | uniq | bedtools sort -i > "+tmp+"/hyper_mskAG.snv",shell=True).wait()    
+        subprocess.Popen("mv "+tmp+"/transcript_mskAG_* "+tmp+"/transcript_mskAG/",shell=True).wait()    
+        subprocess.Popen("mv "+tmp+"/transcript_mskTC_* "+tmp+"/transcript_mskTC/",shell=True).wait()    
+        subprocess.Popen("mv "+tmp+"/regular_unmap* "+tmp+"/transcript/",shell=True).wait()        
+        subprocess.Popen("mv "+tmp+"/transcript_*.* "+tmp+"/transcript/",shell=True).wait()
+
     else:
         subprocess.Popen("cp "+tmp+"/genome_all_ad.snv.dedup "+tmp+"/regular.snv",shell=True).wait()
         subprocess.Popen("cp "+tmp+"/genome_mskTC_all_ad.snv.dedup "+tmp+"/hyper_mskTC.snv",shell=True).wait()
         subprocess.Popen("cp "+tmp+"/genome_mskAG_all_ad.snv.dedup "+tmp+"/hyper_mskAG.snv",shell=True).wait()
-
-    subprocess.Popen("mv "+tmp+"/genome_mskAG_* "+tmp+"/genome_mskAG/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/genome_mskTC_* "+tmp+"/genome_mskTC/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/transcript_mskAG_* "+tmp+"/transcript_mskAG/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/transcript_mskTC_* "+tmp+"/transcript_mskTC/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/regular_unmap* "+tmp+"/transcript/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/genome_*.* "+tmp+"/genome/",shell=True).wait()    
-    subprocess.Popen("mv "+tmp+"/transcript_*.* "+tmp+"/transcript/",shell=True).wait()    
+        subprocess.Popen("mv "+tmp+"/genome_mskAG_* "+tmp+"/genome_mskAG/",shell=True).wait()    
+        subprocess.Popen("mv "+tmp+"/genome_mskTC_* "+tmp+"/genome_mskTC/",shell=True).wait()
+        subprocess.Popen("mv "+tmp+"/genome_*.* "+tmp+"/genome/",shell=True).wait()
 ##----------------------------------------------------------------------------------------------------------
```

### Comparing `sprint2-0.0.19/getRES/step2_annotation_based.py` & `sprint2-0.1/getRES/step2_annotation_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,16 +439,16 @@
 
 
 ##----------------------------------------------------------------------------------------------------------
 
 def main(args):
 
     parser = argparse.ArgumentParser(description="python3 step2_annotation_based.py")
-    parser.add_argument("-o", "--output",default = str(os.getcwd()),  help="path to Output Directory (defalt:Working Directory)")
-    parser.add_argument("-s", "--snv",default = str(os.getcwd()),  help="path to SNV Directory (defalt:Working Directory)")
+    parser.add_argument("-o", "--output",default = str(os.getcwd())+"/2_RES_calling/",  help="path to Output Directory (defalt:Working Directory)")
+    parser.add_argument("-s", "--snv",default = str(os.getcwd())+"/1_SNV_calling/",  help="path to SNV Directory (defalt:Working Directory)")
     parser.add_argument("-rp", "--repeat",help="path to repeat file #Optional")
 
     try:
         args = parser.parse_args(args.split())
 
     except argparse.ArgumentError as e:
         print(e)
```

### Comparing `sprint2-0.0.19/getRES/step3_dsRNA_based.py` & `sprint2-0.1/getRES/step3_dsRNA_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 ##----------------------------------------------------------------------------------------------------------
 def main(args):
 
     parser = argparse.ArgumentParser(description="python3 step3_dsRNA_based.py")
     parser.add_argument("-o", "--output",default = str(os.getcwd()),  help="path to Output Directory (defalt:Working Directory)")
     parser.add_argument("-s", "--snv",default = str(os.getcwd()),  help="path to SNV Directory (defalt:Working Directory)")
     parser.add_argument("-ds", "--dsrna",default = str(os.getcwd())+"/dsRNA_file/",  help="path to candidate dsRNA Directory (defalt:~/dsRNA_file/)")
-    parser.add_argument("-b", "--bedtools",default = str(os.getcwd())+"bedtools",  help="path to bedtools (defalt:~/bedtools)")
+    parser.add_argument("-b", "--bedtools",default = str(os.getcwd())+"/bedtools",  help="path to bedtools (defalt:~/bedtools)")
     parser.add_argument("-p", "--cpu",default = 1,  help="CPU number (defalt=1)")
 
     try:
         args = parser.parse_args(args.split())
     except argparse.ArgumentError as e:
         print(e)
         exit(1)
```

### Comparing `sprint2-0.0.19/setup.py` & `sprint2-0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 
 setup(
     name='sprint2',
-    version='0.0.19',
+    version='0.1',
     packages=find_packages(),
     install_requires=[
         'argparse',
     ],
     entry_points={
         'console_scripts': [
             'MaskAGref=MaskAGref:main',
```

### Comparing `sprint2-0.0.19/sprint2.egg-info/PKG-INFO` & `sprint2-0.1/sprint2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprint2
-Version: 0.0.19
+Version: 0.1
 Summary: SPRINT-2.0: An enhanced tool to identify RNA editing sites
 Home-page: https://github.com/xieyunxiao/SPRINT2
 Author: Feng Zhang, Yunxiao Xie
 Author-email: 20210700107@fudan.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sprint2-0.0.19/sprint2.egg-info/SOURCES.txt` & `sprint2-0.1/sprint2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

