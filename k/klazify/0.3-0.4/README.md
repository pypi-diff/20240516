# Comparing `tmp/klazify-0.3.tar.gz` & `tmp/klazify-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klazify-0.3.tar", last modified: Thu May 16 17:42:26 2024, max compression
+gzip compressed data, was "klazify-0.4.tar", last modified: Thu May 16 18:41:38 2024, max compression
```

## Comparing `klazify-0.3.tar` & `klazify-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:42:26.511902 klazify-0.3/
--rw-rw-rw-   0        0        0     7221 2024-05-16 17:42:26.510439 klazify-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6443 2024-05-16 17:41:26.000000 klazify-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 17:42:26.497665 klazify-0.3/klazify.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-05-16 17:42:26.000000 klazify-0.3/klazify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-16 17:42:26.000000 klazify-0.3/klazify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:42:26.000000 klazify-0.3/klazify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 17:42:26.000000 klazify-0.3/klazify.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 17:42:26.508440 klazify-0.3/klazify_api/
--rw-rw-rw-   0        0        0       47 2024-05-16 16:13:44.000000 klazify-0.3/klazify_api/__init__.py
--rw-rw-rw-   0        0        0      557 2024-05-16 17:34:21.000000 klazify-0.3/klazify_api/client.py
--rw-rw-rw-   0        0        0       42 2024-05-16 17:42:26.512437 klazify-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1121 2024-05-16 17:40:03.000000 klazify-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:41:38.392158 klazify-0.4/
+-rw-rw-rw-   0        0        0     8665 2024-05-16 18:41:38.391160 klazify-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7887 2024-05-16 18:38:51.000000 klazify-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:41:38.385163 klazify-0.4/klazify.egg-info/
+-rw-rw-rw-   0        0        0     8665 2024-05-16 18:41:38.000000 klazify-0.4/klazify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-16 18:41:38.000000 klazify-0.4/klazify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:41:38.000000 klazify-0.4/klazify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 18:41:38.000000 klazify-0.4/klazify.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 18:41:38.389168 klazify-0.4/klazify_api/
+-rw-rw-rw-   0        0        0       47 2024-05-16 16:13:44.000000 klazify-0.4/klazify_api/__init__.py
+-rw-rw-rw-   0        0        0     4035 2024-05-16 18:34:00.000000 klazify-0.4/klazify_api/client.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:41:38.393157 klazify-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2024-05-16 18:40:40.000000 klazify-0.4/setup.py
```

### Comparing `klazify-0.3/PKG-INFO` & `klazify-0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: klazify
-Version: 0.3
-Summary: The most accurate Content Classification API. All-in-one domain data source
-Home-page: https://github.com/Zyla-Labs/pypi-klazify-api
-Author: Klazify
-Author-email: hello@klazify.com
-Keywords: Get Website Logos api,Brand Imagery api,We Categorize the Web,api for website,api key for website,logo api,banking logo api,company logo api,api key website,api of website,best api for website,create an api for a website,create an api for your website,Website Category API, Website Logo API,logo api,URL logo api,Webshrinker,classifies a site into a category,brandfetch,url categorization,url category check api,website category lookup,web categories,url classification dataset
-Description-Content-Type: text/markdown
-
 # [![Klazify](https://www.klazify.com/img/new_klazify_logo.png)](https://klazify.com)
 
 **Klazify** - The most accurate Content Classification API.
 All-in-one domain data source. Get Website Logos, Company Data, Categorization and much more from a URL or Email.
 
 ## Key Features:
 
@@ -20,14 +10,45 @@
 - Full Path URL support
 - Batch Enrichement importing a .CSV.
 - Extract Logo from any URL
 - Social Media Links Scraper API.
 - Multi-site license. 
 - Service-level agreement (SLA).
 
+## Endpoints availables
+
+The Klazify API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+
+1. **Categorization API**
+   - Retrieve the IAB and Klazify category for a specified domain.
+
+2. **Logo API**
+   - Obtain the logo URL associated with a given domain.
+
+3. **Company API**
+   - Provides comprehensive details regarding the categorization of a given domain, with a focus on information related to the identified company and its attributes.
+   
+4. **Website Tech Stack API**
+   - Returns the technological stack utilized by the requested website.
+
+5. **IAB Categories API**
+   - Retrieves the IAB category and its confidence level (ranging from 0 to 1).
+
+6. **Competitors API**
+   - Retrieves competitor domains.
+    
+7. **Similar Companies API**
+   - Identifies companies similar to the specified domain.
+
+8. **Parked Domain API**
+   - Based on the content of a website, indicates whether a domain is parked or not.
+     
+9. **Social Media Links API**
+   - Retrieves the social media links associated with a given domain.
+
 ## Documentation
 
 For comprehensive details regarding API endpoints, usage, and integration guidelines, please refer to our [API Documentation](https://www.klazify.com/category#docs).
 
 Begin leveraging Klazify today to classify any domain or email! Visit [Klazify.com](https://klazify.com) and seamlessly integrate within minutes!
 
 ## Installation
@@ -217,8 +238,16 @@
 }
 ```
 
 ### AVAILABLE METHODS
 
 ```python
 >>> categorize_url(url: str)
+>>> real_time_categorization(url: str)
+>>> domain_logo(url: str)
+>>> domain_company(url: str)
+>>> domain_tech(url: str)
+>>> domain_iab_categories(url: str)
+>>> similar_domain(url: str)
+>>> domain_expiration(url: str)
+>>> domain_social_media(url: str)
 ```
```

### Comparing `klazify-0.3/README.md` & `klazify-0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: klazify
+Version: 0.4
+Summary: The most accurate Content Classification API. All-in-one domain data source
+Home-page: https://github.com/Zyla-Labs/pypi-klazify-api
+Author: Klazify
+Author-email: hello@klazify.com
+Keywords: Get Website Logos api,Brand Imagery api,We Categorize the Web,api for website,api key for website,logo api,banking logo api,company logo api,api key website,api of website,best api for website,create an api for a website,create an api for your website,Website Category API, Website Logo API,logo api,URL logo api,Webshrinker,classifies a site into a category,brandfetch,url categorization,url category check api,website category lookup,web categories,url classification dataset
+Description-Content-Type: text/markdown
+
 # [![Klazify](https://www.klazify.com/img/new_klazify_logo.png)](https://klazify.com)
 
 **Klazify** - The most accurate Content Classification API.
 All-in-one domain data source. Get Website Logos, Company Data, Categorization and much more from a URL or Email.
 
 ## Key Features:
 
@@ -10,14 +20,45 @@
 - Full Path URL support
 - Batch Enrichement importing a .CSV.
 - Extract Logo from any URL
 - Social Media Links Scraper API.
 - Multi-site license. 
 - Service-level agreement (SLA).
 
+## Endpoints availables
+
+The Klazify API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+
+1. **Categorization API**
+   - Retrieve the IAB and Klazify category for a specified domain.
+
+2. **Logo API**
+   - Obtain the logo URL associated with a given domain.
+
+3. **Company API**
+   - Provides comprehensive details regarding the categorization of a given domain, with a focus on information related to the identified company and its attributes.
+   
+4. **Website Tech Stack API**
+   - Returns the technological stack utilized by the requested website.
+
+5. **IAB Categories API**
+   - Retrieves the IAB category and its confidence level (ranging from 0 to 1).
+
+6. **Competitors API**
+   - Retrieves competitor domains.
+    
+7. **Similar Companies API**
+   - Identifies companies similar to the specified domain.
+
+8. **Parked Domain API**
+   - Based on the content of a website, indicates whether a domain is parked or not.
+     
+9. **Social Media Links API**
+   - Retrieves the social media links associated with a given domain.
+
 ## Documentation
 
 For comprehensive details regarding API endpoints, usage, and integration guidelines, please refer to our [API Documentation](https://www.klazify.com/category#docs).
 
 Begin leveraging Klazify today to classify any domain or email! Visit [Klazify.com](https://klazify.com) and seamlessly integrate within minutes!
 
 ## Installation
@@ -207,8 +248,16 @@
 }
 ```
 
 ### AVAILABLE METHODS
 
 ```python
 >>> categorize_url(url: str)
+>>> real_time_categorization(url: str)
+>>> domain_logo(url: str)
+>>> domain_company(url: str)
+>>> domain_tech(url: str)
+>>> domain_iab_categories(url: str)
+>>> similar_domain(url: str)
+>>> domain_expiration(url: str)
+>>> domain_social_media(url: str)
 ```
```

### Comparing `klazify-0.3/klazify.egg-info/PKG-INFO` & `klazify-0.4/klazify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klazify
-Version: 0.3
+Version: 0.4
 Summary: The most accurate Content Classification API. All-in-one domain data source
 Home-page: https://github.com/Zyla-Labs/pypi-klazify-api
 Author: Klazify
 Author-email: hello@klazify.com
 Keywords: Get Website Logos api,Brand Imagery api,We Categorize the Web,api for website,api key for website,logo api,banking logo api,company logo api,api key website,api of website,best api for website,create an api for a website,create an api for your website,Website Category API, Website Logo API,logo api,URL logo api,Webshrinker,classifies a site into a category,brandfetch,url categorization,url category check api,website category lookup,web categories,url classification dataset
 Description-Content-Type: text/markdown
 
@@ -20,14 +20,45 @@
 - Full Path URL support
 - Batch Enrichement importing a .CSV.
 - Extract Logo from any URL
 - Social Media Links Scraper API.
 - Multi-site license. 
 - Service-level agreement (SLA).
 
+## Endpoints availables
+
+The Klazify API comes with multiple endpoints, each providing different functionality. Please note that depending on your subscription plan, certain API endpoints may or may not be available.
+
+1. **Categorization API**
+   - Retrieve the IAB and Klazify category for a specified domain.
+
+2. **Logo API**
+   - Obtain the logo URL associated with a given domain.
+
+3. **Company API**
+   - Provides comprehensive details regarding the categorization of a given domain, with a focus on information related to the identified company and its attributes.
+   
+4. **Website Tech Stack API**
+   - Returns the technological stack utilized by the requested website.
+
+5. **IAB Categories API**
+   - Retrieves the IAB category and its confidence level (ranging from 0 to 1).
+
+6. **Competitors API**
+   - Retrieves competitor domains.
+    
+7. **Similar Companies API**
+   - Identifies companies similar to the specified domain.
+
+8. **Parked Domain API**
+   - Based on the content of a website, indicates whether a domain is parked or not.
+     
+9. **Social Media Links API**
+   - Retrieves the social media links associated with a given domain.
+
 ## Documentation
 
 For comprehensive details regarding API endpoints, usage, and integration guidelines, please refer to our [API Documentation](https://www.klazify.com/category#docs).
 
 Begin leveraging Klazify today to classify any domain or email! Visit [Klazify.com](https://klazify.com) and seamlessly integrate within minutes!
 
 ## Installation
@@ -217,8 +248,16 @@
 }
 ```
 
 ### AVAILABLE METHODS
 
 ```python
 >>> categorize_url(url: str)
+>>> real_time_categorization(url: str)
+>>> domain_logo(url: str)
+>>> domain_company(url: str)
+>>> domain_tech(url: str)
+>>> domain_iab_categories(url: str)
+>>> similar_domain(url: str)
+>>> domain_expiration(url: str)
+>>> domain_social_media(url: str)
 ```
```

### Comparing `klazify-0.3/setup.py` & `klazify-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name='klazify',
-    version='0.3',
+    version='0.4',
     description = 'The most accurate Content Classification API. All-in-one domain data source',
     author = 'Klazify',
     author_email = 'hello@klazify.com',
     url = 'https://github.com/Zyla-Labs/pypi-klazify-api',
     keywords = ['Get Website Logos api','Brand Imagery api','We Categorize the Web', 'api for website', 'api key for website', 'logo api', 'banking logo api', 'company logo api',  'api key website', 'api of website',  'best api for website' , 'create an api for a website',  'create an api for your website', 'Website Category API' ,' Website Logo API' , 'logo api', 'URL logo api', 'Webshrinker',  'classifies a site into a category', 'brandfetch', 'url categorization', 'url category check api',  'website category lookup', 'web categories', 'url classification dataset'],
     packages=find_packages(),
     install_requires=[
```

