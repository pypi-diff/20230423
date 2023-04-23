# Comparing `tmp/spccpkg-0.0.6.tar.gz` & `tmp/spccpkg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.6.tar", last modified: Sun Apr 23 18:21:36 2023, max compression
+gzip compressed data, was "spccpkg-0.0.7.tar", last modified: Sun Apr 23 19:29:51 2023, max compression
```

## Comparing `spccpkg-0.0.6.tar` & `spccpkg-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.818038 spccpkg-0.0.6/
--rw-rw-rw-   0        0        0      451 2023-04-23 18:21:36.817037 spccpkg-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 18:21:36.819039 spccpkg-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 18:21:33.000000 spccpkg-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.793040 spccpkg-0.0.6/spcc/
--rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.6/spcc/__init__.py
--rw-rw-rw-   0        0        0    30456 2023-04-23 18:20:11.000000 spccpkg-0.0.6/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:21:36.816038 spccpkg-0.0.6/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 18:21:36.000000 spccpkg-0.0.6/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.598322 spccpkg-0.0.7/
+-rw-rw-rw-   0        0        0      451 2023-04-23 19:29:51.596326 spccpkg-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 19:29:51.599387 spccpkg-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-23 19:27:08.000000 spccpkg-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.505311 spccpkg-0.0.7/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.7/spcc/__init__.py
+-rw-rw-rw-   0        0        0    38396 2023-04-23 19:26:44.000000 spccpkg-0.0.7/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:29:51.588359 spccpkg-0.0.7/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-23 19:29:51.000000 spccpkg-0.0.7/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 19:29:50.000000 spccpkg-0.0.7/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.6/setup.py` & `spccpkg-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

### Comparing `spccpkg-0.0.6/spcc/code.py` & `spccpkg-0.0.7/spcc/code.py`

 * *Files 17% similar despite different names*

```diff
@@ -392,14 +392,19 @@
     if (stringcheck()):
         print("String is accepted")
     else:
         print("String is not accepted")
 else:
     print("Grammar is not accepted ")
 
+    
+    #A->a
+    #A->A+A
+    #a+
+    #a+a
         '''
         print(string)
 
     def DSP1():
         string = '''
         import java.util.*;
 
@@ -983,22 +988,306 @@
             triple();
             return 0;
             }
         '''
 
         print(string)
 
+    def ICG2():
+        string = '''
+       LEX:
+
+%{
+#include"y.tab.h"
+%}
+%%
+[a-zA-Z]+ 	{strcpy(yylval.str,yytext);   return Var;}
+[0-9]+		{strcpy(yylval.str,yytext);   return Num;}
+\n		{return 0;}
+[ \t]		{}
+.		{return yytext[0];}
+%%
+int yywrap() {
+return 1;
+}
+
+
+Yacc:
+
+%{
+#include<stdio.h>
+#include<stdlib.h>
+#include<string.h>
+char * createT();
+int tempcount=0;
+%}
+%union {char str[30];}
+%left '+' 
+%left '-'
+%left '*'
+%left '/'
+%token <str> Var
+%token <str> Num
+%type  <str> s
+%type  <str> exp
+%%
+s	:	Var '=' exp	{printf("\n%s=%s\n",$1,$3);}
+exp	:	'(' exp ')' 	{strcpy($$,$2);}
+ 	|	exp '+' exp	{strcpy($$,createT()); printf("\n%s=%s+%s",$$,$1,$3);} 
+	|	exp '-' exp	{strcpy($$,createT()); printf("\n%s=%s-%s",$$,$1,$3);}
+	|	exp '*' exp	{strcpy($$,createT()); printf("\n%s=%s*%s",$$,$1,$3);}
+	|	exp '/' exp	{strcpy($$,createT()); printf("\n%s=%s/%s",$$,$1,$3);}
+	|	Num  		{strcpy($$,$1);}
+	|	Var		{strcpy($$,$1);}
+;
+%%
+char * createT() {
+	char snum[30],*ptr;			
+	sprintf(snum,"t%d",tempcount);	
+	ptr=snum;			
+	tempcount++;
+	return ptr;				
+}
+int main() {	
+yyparse(); 	
+return 0;	
+}
+int yyerror(char *err) {	
+printf("\nInvlaid");
+	exit(0);
+}
+
+
+how to run:
+flex icg.l
+bison icg.y
+bison -dy icg.y
+gcc lex.yy.c -o icg.exe
+icg.exe
+ans = (a+b)+(c*d)
+        '''
+        print(string)
+
+    def generatePT():
+        string = '''
+        # Function to generate the LL(1) parsing table
+def generate_table(grammar, start_symbol, first_sets, follow_sets):
+    # Initialize the parsing table
+    table = {}
+    for nonterminal in grammar:
+        for production in grammar[nonterminal]:
+            # Compute the FIRST set of the production
+            first_set = set()
+            for symbol in production:
+                if symbol in first_sets:
+                    first_set |= first_sets[symbol]
+                    if 'epsilon' not in first_sets[symbol]:
+                        break
+                else:
+                    first_set.add(symbol)
+                    break
+            else:
+                first_set.add('epsilon')
+            # Add entries to the parsing table based on the FIRST set
+            for terminal in first_set:
+                if terminal != 'epsilon':
+                    table[(nonterminal, terminal)] = production
+            # Add entries to the parsing table based on the FOLLOW set
+            if 'epsilon' in first_set:
+                follow_set = follow_sets[nonterminal]
+                for terminal in follow_set:
+                    table[(nonterminal, terminal)] = production
+                if '$' in follow_set:
+                    table[(nonterminal, '$')] = production
+    # Return the LL(1) parsing table
+    return table
+
+# Example usage of the generate_table function
+# Define the grammar as a dictionary of nonterminals and productions
+grammar = {
+    'S': ['A', 'b'],
+    'A': ['a', 'B'],
+    'B': ['b', 'epsilon']
+}
+# Define the start symbol of the grammar
+start_symbol = 'S'
+# Get user input for the FIRST and FOLLOW sets of the grammar
+first_sets = {}
+follow_sets = {}
+for nonterminal in grammar:
+    first = input("Enter FIRST set for " + nonterminal + ": ")
+    first_sets[nonterminal] = set(first.split())
+    follow = input("Enter FOLLOW set for " + nonterminal + ": ")
+    follow_sets[nonterminal] = set(follow.split())
+# Generate the LL(1) parsing table
+table = generate_table(grammar, start_symbol, first_sets, follow_sets)
+# Print the LL(1) parsing table
+print("LL(1) Parsing Table:")
+print("{:<10}".format(""), end="")
+for terminal in first_sets[start_symbol] | {'$'}:
+    print("{:<10}".format(terminal), end="")
+print()
+for nonterminal in grammar:
+    print("{:<10}".format(nonterminal), end="")
+    for terminal in first_sets[start_symbol] | {'$'}:
+        if (nonterminal, terminal) in table:
+            production = " ".join(table[(nonterminal, terminal)])
+            print("{:<10}".format(production), end="")
+        else:
+            print("{:<10}".format(""), end="")
+    print()
+
+
+How to execute:
+Enter FIRST set for S: a b
+Enter FOLLOW set for S: $
+Enter FIRST set for A: a
+Enter FOLLOW set for A: b $
+Enter FIRST set for B: b epsilon
+Enter FOLLOW set for B: a $
+
+Output:
+LL(1) Parsing Table:
+          a         b         $
+S         A         b
+A         a         B         epsilon
+B                   b         epsilon
+        '''
+        print(string)
+    
+    def P1macro():
+        string = '''
+        mntc = 1
+mdtc = 1
+ala_counter = 1
+ala_set = set()
+ala = {}
+mnt = []
+mdt = {}
+mystring = ''
+file = open('macro.txt')
+list_program = list(file)
+file.close()
+file = open('macro.txt', 'r+')
+program = file.read()
+words = program.split()
+for i in range(len(words)):
+    if words[i] == "MACRO":
+        index = i
+        # ALA
+        for i in range(index + 1, len(words)):
+            if words[i].startswith("&") and words[i] not in ala_set:
+                ala_set.add(words[i])
+                ala[ala_counter] = words[i]
+                ala_counter+=1
+                
+for i in range(len(list_program)):
+    if list_program[i] == "MACRO\n":
+        mnt.append(mntc)
+        line_split = list_program[i+1].split()
+        mnt.append(line_split[1])
+        mnt.append(mdtc)
+        mntc+=1
+        macro_define_index = i + 2
+        mdt[mdtc] = list_program[i+1]
+        mdtc+=1
+        for j in range(macro_define_index, len(list_program)):
+            line_split = list_program[j].split()
+            for k in range(len(line_split)):
+                if line_split[k] in ala_set:
+                    for index in range(1, len(ala_set)+1):
+                          value = ala.get(index)
+                          if value == line_split[k]:
+                              temp = index
+                              break
+                    line_split[k] = '#' + str(temp)
+            mdt[mdtc] = line_split
+            mdtc+=1
+            
+print("ALA\nIndex\tArgument")
+for i in range(1, len(ala)+1):
+    print(i, "\t", ala.get(i))
+    
+print("\n\nMNT\nIndex\tMacro Name  MDT Index")
+for i in range (len(mnt)):
+    print(mnt[i],"\t   ", end="")
+    
+print("\n\nMDT\nIndex\tCard")
+for i in range (1, len(mdt)+1):
+    print(i,"\t", mdt.get(i))
+
+
+macro.txt:
+
+START
+    MACRO
+    INCR1 &A, &B
+    ADD &A, 1
+    ADD &B, 1
+    MEND
+    CALL INCR1, &FIRST, &SECOND
+    END
+        '''
+        print(string)
+    
+    def P2macro():
+        string = '''
+        MDT = []  # Macro Definition Table
+MNT = {}  # Macro Name Table
+ALA = {}  # Argument List Array
+
+# Read MDT, MNT, and ALA from files generated in pass-1
+with open('MDT.txt', 'r') as f:
+    for line in f:
+        MDT.append(line.strip().split())
+        
+with open('MNT.txt', 'r') as f:
+    for line in f:
+        name, index = line.strip().split()
+        MNT[name] = int(index)
+        
+with open('ALA.txt', 'r') as f:
+    for line in f:
+        index, arg = line.strip().split()
+        ALA[int(index)] = arg
+
+# Read input file
+with open('input.txt', 'r') as f:
+    for line in f:
+        line = line.strip()
+        if line in MNT:  # Macro call
+            mdt_index = MNT[line]
+            ala_index = 1
+            for i in range(mdt_index, len(MDT)):
+                card = MDT[i]
+                if card[0] == 'MEND':
+                    break
+                for j in range(1, len(card)):
+                    if card[j][0] == '&':
+                        card[j] = ALA[int(card[j][1:])]
+                    else:
+                        card[j] = card[j]
+                print('\t'.join(card))
+        else:  # Non-macro instruction
+            print(line)
+        '''
+        print(string)
+
     def main():
         string = '''
+        lexical()
+        flex()
+        ff()
+        generatePT()
+        PP()
+        OP()
+        yacc()
         ICG()
+        ICG2()
         commands()
-        yacc()
-        macro()
-        P2()
         DSP1()
-        OP()
-        flex()
-        PP()
-        lexical()
-        ff()
+        P2()
+        macro()
+        P1macro()
+        P2macro()
         '''
         print(string)
```

