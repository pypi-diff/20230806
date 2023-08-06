# Comparing `tmp/kukie-4.0.0.tar.gz` & `tmp/kukie-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kukie-4.0.0.tar", last modified: Sun Aug  6 13:46:00 2023, max compression
+gzip compressed data, was "kukie-5.0.0.tar", last modified: Sun Aug  6 16:20:22 2023, max compression
```

## Comparing `kukie-4.0.0.tar` & `kukie-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 13:46:00.071239 kukie-4.0.0/
--rw-rw-rw-   0        0        0      499 2023-08-06 13:46:00.070239 kukie-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-08-02 16:31:39.000000 kukie-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 13:46:00.057320 kukie-4.0.0/kukie/
-drwxrwxrwx   0        0        0        0 2023-08-06 13:46:00.068239 kukie-4.0.0/kukie/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 13:46:00.067232 kukie-4.0.0/kukie/src/kukie.egg-info/
--rw-rw-rw-   0        0        0      499 2023-08-06 13:46:00.000000 kukie-4.0.0/kukie/src/kukie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-06 13:46:00.000000 kukie-4.0.0/kukie/src/kukie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 13:46:00.000000 kukie-4.0.0/kukie/src/kukie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-06 13:46:00.000000 kukie-4.0.0/kukie/src/kukie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    66774 2023-08-06 13:45:20.000000 kukie-4.0.0/kukie/src/kukie.py
--rw-rw-rw-   0        0        0       42 2023-08-06 13:46:00.071239 kukie-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-08-06 13:45:53.000000 kukie-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:20:22.173628 kukie-5.0.0/
+-rw-rw-rw-   0        0        0      499 2023-08-06 16:20:22.171628 kukie-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-08-02 16:31:39.000000 kukie-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 16:20:22.143622 kukie-5.0.0/kukie/
+drwxrwxrwx   0        0        0        0 2023-08-06 16:20:22.167627 kukie-5.0.0/kukie/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 16:20:22.162627 kukie-5.0.0/kukie/src/kukie.egg-info/
+-rw-rw-rw-   0        0        0      499 2023-08-06 16:20:22.000000 kukie-5.0.0/kukie/src/kukie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-06 16:20:22.000000 kukie-5.0.0/kukie/src/kukie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 16:20:22.000000 kukie-5.0.0/kukie/src/kukie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-06 16:20:22.000000 kukie-5.0.0/kukie/src/kukie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    68705 2023-08-06 15:51:35.000000 kukie-5.0.0/kukie/src/kukie.py
+-rw-rw-rw-   0        0        0       42 2023-08-06 16:20:22.173628 kukie-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-08-06 16:19:37.000000 kukie-5.0.0/setup.py
```

### Comparing `kukie-4.0.0/kukie/src/kukie.py` & `kukie-5.0.0/kukie/src/kukie.py`

 * *Files 2% similar despite different names*

```diff
@@ -561,15 +561,15 @@
 CQdata ={
 1:
 '''
 WACP to illustrate Command-Line Arguments.
 ''',
 2:
 '''
-WACP to illustrate the user-defined data type student.
+WACP to illustrate the user-defined data type student with union
 ''',
 3:
 '''
 WACP to read the content of a given text file and count the number of characters, words and lines in it.
 
 ''',
 4:
@@ -654,14 +654,23 @@
 '''
 Write a C Program to implement Depth  First Traversal of a Graph.
 ''',
 22:
 '''
 Write a C Program to Calculate complex numbers
 ''',
+23:
+'''
+WAP to create user defined datatype student with struct
+
+''',
+24:
+'''
+union program
+'''
 
 }
 
 
 
 
 
@@ -2253,16 +2262,16 @@
         printf("\\n");
     }
 }
     
 ''',
 15:
 '''
-#include< stdio.h>
-#include< stdlib.h>
+#include<stdio.h>
+#include<stdlib.h>
 #define MAX_CAPACITY 10
 int queue[MAX_CAPACITY];
 int front=-1,rear=-1;
 void enQueue();
 void deQueue();
 void display();
 int isfull()
@@ -2333,16 +2342,16 @@
         printf("\\n");
     }
 }
     
 ''',
 16:
 '''
-#include< stdio.h>
-#include< stdlib.h>
+#include<stdio.h>
+#include<stdlib.h>
 struct node{
     int data;
     struct node *next;
 };
 struct node *front=NULL;
 struct node *rear=NULL;
 void enQueue();
@@ -2421,16 +2430,16 @@
         printf("\\n");
     }
 }
     
 ''',
 17:
 '''
-#include< stdio.h>
-#include< stdlib.h>
+#include<stdio.h>
+#include<stdlib.h>
 #define size 8
 int queue[size];
 int front=-1,rear=-1;
 void enQueue();
 void deQueue();
 void display();
  void main()
@@ -2522,15 +2531,15 @@
          }
      }
  }
     
 ''',
 18:
 '''
-#include< stdio.h>
+#include<stdio.h>
 #define MAX_SIZE 20
 char stk[20];
 int top=-1;
 int isEmpty()
 {
     return top==-1;
 }
@@ -2606,30 +2615,30 @@
             while(!isEmpty() && precedence(expression[i])<=precedence(peek()))
                 expression[++j]=pop();
             push(expression[i]);
         }
     }
     while(!isEmpty())
         expression[++j]=pop();
-    expression[++j]='\0';
+    expression[++j]='\\0';
     printf("%s\\n",expression);
 }
 int main()
 {
     char expression[MAX_SIZE];
     printf("Enter expression:");
     scanf("%[^\\n]s",expression);
     convertinfixtopostfix(expression);
     return 0;
 }
             
 ''',
 19:
 '''
-#include< stdio.h>
+#include<stdio.h>
 int stack[20];
 int top = -1;
 
 void push(int x)
 {
     stack[++top] = x;
 }
@@ -2643,15 +2652,15 @@
 {
     char exp[20];
     char *e;
     int n1,n2,n3,num;
     printf("Enter the expression :: ");
     scanf("%s",exp);
     e = exp;
-    while(*e != '\0')
+    while(*e != '\\0')
     {
         if(isdigit(*e))
         {
             num = *e - 48;
             push(num);
         }
         else
@@ -2842,14 +2851,75 @@
  default:
  printf("Wrong choice\\n");
 break;
 }
 }
  return 0;
 }
+''',
+23:
+'''
+#include < stdio.h>
+            struct date
+            {
+                int dd,mm,yyyy;
+            };
+            struct student
+            {
+                int roll;
+                char name[50];
+                struct date dob;
+            };
+            int main()
+            {
+                int i,n;
+                printf("Enter no.of Students:");
+                scanf("%d",&n);
+                struct student st[n];
+                for(i=0;i < n;i++)
+                {
+                    printf("Enter the info of student[%d]:\\n",i+1);
+                    printf("Enter Roll No.:");
+                    scanf("%d",&st[i].roll);
+                    printf("Enter Name:");
+                    scanf("%s",st[i].name);
+                    printf("Enter DOB(dd,mm,yyyy):");
+                    scanf("%d %d %d",&st[i].dob.dd,&st[i].dob.mm,&st[i].dob.yyyy);
+                }
+                printf("DISPLAYING INFO\\n");
+                for(i=0;i < n;i++)
+                {
+                    printf("Info of Student[%d]\\n",i+1);
+                    printf("Name:%s\\n",st[i].name);
+                    printf("Roll no:%d\\n",st[i].roll);
+                    printf("DOB:%d %d %d\\n",st[i].dob.dd,st[i].dob.mm,st[i].dob.yyyy);
+                }
+            return 0;
+            }
+''',
+24:
+'''
+    #include< stdio.h>
+        #include< string.h>
+        union data{
+        int i;
+        float f;
+        char a[20];
+        };
+        int main()
+        {
+            union data d;
+            d.i=10;
+            printf("data.i=%d\\n",d.i);
+            d.f=20.5;
+            printf("data.f=%f\\n",d.f);
+            strcpy(d.a,"hello");
+            printf("data.a=%s\\n",d.a);
+            return 0;
+}
 '''
 
 }
 
 
 
 
@@ -2876,15 +2946,15 @@
 def verify():
     password = 'rikee'
     while True:
         inpass= input('enter password >>>')
         if password==inpass:
             break
         else:
-            print('\naa kurchi madathapetti...\n')
+            print('\nProgram Elago Radhu ,Kanisam Password ayina Telvali gaa.\n')
             continue
 
 
 
 def write_file(filename, content):
     try:
         with open(filename, 'w') as file:
```

### Comparing `kukie-4.0.0/setup.py` & `kukie-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kukie",                     # This is the name of the package
-    version="4.0.0",                        # The initial release version
+    version="5.0.0",                        # The initial release version
     author="TonyStark",                     # Full name of the author
     description="HAPPY HEIST",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

