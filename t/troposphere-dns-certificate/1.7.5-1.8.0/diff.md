# Comparing `tmp/troposphere-dns-certificate-1.7.5.tar.gz` & `tmp/troposphere-dns-certificate-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troposphere-dns-certificate-1.7.5.tar", last modified: Mon Feb  6 20:10:07 2023, max compression
+gzip compressed data, was "troposphere-dns-certificate-1.8.0.tar", last modified: Sun Apr 23 17:55:03 2023, max compression
```

## Comparing `troposphere-dns-certificate-1.7.5.tar` & `troposphere-dns-certificate-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 20:10:07.366507 troposphere-dns-certificate-1.7.5/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12727 2023-02-06 20:10:07.362507 troposphere-dns-certificate-1.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12251 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-06 20:10:07.366507 troposphere-dns-certificate-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      930 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 20:10:07.362507 troposphere-dns-certificate-1.7.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 20:10:07.362507 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/
--rw-r--r--   0 root         (0) root         (0)      916 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/certificate.py
--rw-r--r--   0 root         (0) root         (0)     6077 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/certificatemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 20:10:07.362507 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12727 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-06 20:10:07.000000 troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 20:10:07.362507 troposphere-dns-certificate-1.7.5/test/
--rw-r--r--   0 root         (0) root         (0)      417 2023-02-06 20:09:59.000000 troposphere-dns-certificate-1.7.5/test/test_lambda_code_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12939 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.205051 troposphere-dns-certificate-1.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12595 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificate.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificatemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/test/
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/test/test_lambda_code_size.py
```

### Comparing `troposphere-dns-certificate-1.7.5/LICENSE` & `troposphere-dns-certificate-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troposphere-dns-certificate-1.7.5/PKG-INFO` & `troposphere-dns-certificate-1.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: troposphere-dns-certificate
-Version: 1.7.5
-Summary: Cloudformation DNS validated certificate resource for troposphere
-Home-page: https://github.com/dflook/cloudformation-dns-certificate
-Author: Daniel Flook
-Author-email: daniel@flook.org
-License: MIT
-Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
-Keywords: cloudformation troposphere certificate
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cloudformation DNS Validated Certificate Resource
 
 This is a cloudformation custom resource which is an enhancement of the [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html) resource.
 
 It allows creating a certificate in a region different from the stack's region (e.g. `us-east-1` for cloudfront),
 and allows for creating a certificate for a Route 53 hosted zone in another AWS account.
 
@@ -121,14 +108,15 @@
 
 #### Syntax
 
 ```yaml
 DomainName: String
 HostedZoneId: String
 Route53RoleArn: String
+Route53RoleExternalId: String
 ```
 
 #### Properties
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
@@ -146,15 +134,23 @@
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
- 
+
+* `Route53RoleExternalId`
+
+  An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
+  See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
+
+  - Required: No
+  - Type: String
+
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
 You can then import the Certificate resource from troposphere_dns_certificate.certificatemanager instead of troposphere.certificatemanager. 
@@ -277,26 +273,30 @@
 
 ### Assuming a role for Route 53 record creation
 
 In some cases the account owning the hosted zone might be a different one than the one you are generating the certificate in.
 To support this you can specify the domain validation option property `Route53RoleArn` with a role-ARN that should be 
 assumed before creating the records required for certificate validation.
 
+Optionally, you can also specify a `Route53RoleExternalId` that will be used when assuming the role specified by `Route53RoleArn`.
+This would be required if the trust policy of the role requires an external ID.
+
 If a top-level Route53RoleArn property is specified it will be assumed when validating domains that don't contain a
 Route53RoleArn domain validation option property.
 
 ```yaml
 ExampleCertificate:
   Properties:
     DomainName: test.example.com
     ValidationMethod: DNS
     DomainValidationOptions:
       - DomainName: test.example.com
         HostedZoneId: Z2KZ5YTUFZNC7H
         Route53RoleArn: arn:aws:iam::TRUSTING-ACCOUNT-ID:role/ACMRecordCreationRole
+        Route53RoleExternalId: EXTERNAL-ID
     Tags:
       - Key: Name
         Value: Example Certificate
     ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'
   Type: Custom::DNSCertificate
 ```
 
@@ -369,14 +369,17 @@
       Statement:
         - Action:
             - sts:AssumeRole
           Principal:
             AWS:
               - arn:aws:iam::TRUSTED-ACCOUNT-ID:root
           Effect: Allow
+          Condition:
+            StringEquals:
+              'sts:ExternalId': EXTERNAL-ID
       Version: '2012-10-17'
     Policies:
       - PolicyName: 'ACMRecordCreation'
         PolicyDocument:
           Version: '2012-10-17'
           Statement:
             - Action:
```

### Comparing `troposphere-dns-certificate-1.7.5/README.md` & `troposphere-dns-certificate-1.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: troposphere-dns-certificate
+Version: 1.8.0
+Summary: Cloudformation DNS validated certificate resource for troposphere
+Home-page: https://github.com/dflook/cloudformation-dns-certificate
+Author: Daniel Flook
+Author-email: daniel@flook.org
+License: MIT
+Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
+Keywords: cloudformation troposphere certificate
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cloudformation DNS Validated Certificate Resource
 
 This is a cloudformation custom resource which is an enhancement of the [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html) resource.
 
 It allows creating a certificate in a region different from the stack's region (e.g. `us-east-1` for cloudfront),
 and allows for creating a certificate for a Route 53 hosted zone in another AWS account.
 
@@ -108,14 +121,15 @@
 
 #### Syntax
 
 ```yaml
 DomainName: String
 HostedZoneId: String
 Route53RoleArn: String
+Route53RoleExternalId: String
 ```
 
 #### Properties
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
@@ -133,15 +147,23 @@
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
- 
+
+* `Route53RoleExternalId`
+
+  An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
+  See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
+
+  - Required: No
+  - Type: String
+
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
 You can then import the Certificate resource from troposphere_dns_certificate.certificatemanager instead of troposphere.certificatemanager. 
@@ -264,26 +286,30 @@
 
 ### Assuming a role for Route 53 record creation
 
 In some cases the account owning the hosted zone might be a different one than the one you are generating the certificate in.
 To support this you can specify the domain validation option property `Route53RoleArn` with a role-ARN that should be 
 assumed before creating the records required for certificate validation.
 
+Optionally, you can also specify a `Route53RoleExternalId` that will be used when assuming the role specified by `Route53RoleArn`.
+This would be required if the trust policy of the role requires an external ID.
+
 If a top-level Route53RoleArn property is specified it will be assumed when validating domains that don't contain a
 Route53RoleArn domain validation option property.
 
 ```yaml
 ExampleCertificate:
   Properties:
     DomainName: test.example.com
     ValidationMethod: DNS
     DomainValidationOptions:
       - DomainName: test.example.com
         HostedZoneId: Z2KZ5YTUFZNC7H
         Route53RoleArn: arn:aws:iam::TRUSTING-ACCOUNT-ID:role/ACMRecordCreationRole
+        Route53RoleExternalId: EXTERNAL-ID
     Tags:
       - Key: Name
         Value: Example Certificate
     ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'
   Type: Custom::DNSCertificate
 ```
 
@@ -356,14 +382,17 @@
       Statement:
         - Action:
             - sts:AssumeRole
           Principal:
             AWS:
               - arn:aws:iam::TRUSTED-ACCOUNT-ID:root
           Effect: Allow
+          Condition:
+            StringEquals:
+              'sts:ExternalId': EXTERNAL-ID
       Version: '2012-10-17'
     Policies:
       - PolicyName: 'ACMRecordCreation'
         PolicyDocument:
           Version: '2012-10-17'
           Statement:
             - Action:
```

### Comparing `troposphere-dns-certificate-1.7.5/setup.py` & `troposphere-dns-certificate-1.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 readme_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(readme_path) as f:
     long_desc = f.read()
 
 setup(
     name='troposphere-dns-certificate',
     description='Cloudformation DNS validated certificate resource for troposphere',
-    version='1.7.5',
+    version='1.8.0',
     author='Daniel Flook',
     author_email='daniel@flook.org',
     url='https://github.com/dflook/cloudformation-dns-certificate',
     license='MIT',
     project_urls={
         'Issues': 'https://github.com/dflook/cloudformation-dns-certificate/issues',
     },
     keywords='cloudformation troposphere certificate',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     long_description=long_desc,
     long_description_content_type='text/markdown',
-    install_requires=['troposphere', 'awacs', 'wrapt', 'python_minifier >= 2.3.0', 'boto3'],
+    install_requires=['troposphere >= 4.3.1', 'awacs', 'wrapt', 'python_minifier >= 2.3.0', 'boto3'],
     zip_safe=False
 )
```

### Comparing `troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/__init__.py` & `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/certificate.py` & `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,19 +229,27 @@
 
         for validation_option in cert['DomainValidationOptions']:
 
             if validation_option['ValidationStatus'] == 'PENDING_VALIDATION':
                 hosted_zone = get_zone_for(validation_option['DomainName'])
 
                 role_arn = hosted_zone.get('Route53RoleArn', props.get('Route53RoleArn'))
+                external_id = hosted_zone.get('Route53RoleExternalId')
+
+                sts_params = {
+                    'RoleArn': role_arn,
+                    'RoleSessionName': ('Certificate' + event['LogicalResourceId'])[:64],
+                    'DurationSeconds': 900,
+                }
+
+                if external_id:
+                    sts_params['ExternalId'] = external_id
 
                 sts = client('sts').assume_role(
-                    RoleArn=role_arn,
-                    RoleSessionName=('Certificate' + event['LogicalResourceId'])[:64],
-                    DurationSeconds=900,
+                    **sts_params
                 )['Credentials'] if role_arn is not None else {}
 
                 route53 = client('route53',
                      aws_access_key_id=sts.get('AccessKeyId'),
                      aws_secret_access_key=sts.get('SecretAccessKey'),
                      aws_session_token=sts.get('SessionToken'),
                  ).change_resource_record_sets(**{
```

### Comparing `troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate/certificatemanager.py` & `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificatemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 class DomainValidationOption(AWSProperty):
     props = {
         'DomainName': (str, True),
         'ValidationDomain': (str, False),
         'HostedZoneId': (str, False),
         'Route53RoleArn': (str, False),
+        'Route53RoleExternalId': (str, False)
     }
 
 
 class Certificate(CustomResource, TroposphereExtension):
     resource_type = 'Custom::DNSCertificate'
 
     props = {
```

### Comparing `troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/PKG-INFO` & `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troposphere-dns-certificate
-Version: 1.7.5
+Version: 1.8.0
 Summary: Cloudformation DNS validated certificate resource for troposphere
 Home-page: https://github.com/dflook/cloudformation-dns-certificate
 Author: Daniel Flook
 Author-email: daniel@flook.org
 License: MIT
 Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
 Keywords: cloudformation troposphere certificate
@@ -121,14 +121,15 @@
 
 #### Syntax
 
 ```yaml
 DomainName: String
 HostedZoneId: String
 Route53RoleArn: String
+Route53RoleExternalId: String
 ```
 
 #### Properties
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
@@ -146,15 +147,23 @@
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
- 
+
+* `Route53RoleExternalId`
+
+  An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
+  See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
+
+  - Required: No
+  - Type: String
+
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
 You can then import the Certificate resource from troposphere_dns_certificate.certificatemanager instead of troposphere.certificatemanager. 
@@ -277,26 +286,30 @@
 
 ### Assuming a role for Route 53 record creation
 
 In some cases the account owning the hosted zone might be a different one than the one you are generating the certificate in.
 To support this you can specify the domain validation option property `Route53RoleArn` with a role-ARN that should be 
 assumed before creating the records required for certificate validation.
 
+Optionally, you can also specify a `Route53RoleExternalId` that will be used when assuming the role specified by `Route53RoleArn`.
+This would be required if the trust policy of the role requires an external ID.
+
 If a top-level Route53RoleArn property is specified it will be assumed when validating domains that don't contain a
 Route53RoleArn domain validation option property.
 
 ```yaml
 ExampleCertificate:
   Properties:
     DomainName: test.example.com
     ValidationMethod: DNS
     DomainValidationOptions:
       - DomainName: test.example.com
         HostedZoneId: Z2KZ5YTUFZNC7H
         Route53RoleArn: arn:aws:iam::TRUSTING-ACCOUNT-ID:role/ACMRecordCreationRole
+        Route53RoleExternalId: EXTERNAL-ID
     Tags:
       - Key: Name
         Value: Example Certificate
     ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'
   Type: Custom::DNSCertificate
 ```
 
@@ -369,14 +382,17 @@
       Statement:
         - Action:
             - sts:AssumeRole
           Principal:
             AWS:
               - arn:aws:iam::TRUSTED-ACCOUNT-ID:root
           Effect: Allow
+          Condition:
+            StringEquals:
+              'sts:ExternalId': EXTERNAL-ID
       Version: '2012-10-17'
     Policies:
       - PolicyName: 'ACMRecordCreation'
         PolicyDocument:
           Version: '2012-10-17'
           Statement:
             - Action:
```

### Comparing `troposphere-dns-certificate-1.7.5/src/troposphere_dns_certificate.egg-info/SOURCES.txt` & `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

