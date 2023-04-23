# Comparing `tmp/networth-1.1.0.tar.gz` & `tmp/networth-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/networth-1.1.0.tar", last modified: Fri Mar 12 02:12:51 2021, max compression
+gzip compressed data, was "networth-1.2.tar", last modified: Sun Apr 23 01:50:53 2023, max compression
```

## Comparing `networth-1.1.0.tar` & `networth-1.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 ken       (1000) ken        (502)        0 2021-03-12 02:12:51.343503 networth-1.1.0/
--rw-rw-r--   0 ken       (1000) ken        (502)    17324 2021-03-12 02:12:51.343503 networth-1.1.0/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken        (502)    13449 2021-03-12 02:09:24.000000 networth-1.1.0/README.rst
--rwxrwxr-x   0 ken       (1000) ken        (502)    29495 2021-03-12 02:09:24.000000 networth-1.1.0/networth
-drwxrwxr-x   0 ken       (1000) ken        (502)        0 2021-03-12 02:12:51.342503 networth-1.1.0/networth.egg-info/
--rw-rw-r--   0 ken       (1000) ken        (502)    17324 2021-03-12 02:12:51.000000 networth-1.1.0/networth.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken        (502)      201 2021-03-12 02:12:51.000000 networth-1.1.0/networth.egg-info/SOURCES.txt
--rw-rw-r--   0 ken       (1000) ken        (502)        1 2021-03-12 02:12:51.000000 networth-1.1.0/networth.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken        (502)      123 2021-03-12 02:12:51.000000 networth-1.1.0/networth.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken        (502)        1 2021-03-12 02:12:51.000000 networth-1.1.0/networth.egg-info/top_level.txt
--rwxrwxr-x   0 ken       (1000) ken        (502)     5363 2021-02-23 23:08:58.000000 networth-1.1.0/plot-networth
--rw-rw-r--   0 ken       (1000) ken        (502)       38 2021-03-12 02:12:51.343503 networth-1.1.0/setup.cfg
--rw-rw-r--   0 ken       (1000) ken        (502)     1702 2021-03-12 02:09:24.000000 networth-1.1.0/setup.py
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-23 01:50:53.596948 networth-1.2/
+-rw-rw-r--   0 ken       (1000) ken       (1001)    35142 2019-11-13 05:28:15.000000 networth-1.2/LICENSE
+-rw-------   0 ken       (1000) ken       (1001)    14891 2023-04-23 01:50:53.596948 networth-1.2/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1001)    14123 2023-04-23 01:39:59.000000 networth-1.2/README.rst
+-rwxrwxr-x   0 ken       (1000) ken       (1001)    32871 2023-04-23 01:39:59.000000 networth-1.2/networth
+drwx------   0 ken       (1000) ken       (1001)        0 2023-04-23 01:50:53.595948 networth-1.2/networth.egg-info/
+-rw-------   0 ken       (1000) ken       (1001)    14891 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/PKG-INFO
+-rw-------   0 ken       (1000) ken       (1001)      236 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/SOURCES.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/dependency_links.txt
+-rw-------   0 ken       (1000) ken       (1001)      123 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/requires.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/top_level.txt
+-rw-------   0 ken       (1000) ken       (1001)        1 2023-04-23 01:50:53.000000 networth-1.2/networth.egg-info/zip-safe
+-rwxrwxr-x   0 ken       (1000) ken       (1001)     5896 2023-04-22 22:14:37.000000 networth-1.2/plot-networth
+-rw-------   0 ken       (1000) ken       (1001)       38 2023-04-23 01:50:53.596948 networth-1.2/setup.cfg
+-rw-rw-r--   0 ken       (1000) ken       (1001)     1572 2023-04-23 01:42:33.000000 networth-1.2/setup.py
```

### Comparing `networth-1.1.0/PKG-INFO` & `networth-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,393 +1,411 @@
 Metadata-Version: 2.1
 Name: networth
-Version: 1.1.0
+Version: 1.2
 Summary: Summarize net worth
 Home-page: https://github.com/kenkundert/networth
+Download-URL: https://github.com/kenkundert/networth/tarball/master
 Author: Ken Kundert
 Author-email: networth@nurdletech.com
 License: GPLv3+
-Download-URL: https://github.com/kenkundert/networth/tarball/master
-Description: Networth: Summarize Your Net Worth
-        ==================================
-        
-        | Version: 1.1.0
-        | Released: 2021-03-11
-        
-        *Networth* works with `Avendesora <https://avendesora.readthedocs.io>`_ to 
-        generate a summary of your networth. *Networth* reads *estimated_value* fields 
-        from *Avendesora* accounts and summarizes the result.  It is often used with, 
-        and shares fields with, `PostMortem <https://github.com/KenKundert/postmortem>`_.
-        Works with data services to download up-to-date prices for securities and 
-        cryptocurrencies.
-        
-        Please report all bugs and suggestions to networth@nurdletech.com
-        
-        Getting Started
-        ---------------
-        
-        You download and install *Networth* with::
-        
-            pip3 install --user networth
-        
-        Once installed, you will need at least two configuration files. The 
-        configuration files are `NestedText <https://nestedtext.readthedocs.io>`_.  The 
-        first file contains settings that are shared between all profiles.  It is 
-        ~/.config/networth/config.  The remaining files are specific to profiles.  You 
-        would generally have one profile for yourself, but you might also have profiles 
-        for organizations or people that you are monitoring.
-        
-        Profile files have a .prof suffix, and the name of the profile is the name of 
-        the profile file without the suffix.
-        
-        In general, any setting may be in either the config file or the profile file.  
-        However, the following setting should in the config file:
-        
-        default profile:
-            A string that contains the name of the profile to use if the one is not 
-            explicitly specified on the command line.
-        
-        In addition, the following settings are available:
-        
-        avendesora fieldname:
-            The name of the *Avendesora* account field that contains the networth 
-            information.  Typically *estimated_value*.
-        
-        value updated subfieldname:
-            The name of the subfield of *estimated_value* that contains the date the 
-            value was last updated.  Typically *updated*.
-        
-        max account value age:
-            Number of days. Values that are older than this are called out as being 
-            stale. Default is 120 days.
-        
-        date formats:
-            The list of allowed date formats. May be specified as a list or as a string
-            string that contains the allowed date formats separated by white space.  Any 
-            spaces is a specific format is replaced by an underscore so that it is not 
-            confused as more than one format. For example a format of 'MMMM YYYY' would 
-            be represented as 'MMMM_YYYY'. The formats allowed are those supported by 
-            Arrow.
-        
-            By default the following formats are accepted: 'MMMM YYYY', 'MMM YYYY', 
-            'YYYY-M-D', and 'YYMMDD'. So the following dates would be accepted: 'January 
-            2019', 'Jan 2019', '2019-1-1' and '190101'.
-        
-        asset color:
-            The color to used for positive values. May be black, white, blue, cyan, 
-            green, red, magenta, or yellow. The default is green.
-        
-        debt color:
-            The color to used for negative values. May be black, white, blue, cyan, 
-            green, red, magenta, or yellow. The default is red.
-        
-        screen width:
-            An integer that contains the width of the screen.
-        
-        aliases:
-            A dictionary that is used to map an account name to something that is easier 
-            to read.
-        
-        cryptocompare:
-            A dictionary containing information about cryptocurrency prices that are to 
-            be downloaded from cryptocompare.com.
-        
-            To avoid caching issues it is recommended that *cryptocompare* files be 
-            placed in the shared *config* file if multiple profiles need it.
-        
-            tokens:
-                A dictionary of crytpocurrency tokens that should be available for use.
-                The key of the dictionary is the token symbol, the value is the category 
-                it should associate with.
-        
-            ttl:
-                Cache time to live.  If the cache is older than this time, it is 
-                refreshed.  Here are example times: 600s, 10m, 6h, 1d.
-        
-            api key:
-                The coin prices are downloaded from cryptocompare.com. Specifying the 
-                API key is optional.  Providing an API key increases your limits, but 
-                limits are generally not a problem for *Networth* because it is run so 
-                infrequently.
-        
-            api key account field:
-                You may place the API key in *Avendesora* and use this key to specify the 
-                account and field name for the API key.
-        
-        iexcloud:
-            A dictionary containing information about security prices that are to be 
-            downloaded from iexcloud.io.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *iexcloud* files be placed in 
-            the shared *config* file if multiple profiles need it.
-        
-        twelve data:
-            A dictionary containing information about security prices that are to be 
-            downloaded from twelvedata.com.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *twelvedata* files be placed 
-            in the shared *config* file if multiple profiles need it.
-        
-            *Twelve Data* provides real time values, but have very low limits unless you 
-            get an expensive subscription.  If you do not have a subscription, it is 
-            recommended that you limit the number of tokens to 8 or less.
-        
-        metals api:
-            A dictionary containing information about precious metals prices that are to 
-            be downloaded from metals-api.com.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *metals* files be placed in 
-            the shared *config* file if multiple profiles need it.
-        
-        estimated value overrides file:
-            A path to a file of *estimated_value* overrides. Give as a NestedText file 
-            that contains a dictionary of dictionaries.  The keys for the top level are 
-            account names, and the value contains the estimated value dictionary that 
-            would normally be found in the *Avendesora* accounts file.
-        
-        
-        Example Configuration Files
-        ---------------------------
-        
-        Here is an example *config* file::
-        
-            default profile: me
-        
-            # account value settings
-            avendesora fieldname: estimated_value
-            value updated subfieldname: updated
-            max account value age: 120
-            date formats: M/D/YY M/D/YYYY
-        
-            # bar settings
-            screen width: 110
-        
-            # cryptocurrency prices
-            cryptocompare:
-                tokens:
-                    USD: cash
-                    BTC: cryptocurrency
-                    ETH: cryptocurrency
-        
-            # securities prices
-            iexcloud:
-                api key: pk_9eb3acfc7dbe4055a795ff179d46a980
-                tokens:
-                    GOOG: equities
-                    AMZN: equities
-                    GBTC: cryptocurrency
-        
-        Here is a example profile file::
-        
-            # account aliases
-            aliases:
-                quickenloans: mortgage
-                wellsfargo: wells fargo
-        
-        
-        Here is a example estimated value overrides file::
-        
-            chase:
-                updated: February 2021
-                cash:
-                    > $4,425.71 +       # checking
-                    > $1,896.26         # savings
-        
-        
-        Estimated Values
-        ----------------
-        
-        Next, you need to add *estimated_value* fields to your *Avendesora* accounts, 
-        the value of which is a dictionary. It may contain a *updated* subfield that 
-        gives the date the value was last updated.  In addition, it may contain 
-        subfields for various asset classes or coins or securities.  The values may 
-        either be real numbers or strings that contain quantities (values plus units).  
-        Here are some examples::
-        
-            class ChaseBank(Account):
-                ...
-                estimated_value = dict(updated='December 2018', cash=2181.16+5121.79)
-        
-            class QuickenLoans(Account):
-                ...
-                estimated_value = dict(updated='October 2018', real_estate='-$294,058')
-        
-            class Vanguard(Account):
-                ...
-                estimated_value = dict(updated='November 2018', retirement='$74,327')
-        
-            class TDAmeritrade(Account):
-                ...
-                estimated_value = dict( updated='November 2018', retirement='$74,327+$111,554')
-        
-            class Fidelity(Account):
-                ...
-                estimated_value = dict( updated='November 2018', retirement='''
-                    $62,976.22 +    # 401k
-                    $26,704.85      # IRA
-                ''')
-        
-            class UnitedAirlines(Account):
-                ...
-                estimated_value = dict(updated='July 2018', miles='7,384_miles')
-        
-            class CoinBase(Account):
-                ...
-                estimated_value = dict(updated='August 2018', ETH=2, BTC=4, cash=24.52)
-        
-            class TD_Ameritrade(Account):
-                ...
-                estimated_value = dict(updated='January 2019', GOOG=10, AMZN=5, cash=327.53)
-        
-        The value of securities are given is number of shares. The value given for 
-        cryptocurrencies is number of tokens. All other values are assumed to be in 
-        dollars if the units are not given. If the units are given and they are not 
-        dollars (such as miles for frequent flier programs), then those values are 
-        summarized but not included in your total networth.
-        
-        Specifying the *updated* date is optional. If specified, then *networth* will 
-        indicate the values as stale if they exceed *max_account_value_age*.
-        
-        It is also specify information about a loan, and *networth* will compute its 
-        current balance.  This is done by giving the principal on a particular date, the 
-        date for the given principal, the monthly payments, the interest rate, and 
-        optionally, the share. The rate and the share can be given in percent, meaning 
-        that an rate of 4% can either be specified as 4% or as 0.04. Similarly a share 
-        half share can be indicated as 50% or 0.5.  For example::
-        
-            class QuickenLoans(Account):
-                ...
-                estimated_value = dict(
-                    real_estate = '''
-                        principal=-$294,058
-                        date=09/04/2013
-                        payment=$1,500.00
-                        rate=4.375%
-                        share=50%
-                    ''',
-                )
-        
-        the key=value pairs can be separated by any white space, but there must be no
-        white space surrounding the = sign. For mortgages that you owe, the principal 
-        should be negative. You can also use this feature to describe an automatic 
-        savings plan into an interest bearing account.  In this case the principal would 
-        be your starting balance and the payment would be your monthly investment 
-        amount.  In this case the starting balance would be positive.
-        
-        
-        Usage
-        -----
-        
-        When running the command, you may specify a profile. If you do not, you get the 
-        default profile.  For example::
-        
-            > networth me
-            By Account:
-                    betterment:    $22k equities=$9k, cash=$3k, retirement=$9k
-                         chase:     $7k cash
-                     southwest:      $0 miles=78kmiles
-                      coindesk:  $15.3k cryptocurrency
-        
-            By Type:
-                cryptocurrency:  $15.3k (35.3%) ██████████████████████████████████████████
-                          cash:    $10k (23.1%) ███████████████████████████████
-                      equities:     $9k (20.8%) ███████████████████████████
-                    retirement:     $9k (20.8%) ███████████████████████████
-        
-                         TOTAL:  $43.3k (assets = $43.3k, debt = $0)
-        
-        In this run, the values associated with the various asset classes (ex. equities, 
-        cash, retirement, etc.) are taken as is. As such, you must be diligent about 
-        keeping these values up to date, which is a manual operation. You might consider 
-        updating your *estimated values* every 3-6 months.  However the current prices 
-        for your configured securities and cryptocurrencies are downloaded and 
-        multiplied by the given number of shares or tokens to get the up-to-date values 
-        of your equities and cryptocurrency holdings. Thus you only need update them 
-        after a transaction. Finally, mortgage balances are also kept up to date. You 
-        only need update mortgages if you decide to change the payment amount in order 
-        to pay off the loan faster.
-        
-        
-        History
-        -------
-        
-        If you would like to be able to plot your net worth over time you run the 
-        following regularly::
-        
-            networth -w <profile>
-        
-        Each time you do, the networth values are added to a data file 
-        (~/.local/share/networth/<profile>.nt).
-        
-        You can then plot the historical values using::
-        
-            plot-networth <name>...
-        
-        You can get a list of the values you can plot using::
-        
-            plot-networth -l
-        
-        
-        Releases
-        --------
-        **Latest Development Version**:
-            | Version: 1.1.0
-            | Released: 2021-03-11
-        
-        **1.1 (2021-03-11)**:
-            - clean up and minor refinements.
-        
-        **1.0 (2021-02-13)**:
-            - Add *estimated value overrides file* setting.
-            - Add --details option.
-            - Add --write-data option.
-            - Add *plot-networth* command.
-            - Allow categories to be specified for downloaded token prices.
-        
-        **0.8 (2020-10-10)**:
-            - Add support for downloading prices of precious metals.
-            - Switch to *NestedText* for the settings files.
-        
-        **0.7 (2020-03-06)**:
-            - Now uses `QuantiPhy Eval <https://github.com/KenKundert/quantiphy_eval>`_ 
-              to allow you to use expressions within strings for estimated values.
-        
-        **0.6 (2020-01-08)**:
-            - Added --prices and --clear-cache command line options.
-            - Support using a proxy.
-        
-        **0.5 (2019-07-18)**:
-        
-        **0.4 (2019-06-15)**:
-            - Convert to using new IEXcloud API for downloading security prices.
-        
-        **0.3 (2019-04-20)**:
-            - Allow arbitrary date format in mortgages.
-            - Improve error reporting.
-            - Change the sign of the principal in mortgages.
-        
-        **0.1 (2019-03-23)**:
-            - Initial release.
-            - Add mortgage balance calculations.
-        
-        **0.0 (2019-01-31)**:
-            - Initial version.
-        
-        
 Keywords: networth
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Networth — Summarize Your Net Worth
+===================================
+
+.. image:: https://pepy.tech/badge/networth/month
+    :target: https://pepy.tech/project/networth
+
+.. image:: https://img.shields.io/pypi/v/networth.svg
+    :target: https://pypi.python.org/pypi/networth
+
+.. image:: https://img.shields.io/pypi/pyversions/networth.svg
+    :target: https://pypi.python.org/pypi/networth/
+
+
+| Version: 1.2
+| Released: 2023-04-22
+
+*Networth* works with `Avendesora <https://avendesora.readthedocs.io>`_ to 
+generate a summary of your networth. *Networth* reads *estimated_value* fields 
+from *Avendesora* accounts and summarizes the result.  It is often used with, 
+and shares fields with, `PostMortem <https://github.com/KenKundert/postmortem>`_.
+Works with data services to download up-to-date prices for securities and 
+cryptocurrencies.
+
+Please report all bugs and suggestions to networth@nurdletech.com
+
+Getting Started
+---------------
+
+You download and install *Networth* with::
+
+    pip3 install --user networth
+
+Once installed, you will need at least two configuration files. The 
+configuration files are `NestedText <https://nestedtext.readthedocs.io>`_.  The 
+first file contains settings that are shared between all profiles.  It is 
+~/.config/networth/config.  The remaining files are specific to profiles.  You 
+would generally have one profile for yourself, but you might also have profiles 
+for organizations or people that you are monitoring.
+
+Profile files have a .prof suffix, and the name of the profile is the name of 
+the profile file without the suffix.
+
+In general, any setting may be in either the config file or the profile file.  
+However, the following setting should in the config file:
+
+default profile:
+    A string that contains the name of the profile to use if the one is not 
+    explicitly specified on the command line.
+
+In addition, the following settings are available:
+
+avendesora fieldname:
+    The name of the *Avendesora* account field that contains the networth 
+    information.  Typically *estimated_value*.
+
+value updated subfieldname:
+    The name of the subfield of *estimated_value* that contains the date the 
+    value was last updated.  Typically *updated*.
+
+max account value age:
+    Number of days. Values that are older than this are called out as being 
+    stale. Default is 120 days.
+
+date formats:
+    The list of allowed date formats. May be specified as a list or as a string
+    string that contains the allowed date formats separated by white space.  Any 
+    spaces is a specific format is replaced by an underscore so that it is not 
+    confused as more than one format. For example a format of 'MMMM YYYY' would 
+    be represented as 'MMMM_YYYY'. The formats allowed are those supported by 
+    Arrow.
+
+    By default the following formats are accepted: 'MMMM YYYY', 'MMM YYYY', 
+    'YYYY-M-D', and 'YYMMDD'. So the following dates would be accepted: 'January 
+    2019', 'Jan 2019', '2019-1-1' and '190101'.
+
+asset color:
+    The color to used for positive values. May be black, white, blue, cyan, 
+    green, red, magenta, or yellow. The default is green.
+
+debt color:
+    The color to used for negative values. May be black, white, blue, cyan, 
+    green, red, magenta, or yellow. The default is red.
+
+screen width:
+    An integer that contains the width of the screen.
+
+aliases:
+    A dictionary that is used to map an account name to something that is easier 
+    to read.
+
+cryptocompare:
+    A dictionary containing information about cryptocurrency prices that are to 
+    be downloaded from cryptocompare.com.
+
+    To avoid caching issues it is recommended that *cryptocompare* files be 
+    placed in the shared *config* file if multiple profiles need it.
+
+    tokens:
+        A dictionary of crytpocurrency tokens that should be available for use.
+        The key of the dictionary is the token symbol, the value is the category 
+        it should associate with.
+
+    ttl:
+        Cache time to live.  If the cache is older than this time, it is 
+        refreshed.  Here are example times: 600s, 10m, 6h, 1d.  The default is 
+        10m.
+
+    api key:
+        The coin prices are downloaded from cryptocompare.com. Specifying the 
+        API key is optional.  Providing an API key increases your limits, but 
+        limits are generally not a problem for *Networth* because it is run so 
+        infrequently.
+
+    api key account field:
+        You may place the API key in *Avendesora* and use this key to specify the 
+        account and field name for the API key.
+
+iexcloud:
+    A dictionary containing information about security prices that are to be 
+    downloaded from iexcloud.io.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *iexcloud* files be placed in 
+    the shared *config* file if multiple profiles need it.
+
+twelve data:
+    A dictionary containing information about security prices that are to be 
+    downloaded from twelvedata.com.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *twelvedata* files be placed 
+    in the shared *config* file if multiple profiles need it.
+
+    *Twelve Data* provides real time values, but have very low limits unless you 
+    get an expensive subscription.  If you do not have a subscription, it is 
+    recommended that you limit the number of tokens to 8 or less.
+
+metals api:
+    A dictionary containing information about precious metals prices that are to 
+    be downloaded from metals-api.com.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *metals* files be placed in 
+    the shared *config* file if multiple profiles need it.
+
+    Metals API has dropped their free tier.
+
+metals live:
+    A dictionary containing information about precious metals prices that are to 
+    be downloaded from metals-api.com.  This dictionary only requires the 
+    *tokens* field. An API key is not required.
+
+estimated value overrides file:
+    A path to a file of *estimated_value* overrides. Give as a NestedText file 
+    that contains a dictionary of dictionaries.  The keys for the top level are 
+    account names, and the value contains the estimated value dictionary that 
+    would normally be found in the *Avendesora* accounts file.
+
+
+Example Configuration Files
+---------------------------
+
+Here is an example *config* file::
+
+    default profile: me
+
+    # account value settings
+    avendesora fieldname: estimated_value
+    value updated subfieldname: updated
+    max account value age: 120
+    date formats: M/D/YY M/D/YYYY
+
+    # bar settings
+    screen width: 110
+
+    # cryptocurrency prices
+    cryptocompare:
+        tokens:
+            USD: cash
+            BTC: cryptocurrency
+            ETH: cryptocurrency
+
+    # securities prices
+    iexcloud:
+        api key: pk_9eb3acfc7dbe4055a795ff179d46a980
+        tokens:
+            GOOG: equities
+            AMZN: equities
+            GBTC: cryptocurrency
+
+Here is a example profile file::
+
+    # account aliases
+    aliases:
+        quickenloans: mortgage
+        wellsfargo: wells fargo
+
+
+Here is a example estimated value overrides file::
+
+    chase:
+        updated: February 2021
+        cash:
+            > $4,425.71 +       # checking
+            > $1,896.26         # savings
+
+
+Estimated Values
+----------------
+
+Next, you need to add *estimated_value* fields to your *Avendesora* accounts, 
+the value of which is a dictionary. It may contain a *updated* subfield that 
+gives the date the value was last updated.  In addition, it may contain 
+subfields for various asset classes or coins or securities.  The values may 
+either be real numbers or strings that contain quantities (values plus units).  
+Here are some examples::
+
+    class ChaseBank(Account):
+        ...
+        estimated_value = dict(updated='December 2018', cash=2181.16+5121.79)
+
+    class QuickenLoans(Account):
+        ...
+        estimated_value = dict(updated='October 2018', real_estate='-$294,058')
+
+    class Vanguard(Account):
+        ...
+        estimated_value = dict(updated='November 2018', retirement='$74,327')
+
+    class TDAmeritrade(Account):
+        ...
+        estimated_value = dict( updated='November 2018', retirement='$74,327+$111,554')
+
+    class Fidelity(Account):
+        ...
+        estimated_value = dict( updated='November 2018', retirement='''
+            $62,976.22 +    # 401k
+            $26,704.85      # IRA
+        ''')
+
+    class UnitedAirlines(Account):
+        ...
+        estimated_value = dict(updated='July 2018', miles='7,384_miles')
+
+    class CoinBase(Account):
+        ...
+        estimated_value = dict(updated='August 2018', ETH=2, BTC=4, cash=24.52)
+
+    class TD_Ameritrade(Account):
+        ...
+        estimated_value = dict(updated='January 2019', GOOG=10, AMZN=5, cash=327.53)
+
+The value of securities are given is number of shares. The value given for 
+cryptocurrencies is number of tokens. All other values are assumed to be in 
+dollars if the units are not given. If the units are given and they are not 
+dollars (such as miles for frequent flier programs), then those values are 
+summarized but not included in your total networth.
+
+Specifying the *updated* date is optional. If specified, then *networth* will 
+indicate the values as stale if they exceed *max_account_value_age*.
+
+It is also specify information about a loan, and *networth* will compute its 
+current balance.  This is done by giving the principal on a particular date, the 
+date for the given principal, the monthly payments, the interest rate, and 
+optionally, the share. The rate and the share can be given in percent, meaning 
+that an rate of 4% can either be specified as 4% or as 0.04. Similarly a share 
+half share can be indicated as 50% or 0.5.  For example::
+
+    class QuickenLoans(Account):
+        ...
+        estimated_value = dict(
+            real_estate = '''
+                principal=-$294,058
+                date=09/04/2013
+                payment=$1,500.00
+                rate=4.375%
+                share=50%
+            ''',
+        )
+
+the key=value pairs can be separated by any white space, but there must be no
+white space surrounding the = sign. For mortgages that you owe, the principal 
+should be negative. You can also use this feature to describe an automatic 
+savings plan into an interest bearing account.  In this case the principal would 
+be your starting balance and the payment would be your monthly investment 
+amount.  In this case the starting balance would be positive.
+
+
+Usage
+-----
+
+When running the command, you may specify a profile. If you do not, you get the 
+default profile.  For example::
+
+    > networth me
+    By Account:
+            betterment:    $22k equities=$9k, cash=$3k, retirement=$9k
+                 chase:     $7k cash
+             southwest:      $0 miles=78kmiles
+              coindesk:  $15.3k cryptocurrency
+
+    By Type:
+        cryptocurrency:  $15.3k (35.3%) ██████████████████████████████████████████
+                  cash:    $10k (23.1%) ███████████████████████████████
+              equities:     $9k (20.8%) ███████████████████████████
+            retirement:     $9k (20.8%) ███████████████████████████
+
+                 TOTAL:  $43.3k (assets = $43.3k, debt = $0)
+
+In this run, the values associated with the various asset classes (ex. equities, 
+cash, retirement, etc.) are taken as is. As such, you must be diligent about 
+keeping these values up to date, which is a manual operation. You might consider 
+updating your *estimated values* every 3-6 months.  However the current prices 
+for your configured securities and cryptocurrencies are downloaded and 
+multiplied by the given number of shares or tokens to get the up-to-date values 
+of your equities and cryptocurrency holdings. Thus you only need update them 
+after a transaction. Finally, mortgage balances are also kept up to date. You 
+only need update mortgages if you decide to change the payment amount in order 
+to pay off the loan faster.
+
+
+History
+-------
+
+If you would like to be able to plot your net worth over time you run the 
+following regularly::
+
+    networth -w <profile>
+
+Each time you do, the networth values are added to a data file 
+(~/.local/share/networth/<profile>.nt).
+
+You can then plot the historical values using::
+
+    plot-networth <name>...
+
+You can get a list of the values you can plot using::
+
+    plot-networth -l
+
+
+Releases
+--------
+**Latest Development Version**:
+    | Version: 1.2
+    | Released: 2023-04-22
+
+**1.2 (2023-04-22)**:
+    - add metals.live data service
+
+**1.1 (2021-03-11)**:
+    - clean up and minor refinements.
+
+**1.0 (2021-02-13)**:
+    - Add *estimated value overrides file* setting.
+    - Add --details option.
+    - Add --write-data option.
+    - Add *plot-networth* command.
+    - Allow categories to be specified for downloaded token prices.
+
+**0.8 (2020-10-10)**:
+    - Add support for downloading prices of precious metals.
+    - Switch to *NestedText* for the settings files.
+
+**0.7 (2020-03-06)**:
+    - Now uses `QuantiPhy Eval <https://github.com/KenKundert/quantiphy_eval>`_ 
+      to allow you to use expressions within strings for estimated values.
+
+**0.6 (2020-01-08)**:
+    - Added --prices and --clear-cache command line options.
+    - Support using a proxy.
+
+**0.5 (2019-07-18)**:
+
+**0.4 (2019-06-15)**:
+    - Convert to using new IEXcloud API for downloading security prices.
+
+**0.3 (2019-04-20)**:
+    - Allow arbitrary date format in mortgages.
+    - Improve error reporting.
+    - Change the sign of the principal in mortgages.
+
+**0.1 (2019-03-23)**:
+    - Initial release.
+    - Add mortgage balance calculations.
+
+**0.0 (2019-01-31)**:
+    - Initial version.
+
```

### Comparing `networth-1.1.0/README.rst` & `networth-1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-Networth: Summarize Your Net Worth
-==================================
+Networth — Summarize Your Net Worth
+===================================
 
-| Version: 1.1.0
-| Released: 2021-03-11
+.. image:: https://pepy.tech/badge/networth/month
+    :target: https://pepy.tech/project/networth
+
+.. image:: https://img.shields.io/pypi/v/networth.svg
+    :target: https://pypi.python.org/pypi/networth
+
+.. image:: https://img.shields.io/pypi/pyversions/networth.svg
+    :target: https://pypi.python.org/pypi/networth/
+
+
+| Version: 1.2
+| Released: 2023-04-22
 
 *Networth* works with `Avendesora <https://avendesora.readthedocs.io>`_ to 
 generate a summary of your networth. *Networth* reads *estimated_value* fields 
 from *Avendesora* accounts and summarizes the result.  It is often used with, 
 and shares fields with, `PostMortem <https://github.com/KenKundert/postmortem>`_.
 Works with data services to download up-to-date prices for securities and 
 cryptocurrencies.
@@ -88,15 +98,16 @@
     tokens:
         A dictionary of crytpocurrency tokens that should be available for use.
         The key of the dictionary is the token symbol, the value is the category 
         it should associate with.
 
     ttl:
         Cache time to live.  If the cache is older than this time, it is 
-        refreshed.  Here are example times: 600s, 10m, 6h, 1d.
+        refreshed.  Here are example times: 600s, 10m, 6h, 1d.  The default is 
+        10m.
 
     api key:
         The coin prices are downloaded from cryptocompare.com. Specifying the 
         API key is optional.  Providing an API key increases your limits, but 
         limits are generally not a problem for *Networth* because it is run so 
         infrequently.
 
@@ -128,14 +139,21 @@
     A dictionary containing information about precious metals prices that are to 
     be downloaded from metals-api.com.  This dictionary takes the same fields as 
     *cryptocompare*.  An API key is required.
 
     To avoid caching issues it is recommended that *metals* files be placed in 
     the shared *config* file if multiple profiles need it.
 
+    Metals API has dropped their free tier.
+
+metals live:
+    A dictionary containing information about precious metals prices that are to 
+    be downloaded from metals-api.com.  This dictionary only requires the 
+    *tokens* field. An API key is not required.
+
 estimated value overrides file:
     A path to a file of *estimated_value* overrides. Give as a NestedText file 
     that contains a dictionary of dictionaries.  The keys for the top level are 
     account names, and the value contains the estimated value dictionary that 
     would normally be found in the *Avendesora* accounts file.
 
 
@@ -320,16 +338,19 @@
 
     plot-networth -l
 
 
 Releases
 --------
 **Latest Development Version**:
-    | Version: 1.1.0
-    | Released: 2021-03-11
+    | Version: 1.2
+    | Released: 2023-04-22
+
+**1.2 (2023-04-22)**:
+    - add metals.live data service
 
 **1.1 (2021-03-11)**:
     - clean up and minor refinements.
 
 **1.0 (2021-02-13)**:
     - Add *estimated value overrides file* setting.
     - Add --details option.
```

### Comparing `networth-1.1.0/networth` & `networth-1.2/networth`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,30 @@
 You can also specify an argument of the form AAA=NN where AAA is the name of 
 a security and NN is the number of shares. This amount is added to the account 
 'command line'.
 
 The prices and log files can be found in {cache_dir}.
 """
 
+# License {{{1
+# Copyright (C) 2016-2023 Kenneth S. Kundert
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see http://www.gnu.org/licenses/.
+
 # Imports {{{1
 from appdirs import user_config_dir, user_cache_dir, user_data_dir
 from avendesora import PasswordGenerator, PasswordError
 import nestedtext as nt
 import voluptuous
 from docopt import docopt
 from inform import (
@@ -50,16 +66,16 @@
 from operator import itemgetter
 import arrow
 import requests
 from pathlib import Path
 from quantiphy import Quantity, InvalidNumber, UnitConversion
 from quantiphy_eval import evaluate, initialize, rm_commas
 
-__version__ = "1.1.0"
-__released__ = "2021-03-11"
+__version__ = "1.2"
+__released__ = "2023-04-22"
 
 # Settings {{{1
 # These can be overridden in ~/.config/networth/config
 prog_name = 'networth'
 config_filename = 'config'
 default_profile = None
 aliases = {}
@@ -170,14 +186,16 @@
             return int(v)
     except:
         pass
     raise voluptuous.Invalid('expected integer')
 
 # interpret dict value {{{2
 def convert_to_dict(d):
+    if not d:
+        d = {}
     new = {}
     for k, v in d.items():
         if not is_str(k) or not is_str(v):
             raise voluptuous.Invalid('expected dictionary of strings')
         new[k.replace(' ', '_')] = v
     return new
 
@@ -206,25 +224,32 @@
 
 # colored bar {{{2
 def colored_bar(value, width):
     return colorize(value, render_bar(abs(value), width))
 
 # resolve_value {{{2
 # Evaluate & convert (expression, coin, security, mortgage) to final value.
-def resolve_value(key, value):
+def resolve_value(key, value, account_name):
     try:
         value = evaluate(rm_commas(value))
     except Exception:
         try:
             value = ' '.join(value.split())
         except AttributeError:
             pass
 
     if key in tokens:
         if key in prices:
+            if value:
+                accounts = raw_accounts.get(key, [])
+                try:
+                    accounts.append(f'{Quantity(value):p} in {account_name}')
+                except InvalidNumber as e:
+                    raise Error(e, culprit=account_name)
+                raw_accounts[key] = accounts
             raw_totals[key] = raw_totals.get(key, Quantity(0, key)).add(value)
             value = Quantity(
                 float(value)*prices[key],
                 prices[key]
             )
             key = tokens[key]
         else:
@@ -320,15 +345,15 @@
     def get_prices(self):
         if not self.tokens:
             return {}
 
         cache_valid = False
         prices_cache = cache_dir / self.NAME
         if prices_cache and prices_cache.exists():
-            age = now.timestamp - prices_cache.stat().st_mtime
+            age = now.timestamp() - prices_cache.stat().st_mtime
             cache_valid = age < self.ttl
         if use_caches and cache_valid:
             narrate(f'{self.NAME} prices are current:', prices_cache)
             contents = prices_cache.read_text()
             return Quantity.extract(contents)
         else:
             # download latest asset prices from metals-api.com
@@ -349,22 +374,23 @@
             # extract prices
             try:
                 data = r.json()
             except:
                 raise Error(f'{self.NAME} price download was garbled.')
             prices = self.extract_prices(data)
 
-            if prices_cache:
+            if prices_cache and prices:
                 contents = '\n'.join(
                     '{} = {}'.format(k,v.fixed(prec='full'))
                     for k,v in prices.items()
                 )
                 narrate(f'updating {self.NAME} prices:', prices_cache)
                 prices_cache.write_text(contents)
-            return prices
+
+            return prices if prices else {}
 
     @classmethod
     def services(cls):
         for sub in cls.__subclasses__():
             yield sub
 
     @classmethod
@@ -436,29 +462,58 @@
             access_key = self.api_key,
             base = 'USD',
             symbols = ','.join(self.tokens.keys())
         )
         return url, params
 
     def extract_prices(self, data):
+        data = data['data']
         if not data['success']:
             raise Error(
                 'metals-api price download failed.',
                 codicil = data['error']['info']
             )
+
         assert data['base'] == 'USD'
-        assert data['unit'] == 'per ounce'
+        # assert data['unit'] == 'per ounce'
         assert data['rates']['USD'] == 1
         return {
             k: Dollars(1/float(v))
             for k, v in data['rates'].items()
             if k != 'USD'
         }
 
 
+# MetalsLive class {{{2
+class MetalsLive(DataService):
+    NAME = 'metals_live'
+
+    def get_url(self):
+        base_url = 'http://api.metals.live'
+        path = 'v1/spot'
+            # returns current price of gold, silver, platinum, palladium
+        url = '/'.join([base_url, path])
+        params = dict(
+            api_key = "<api key>",
+        )
+        params = None  # params not needed for free tier
+        return url, params
+
+    def extract_prices(self, data):
+        map_names = dict(
+            gold='XAU', silver='XAG', platinum='XPT', palladium='XPD'
+        )
+        return {
+            map_names[k]: Dollars(v)
+            for each in data
+            for k, v in each.items()
+            if k != 'timestamp'
+        }
+
+
 # TwelveData class {{{2
 class TwelveData(DataService):
     NAME = 'twelve_data'
 
     def get_url(self):
         url = 'https://api.twelvedata.com/time_series'
         params = dict(
@@ -477,14 +532,40 @@
         else:
             return {
                 name: Dollars(info['values'][0]['close'])
                 for name, info in data.items()
             }
 
 
+# Nasdac class {{{2
+class Nasdac(DataService):
+    NAME = 'nasdaq'
+    # This one was never completed. Do not use.
+
+    def get_url(self):
+        # see https://blog.data.nasdaq.com/api-for-commodity-data
+        url = 'https://data.nasdaq.com/api/v3/datasets/LBMA/GOLD'
+        # url = 'https://data.nasdaq.com/api/v3/datasets/WGC/GOLD_DAILY_USD'
+        params = dict(
+            api_key = self.api_key
+        )
+        return url, params
+
+    def extract_prices(self, data):
+        # form of data changes based on whether you ask for one or many tokens
+        if len(self.tokens) == 1:
+            name = ''.join(self.tokens.keys())
+            return {name: Dollars(data['values'][0]['close'])}
+        else:
+            return {
+                name: Dollars(info['values'][0]['close'])
+                for name, info in data.items()
+            }
+
+
 # Initialization {{{1
 try:
     settings_dir = Path(user_config_dir(prog_name))
     cache_dir = Path(user_cache_dir(prog_name))
     cache_dir.mkdir(parents=True, exist_ok=True)
     Quantity.set_prefs(prec='full', strip_radix=True)
     inform = Inform(logfile=cache_dir / 'log')
@@ -593,14 +674,15 @@
     if insecure:
         requests.packages.urllib3.disable_warnings()
     use_proxy = cmdline['--proxy']
     if not use_proxy:
         proxies = None
     show_prices = cmdline['--prices']
     use_caches = not cmdline['--clear-cache']
+    show_all = cmdline['--all']
     show_details = cmdline['--details']
     write_data = cmdline['--write-data']
     inform.quiet = write_data
 
     # Read profile settings {{{1
     config_filepath = Path(user_config_dir(prog_name), profile + '.prof')
     if config_filepath.exists():
@@ -647,14 +729,15 @@
         if service.NAME in profile_settings:
             warn('must be specified in shared config file.', culprit=service.NAME)
 
     # Build account summaries {{{1
     totals_by_type = {}
     totals_by_account = {}
     raw_totals = {}
+    raw_accounts = {}
     accounts = []
     total_assets = Quantity(0, '$')
     total_debt = Quantity(0, '$')
     grand_total = Quantity(0, '$')
     width = 0
 
     # accounts in Avendesora {{{2
@@ -694,15 +777,15 @@
             keys_differ = False
             for key, value in data.items():
                     if key == value_updated_subfieldname:
                         updated = value
                         continue
 
                     orig_key = key
-                    key, value = resolve_value(key, value)
+                    key, value = resolve_value(key, value, account_name)
                     if value.units == '$':
                         total = total.add(value)
                     else:
                         odd_units = True
                     contents[key] = value.add(contents.get(key, 0))
                     if value > 0:
                         details[orig_key] = value
@@ -734,15 +817,15 @@
                 if age and age > max_account_value_age:
                     desc += f' ({age//30} months old)'
             summary = join(
                 total, desc.replace('_', ' '),
                 #template=('{:7q} {}', '{:7q}'), remove=(None,'') ksk
                 template=('{:10,.0p} {}', '{:10,.0p}'), remove=(None,'')
             )
-            if total or cmdline['--all']:
+            if total or show_all:
                 accounts.append((account_name, total, summary, details))
 
             # sum assets and debts {{{3
             if total > 0:
                 total_assets = total_assets.add(total)
             else:
                 total_debt = total_debt.add(-total)
@@ -757,15 +840,15 @@
         total = Quantity(0, '$')
         details = {}
         keys_differ = False
 
         for orig_key, value in extras.items():
             # sum the data {{{3
             odd_units = False
-            key, value = resolve_value(orig_key, value)
+            key, value = resolve_value(orig_key, value, account_name)
             if value.units == '$':
                 total = total.add(value)
             else:
                 odd_units = True
             if value > 0:
                 details[orig_key] = value
             if key != orig_key:
@@ -806,28 +889,41 @@
                 '   {2:>15.3p}: {1:#,.2p}/{0}',
                 '   {0:>15}: {1:#,.2p}/{0}'
             ),
             remove = None,
         )
         if prices:
             display('Prices:')
-            for k, v in prices.items():
+            #for k, v in prices.items():
+            for k in sorted(prices):
+                v = prices[k]
                 if k != 'USD':
+                    raw_total = raw_totals.get(k)
+                    if not raw_total:
+                        if show_all:
+                            raw_total = None
+                        else:
+                            continue
                     display(k, v, raw_totals.get(k), **fmt)
+                    if show_details and k in raw_accounts:
+                        if len(raw_accounts[k]) > 1:
+                            for each in raw_accounts[k]:
+                                display((3+15+1)*' ', each)
             display()
 
     # Summarize by account {{{1
     display('Assets By Account:')
     for name, total, summary, details in sorted(accounts, **sort_mode):
         display(f'{name:>{width+2}s}: {summary}')
         totals_by_account[name] = total
         if show_details and details:
-            for key in details:
-                value = details[key]
-                display(f'{"":>{width+2}s}  {value:10,.0p} {key}')
+            if len(details) > 1:
+                for key in details:
+                    value = details[key]
+                    display(f'{"":>{width+2}s}  {value:10,.0p} {key}')
 
     # Summarize by investment type {{{1
     display('\nAssets By Type:')
     largest_share = max(abs(v) for v in totals_by_type.values() if v.units == '$')
     barwidth = screen_width - width - 19
     for asset_type in sorted(totals_by_type, key=lambda k: totals_by_type[k], reverse=True):
         value = totals_by_type[asset_type]
```

### Comparing `networth-1.1.0/networth.egg-info/PKG-INFO` & `networth-1.2/networth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,393 +1,411 @@
 Metadata-Version: 2.1
 Name: networth
-Version: 1.1.0
+Version: 1.2
 Summary: Summarize net worth
 Home-page: https://github.com/kenkundert/networth
+Download-URL: https://github.com/kenkundert/networth/tarball/master
 Author: Ken Kundert
 Author-email: networth@nurdletech.com
 License: GPLv3+
-Download-URL: https://github.com/kenkundert/networth/tarball/master
-Description: Networth: Summarize Your Net Worth
-        ==================================
-        
-        | Version: 1.1.0
-        | Released: 2021-03-11
-        
-        *Networth* works with `Avendesora <https://avendesora.readthedocs.io>`_ to 
-        generate a summary of your networth. *Networth* reads *estimated_value* fields 
-        from *Avendesora* accounts and summarizes the result.  It is often used with, 
-        and shares fields with, `PostMortem <https://github.com/KenKundert/postmortem>`_.
-        Works with data services to download up-to-date prices for securities and 
-        cryptocurrencies.
-        
-        Please report all bugs and suggestions to networth@nurdletech.com
-        
-        Getting Started
-        ---------------
-        
-        You download and install *Networth* with::
-        
-            pip3 install --user networth
-        
-        Once installed, you will need at least two configuration files. The 
-        configuration files are `NestedText <https://nestedtext.readthedocs.io>`_.  The 
-        first file contains settings that are shared between all profiles.  It is 
-        ~/.config/networth/config.  The remaining files are specific to profiles.  You 
-        would generally have one profile for yourself, but you might also have profiles 
-        for organizations or people that you are monitoring.
-        
-        Profile files have a .prof suffix, and the name of the profile is the name of 
-        the profile file without the suffix.
-        
-        In general, any setting may be in either the config file or the profile file.  
-        However, the following setting should in the config file:
-        
-        default profile:
-            A string that contains the name of the profile to use if the one is not 
-            explicitly specified on the command line.
-        
-        In addition, the following settings are available:
-        
-        avendesora fieldname:
-            The name of the *Avendesora* account field that contains the networth 
-            information.  Typically *estimated_value*.
-        
-        value updated subfieldname:
-            The name of the subfield of *estimated_value* that contains the date the 
-            value was last updated.  Typically *updated*.
-        
-        max account value age:
-            Number of days. Values that are older than this are called out as being 
-            stale. Default is 120 days.
-        
-        date formats:
-            The list of allowed date formats. May be specified as a list or as a string
-            string that contains the allowed date formats separated by white space.  Any 
-            spaces is a specific format is replaced by an underscore so that it is not 
-            confused as more than one format. For example a format of 'MMMM YYYY' would 
-            be represented as 'MMMM_YYYY'. The formats allowed are those supported by 
-            Arrow.
-        
-            By default the following formats are accepted: 'MMMM YYYY', 'MMM YYYY', 
-            'YYYY-M-D', and 'YYMMDD'. So the following dates would be accepted: 'January 
-            2019', 'Jan 2019', '2019-1-1' and '190101'.
-        
-        asset color:
-            The color to used for positive values. May be black, white, blue, cyan, 
-            green, red, magenta, or yellow. The default is green.
-        
-        debt color:
-            The color to used for negative values. May be black, white, blue, cyan, 
-            green, red, magenta, or yellow. The default is red.
-        
-        screen width:
-            An integer that contains the width of the screen.
-        
-        aliases:
-            A dictionary that is used to map an account name to something that is easier 
-            to read.
-        
-        cryptocompare:
-            A dictionary containing information about cryptocurrency prices that are to 
-            be downloaded from cryptocompare.com.
-        
-            To avoid caching issues it is recommended that *cryptocompare* files be 
-            placed in the shared *config* file if multiple profiles need it.
-        
-            tokens:
-                A dictionary of crytpocurrency tokens that should be available for use.
-                The key of the dictionary is the token symbol, the value is the category 
-                it should associate with.
-        
-            ttl:
-                Cache time to live.  If the cache is older than this time, it is 
-                refreshed.  Here are example times: 600s, 10m, 6h, 1d.
-        
-            api key:
-                The coin prices are downloaded from cryptocompare.com. Specifying the 
-                API key is optional.  Providing an API key increases your limits, but 
-                limits are generally not a problem for *Networth* because it is run so 
-                infrequently.
-        
-            api key account field:
-                You may place the API key in *Avendesora* and use this key to specify the 
-                account and field name for the API key.
-        
-        iexcloud:
-            A dictionary containing information about security prices that are to be 
-            downloaded from iexcloud.io.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *iexcloud* files be placed in 
-            the shared *config* file if multiple profiles need it.
-        
-        twelve data:
-            A dictionary containing information about security prices that are to be 
-            downloaded from twelvedata.com.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *twelvedata* files be placed 
-            in the shared *config* file if multiple profiles need it.
-        
-            *Twelve Data* provides real time values, but have very low limits unless you 
-            get an expensive subscription.  If you do not have a subscription, it is 
-            recommended that you limit the number of tokens to 8 or less.
-        
-        metals api:
-            A dictionary containing information about precious metals prices that are to 
-            be downloaded from metals-api.com.  This dictionary takes the same fields as 
-            *cryptocompare*.  An API key is required.
-        
-            To avoid caching issues it is recommended that *metals* files be placed in 
-            the shared *config* file if multiple profiles need it.
-        
-        estimated value overrides file:
-            A path to a file of *estimated_value* overrides. Give as a NestedText file 
-            that contains a dictionary of dictionaries.  The keys for the top level are 
-            account names, and the value contains the estimated value dictionary that 
-            would normally be found in the *Avendesora* accounts file.
-        
-        
-        Example Configuration Files
-        ---------------------------
-        
-        Here is an example *config* file::
-        
-            default profile: me
-        
-            # account value settings
-            avendesora fieldname: estimated_value
-            value updated subfieldname: updated
-            max account value age: 120
-            date formats: M/D/YY M/D/YYYY
-        
-            # bar settings
-            screen width: 110
-        
-            # cryptocurrency prices
-            cryptocompare:
-                tokens:
-                    USD: cash
-                    BTC: cryptocurrency
-                    ETH: cryptocurrency
-        
-            # securities prices
-            iexcloud:
-                api key: pk_9eb3acfc7dbe4055a795ff179d46a980
-                tokens:
-                    GOOG: equities
-                    AMZN: equities
-                    GBTC: cryptocurrency
-        
-        Here is a example profile file::
-        
-            # account aliases
-            aliases:
-                quickenloans: mortgage
-                wellsfargo: wells fargo
-        
-        
-        Here is a example estimated value overrides file::
-        
-            chase:
-                updated: February 2021
-                cash:
-                    > $4,425.71 +       # checking
-                    > $1,896.26         # savings
-        
-        
-        Estimated Values
-        ----------------
-        
-        Next, you need to add *estimated_value* fields to your *Avendesora* accounts, 
-        the value of which is a dictionary. It may contain a *updated* subfield that 
-        gives the date the value was last updated.  In addition, it may contain 
-        subfields for various asset classes or coins or securities.  The values may 
-        either be real numbers or strings that contain quantities (values plus units).  
-        Here are some examples::
-        
-            class ChaseBank(Account):
-                ...
-                estimated_value = dict(updated='December 2018', cash=2181.16+5121.79)
-        
-            class QuickenLoans(Account):
-                ...
-                estimated_value = dict(updated='October 2018', real_estate='-$294,058')
-        
-            class Vanguard(Account):
-                ...
-                estimated_value = dict(updated='November 2018', retirement='$74,327')
-        
-            class TDAmeritrade(Account):
-                ...
-                estimated_value = dict( updated='November 2018', retirement='$74,327+$111,554')
-        
-            class Fidelity(Account):
-                ...
-                estimated_value = dict( updated='November 2018', retirement='''
-                    $62,976.22 +    # 401k
-                    $26,704.85      # IRA
-                ''')
-        
-            class UnitedAirlines(Account):
-                ...
-                estimated_value = dict(updated='July 2018', miles='7,384_miles')
-        
-            class CoinBase(Account):
-                ...
-                estimated_value = dict(updated='August 2018', ETH=2, BTC=4, cash=24.52)
-        
-            class TD_Ameritrade(Account):
-                ...
-                estimated_value = dict(updated='January 2019', GOOG=10, AMZN=5, cash=327.53)
-        
-        The value of securities are given is number of shares. The value given for 
-        cryptocurrencies is number of tokens. All other values are assumed to be in 
-        dollars if the units are not given. If the units are given and they are not 
-        dollars (such as miles for frequent flier programs), then those values are 
-        summarized but not included in your total networth.
-        
-        Specifying the *updated* date is optional. If specified, then *networth* will 
-        indicate the values as stale if they exceed *max_account_value_age*.
-        
-        It is also specify information about a loan, and *networth* will compute its 
-        current balance.  This is done by giving the principal on a particular date, the 
-        date for the given principal, the monthly payments, the interest rate, and 
-        optionally, the share. The rate and the share can be given in percent, meaning 
-        that an rate of 4% can either be specified as 4% or as 0.04. Similarly a share 
-        half share can be indicated as 50% or 0.5.  For example::
-        
-            class QuickenLoans(Account):
-                ...
-                estimated_value = dict(
-                    real_estate = '''
-                        principal=-$294,058
-                        date=09/04/2013
-                        payment=$1,500.00
-                        rate=4.375%
-                        share=50%
-                    ''',
-                )
-        
-        the key=value pairs can be separated by any white space, but there must be no
-        white space surrounding the = sign. For mortgages that you owe, the principal 
-        should be negative. You can also use this feature to describe an automatic 
-        savings plan into an interest bearing account.  In this case the principal would 
-        be your starting balance and the payment would be your monthly investment 
-        amount.  In this case the starting balance would be positive.
-        
-        
-        Usage
-        -----
-        
-        When running the command, you may specify a profile. If you do not, you get the 
-        default profile.  For example::
-        
-            > networth me
-            By Account:
-                    betterment:    $22k equities=$9k, cash=$3k, retirement=$9k
-                         chase:     $7k cash
-                     southwest:      $0 miles=78kmiles
-                      coindesk:  $15.3k cryptocurrency
-        
-            By Type:
-                cryptocurrency:  $15.3k (35.3%) ██████████████████████████████████████████
-                          cash:    $10k (23.1%) ███████████████████████████████
-                      equities:     $9k (20.8%) ███████████████████████████
-                    retirement:     $9k (20.8%) ███████████████████████████
-        
-                         TOTAL:  $43.3k (assets = $43.3k, debt = $0)
-        
-        In this run, the values associated with the various asset classes (ex. equities, 
-        cash, retirement, etc.) are taken as is. As such, you must be diligent about 
-        keeping these values up to date, which is a manual operation. You might consider 
-        updating your *estimated values* every 3-6 months.  However the current prices 
-        for your configured securities and cryptocurrencies are downloaded and 
-        multiplied by the given number of shares or tokens to get the up-to-date values 
-        of your equities and cryptocurrency holdings. Thus you only need update them 
-        after a transaction. Finally, mortgage balances are also kept up to date. You 
-        only need update mortgages if you decide to change the payment amount in order 
-        to pay off the loan faster.
-        
-        
-        History
-        -------
-        
-        If you would like to be able to plot your net worth over time you run the 
-        following regularly::
-        
-            networth -w <profile>
-        
-        Each time you do, the networth values are added to a data file 
-        (~/.local/share/networth/<profile>.nt).
-        
-        You can then plot the historical values using::
-        
-            plot-networth <name>...
-        
-        You can get a list of the values you can plot using::
-        
-            plot-networth -l
-        
-        
-        Releases
-        --------
-        **Latest Development Version**:
-            | Version: 1.1.0
-            | Released: 2021-03-11
-        
-        **1.1 (2021-03-11)**:
-            - clean up and minor refinements.
-        
-        **1.0 (2021-02-13)**:
-            - Add *estimated value overrides file* setting.
-            - Add --details option.
-            - Add --write-data option.
-            - Add *plot-networth* command.
-            - Allow categories to be specified for downloaded token prices.
-        
-        **0.8 (2020-10-10)**:
-            - Add support for downloading prices of precious metals.
-            - Switch to *NestedText* for the settings files.
-        
-        **0.7 (2020-03-06)**:
-            - Now uses `QuantiPhy Eval <https://github.com/KenKundert/quantiphy_eval>`_ 
-              to allow you to use expressions within strings for estimated values.
-        
-        **0.6 (2020-01-08)**:
-            - Added --prices and --clear-cache command line options.
-            - Support using a proxy.
-        
-        **0.5 (2019-07-18)**:
-        
-        **0.4 (2019-06-15)**:
-            - Convert to using new IEXcloud API for downloading security prices.
-        
-        **0.3 (2019-04-20)**:
-            - Allow arbitrary date format in mortgages.
-            - Improve error reporting.
-            - Change the sign of the principal in mortgages.
-        
-        **0.1 (2019-03-23)**:
-            - Initial release.
-            - Add mortgage balance calculations.
-        
-        **0.0 (2019-01-31)**:
-            - Initial version.
-        
-        
 Keywords: networth
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Networth — Summarize Your Net Worth
+===================================
+
+.. image:: https://pepy.tech/badge/networth/month
+    :target: https://pepy.tech/project/networth
+
+.. image:: https://img.shields.io/pypi/v/networth.svg
+    :target: https://pypi.python.org/pypi/networth
+
+.. image:: https://img.shields.io/pypi/pyversions/networth.svg
+    :target: https://pypi.python.org/pypi/networth/
+
+
+| Version: 1.2
+| Released: 2023-04-22
+
+*Networth* works with `Avendesora <https://avendesora.readthedocs.io>`_ to 
+generate a summary of your networth. *Networth* reads *estimated_value* fields 
+from *Avendesora* accounts and summarizes the result.  It is often used with, 
+and shares fields with, `PostMortem <https://github.com/KenKundert/postmortem>`_.
+Works with data services to download up-to-date prices for securities and 
+cryptocurrencies.
+
+Please report all bugs and suggestions to networth@nurdletech.com
+
+Getting Started
+---------------
+
+You download and install *Networth* with::
+
+    pip3 install --user networth
+
+Once installed, you will need at least two configuration files. The 
+configuration files are `NestedText <https://nestedtext.readthedocs.io>`_.  The 
+first file contains settings that are shared between all profiles.  It is 
+~/.config/networth/config.  The remaining files are specific to profiles.  You 
+would generally have one profile for yourself, but you might also have profiles 
+for organizations or people that you are monitoring.
+
+Profile files have a .prof suffix, and the name of the profile is the name of 
+the profile file without the suffix.
+
+In general, any setting may be in either the config file or the profile file.  
+However, the following setting should in the config file:
+
+default profile:
+    A string that contains the name of the profile to use if the one is not 
+    explicitly specified on the command line.
+
+In addition, the following settings are available:
+
+avendesora fieldname:
+    The name of the *Avendesora* account field that contains the networth 
+    information.  Typically *estimated_value*.
+
+value updated subfieldname:
+    The name of the subfield of *estimated_value* that contains the date the 
+    value was last updated.  Typically *updated*.
+
+max account value age:
+    Number of days. Values that are older than this are called out as being 
+    stale. Default is 120 days.
+
+date formats:
+    The list of allowed date formats. May be specified as a list or as a string
+    string that contains the allowed date formats separated by white space.  Any 
+    spaces is a specific format is replaced by an underscore so that it is not 
+    confused as more than one format. For example a format of 'MMMM YYYY' would 
+    be represented as 'MMMM_YYYY'. The formats allowed are those supported by 
+    Arrow.
+
+    By default the following formats are accepted: 'MMMM YYYY', 'MMM YYYY', 
+    'YYYY-M-D', and 'YYMMDD'. So the following dates would be accepted: 'January 
+    2019', 'Jan 2019', '2019-1-1' and '190101'.
+
+asset color:
+    The color to used for positive values. May be black, white, blue, cyan, 
+    green, red, magenta, or yellow. The default is green.
+
+debt color:
+    The color to used for negative values. May be black, white, blue, cyan, 
+    green, red, magenta, or yellow. The default is red.
+
+screen width:
+    An integer that contains the width of the screen.
+
+aliases:
+    A dictionary that is used to map an account name to something that is easier 
+    to read.
+
+cryptocompare:
+    A dictionary containing information about cryptocurrency prices that are to 
+    be downloaded from cryptocompare.com.
+
+    To avoid caching issues it is recommended that *cryptocompare* files be 
+    placed in the shared *config* file if multiple profiles need it.
+
+    tokens:
+        A dictionary of crytpocurrency tokens that should be available for use.
+        The key of the dictionary is the token symbol, the value is the category 
+        it should associate with.
+
+    ttl:
+        Cache time to live.  If the cache is older than this time, it is 
+        refreshed.  Here are example times: 600s, 10m, 6h, 1d.  The default is 
+        10m.
+
+    api key:
+        The coin prices are downloaded from cryptocompare.com. Specifying the 
+        API key is optional.  Providing an API key increases your limits, but 
+        limits are generally not a problem for *Networth* because it is run so 
+        infrequently.
+
+    api key account field:
+        You may place the API key in *Avendesora* and use this key to specify the 
+        account and field name for the API key.
+
+iexcloud:
+    A dictionary containing information about security prices that are to be 
+    downloaded from iexcloud.io.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *iexcloud* files be placed in 
+    the shared *config* file if multiple profiles need it.
+
+twelve data:
+    A dictionary containing information about security prices that are to be 
+    downloaded from twelvedata.com.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *twelvedata* files be placed 
+    in the shared *config* file if multiple profiles need it.
+
+    *Twelve Data* provides real time values, but have very low limits unless you 
+    get an expensive subscription.  If you do not have a subscription, it is 
+    recommended that you limit the number of tokens to 8 or less.
+
+metals api:
+    A dictionary containing information about precious metals prices that are to 
+    be downloaded from metals-api.com.  This dictionary takes the same fields as 
+    *cryptocompare*.  An API key is required.
+
+    To avoid caching issues it is recommended that *metals* files be placed in 
+    the shared *config* file if multiple profiles need it.
+
+    Metals API has dropped their free tier.
+
+metals live:
+    A dictionary containing information about precious metals prices that are to 
+    be downloaded from metals-api.com.  This dictionary only requires the 
+    *tokens* field. An API key is not required.
+
+estimated value overrides file:
+    A path to a file of *estimated_value* overrides. Give as a NestedText file 
+    that contains a dictionary of dictionaries.  The keys for the top level are 
+    account names, and the value contains the estimated value dictionary that 
+    would normally be found in the *Avendesora* accounts file.
+
+
+Example Configuration Files
+---------------------------
+
+Here is an example *config* file::
+
+    default profile: me
+
+    # account value settings
+    avendesora fieldname: estimated_value
+    value updated subfieldname: updated
+    max account value age: 120
+    date formats: M/D/YY M/D/YYYY
+
+    # bar settings
+    screen width: 110
+
+    # cryptocurrency prices
+    cryptocompare:
+        tokens:
+            USD: cash
+            BTC: cryptocurrency
+            ETH: cryptocurrency
+
+    # securities prices
+    iexcloud:
+        api key: pk_9eb3acfc7dbe4055a795ff179d46a980
+        tokens:
+            GOOG: equities
+            AMZN: equities
+            GBTC: cryptocurrency
+
+Here is a example profile file::
+
+    # account aliases
+    aliases:
+        quickenloans: mortgage
+        wellsfargo: wells fargo
+
+
+Here is a example estimated value overrides file::
+
+    chase:
+        updated: February 2021
+        cash:
+            > $4,425.71 +       # checking
+            > $1,896.26         # savings
+
+
+Estimated Values
+----------------
+
+Next, you need to add *estimated_value* fields to your *Avendesora* accounts, 
+the value of which is a dictionary. It may contain a *updated* subfield that 
+gives the date the value was last updated.  In addition, it may contain 
+subfields for various asset classes or coins or securities.  The values may 
+either be real numbers or strings that contain quantities (values plus units).  
+Here are some examples::
+
+    class ChaseBank(Account):
+        ...
+        estimated_value = dict(updated='December 2018', cash=2181.16+5121.79)
+
+    class QuickenLoans(Account):
+        ...
+        estimated_value = dict(updated='October 2018', real_estate='-$294,058')
+
+    class Vanguard(Account):
+        ...
+        estimated_value = dict(updated='November 2018', retirement='$74,327')
+
+    class TDAmeritrade(Account):
+        ...
+        estimated_value = dict( updated='November 2018', retirement='$74,327+$111,554')
+
+    class Fidelity(Account):
+        ...
+        estimated_value = dict( updated='November 2018', retirement='''
+            $62,976.22 +    # 401k
+            $26,704.85      # IRA
+        ''')
+
+    class UnitedAirlines(Account):
+        ...
+        estimated_value = dict(updated='July 2018', miles='7,384_miles')
+
+    class CoinBase(Account):
+        ...
+        estimated_value = dict(updated='August 2018', ETH=2, BTC=4, cash=24.52)
+
+    class TD_Ameritrade(Account):
+        ...
+        estimated_value = dict(updated='January 2019', GOOG=10, AMZN=5, cash=327.53)
+
+The value of securities are given is number of shares. The value given for 
+cryptocurrencies is number of tokens. All other values are assumed to be in 
+dollars if the units are not given. If the units are given and they are not 
+dollars (such as miles for frequent flier programs), then those values are 
+summarized but not included in your total networth.
+
+Specifying the *updated* date is optional. If specified, then *networth* will 
+indicate the values as stale if they exceed *max_account_value_age*.
+
+It is also specify information about a loan, and *networth* will compute its 
+current balance.  This is done by giving the principal on a particular date, the 
+date for the given principal, the monthly payments, the interest rate, and 
+optionally, the share. The rate and the share can be given in percent, meaning 
+that an rate of 4% can either be specified as 4% or as 0.04. Similarly a share 
+half share can be indicated as 50% or 0.5.  For example::
+
+    class QuickenLoans(Account):
+        ...
+        estimated_value = dict(
+            real_estate = '''
+                principal=-$294,058
+                date=09/04/2013
+                payment=$1,500.00
+                rate=4.375%
+                share=50%
+            ''',
+        )
+
+the key=value pairs can be separated by any white space, but there must be no
+white space surrounding the = sign. For mortgages that you owe, the principal 
+should be negative. You can also use this feature to describe an automatic 
+savings plan into an interest bearing account.  In this case the principal would 
+be your starting balance and the payment would be your monthly investment 
+amount.  In this case the starting balance would be positive.
+
+
+Usage
+-----
+
+When running the command, you may specify a profile. If you do not, you get the 
+default profile.  For example::
+
+    > networth me
+    By Account:
+            betterment:    $22k equities=$9k, cash=$3k, retirement=$9k
+                 chase:     $7k cash
+             southwest:      $0 miles=78kmiles
+              coindesk:  $15.3k cryptocurrency
+
+    By Type:
+        cryptocurrency:  $15.3k (35.3%) ██████████████████████████████████████████
+                  cash:    $10k (23.1%) ███████████████████████████████
+              equities:     $9k (20.8%) ███████████████████████████
+            retirement:     $9k (20.8%) ███████████████████████████
+
+                 TOTAL:  $43.3k (assets = $43.3k, debt = $0)
+
+In this run, the values associated with the various asset classes (ex. equities, 
+cash, retirement, etc.) are taken as is. As such, you must be diligent about 
+keeping these values up to date, which is a manual operation. You might consider 
+updating your *estimated values* every 3-6 months.  However the current prices 
+for your configured securities and cryptocurrencies are downloaded and 
+multiplied by the given number of shares or tokens to get the up-to-date values 
+of your equities and cryptocurrency holdings. Thus you only need update them 
+after a transaction. Finally, mortgage balances are also kept up to date. You 
+only need update mortgages if you decide to change the payment amount in order 
+to pay off the loan faster.
+
+
+History
+-------
+
+If you would like to be able to plot your net worth over time you run the 
+following regularly::
+
+    networth -w <profile>
+
+Each time you do, the networth values are added to a data file 
+(~/.local/share/networth/<profile>.nt).
+
+You can then plot the historical values using::
+
+    plot-networth <name>...
+
+You can get a list of the values you can plot using::
+
+    plot-networth -l
+
+
+Releases
+--------
+**Latest Development Version**:
+    | Version: 1.2
+    | Released: 2023-04-22
+
+**1.2 (2023-04-22)**:
+    - add metals.live data service
+
+**1.1 (2021-03-11)**:
+    - clean up and minor refinements.
+
+**1.0 (2021-02-13)**:
+    - Add *estimated value overrides file* setting.
+    - Add --details option.
+    - Add --write-data option.
+    - Add *plot-networth* command.
+    - Allow categories to be specified for downloaded token prices.
+
+**0.8 (2020-10-10)**:
+    - Add support for downloading prices of precious metals.
+    - Switch to *NestedText* for the settings files.
+
+**0.7 (2020-03-06)**:
+    - Now uses `QuantiPhy Eval <https://github.com/KenKundert/quantiphy_eval>`_ 
+      to allow you to use expressions within strings for estimated values.
+
+**0.6 (2020-01-08)**:
+    - Added --prices and --clear-cache command line options.
+    - Support using a proxy.
+
+**0.5 (2019-07-18)**:
+
+**0.4 (2019-06-15)**:
+    - Convert to using new IEXcloud API for downloading security prices.
+
+**0.3 (2019-04-20)**:
+    - Allow arbitrary date format in mortgages.
+    - Improve error reporting.
+    - Change the sign of the principal in mortgages.
+
+**0.1 (2019-03-23)**:
+    - Initial release.
+    - Add mortgage balance calculations.
+
+**0.0 (2019-01-31)**:
+    - Initial version.
+
```

### Comparing `networth-1.1.0/plot-networth` & `networth-1.2/plot-networth`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,38 @@
     -a, --accounts                      plot all accounts
     -t, --types                         plot all asset types
     -g, --gross                         plot gross and net values
     -s <file>, --svg <file>             produce plot as SVG file
                                         rather than display it
 
 {available_profiles}
+Use --list to show the names of the things that can be plotted.  The default is net.
 """
 
 try:
     # Imports {{{1
     from appdirs import user_config_dir, user_data_dir
     import nestedtext as nt
     from docopt import docopt
     from inform import (
-        columns, conjoin, display, done, error, fatal, os_error, terminate, Error
+        columns, conjoin, display, done, error, fatal, os_error, terminate,
+        title_case, Error
     )
     import arrow
     from pathlib import Path
     from quantiphy import Quantity
     import matplotlib
     import matplotlib.pyplot as plt
     import matplotlib.dates as mdates
     from matplotlib.ticker import FuncFormatter, NullFormatter
 
+    # stop matplotlib from issuing spurious warnings
+    import warnings
+    warnings.filterwarnings("ignore")
+
     __version__ = "0.8.1"
     __released__ = "2020-11-17"
 
     # Settings {{{1
     # These can be overridden in ~/.config/networth/config
     prog_name = 'networth'
     config_filename = 'config'
@@ -52,19 +58,20 @@
     # Read generic settings {{{1
     config_filepath = Path(settings_dir, config_filename)
     if config_filepath.exists():
         settings = config_filepath.read_text()
         settings = nt.loads(settings)
 
     # Read command line and process options {{{1
+    default_profile = settings.get('default profile', default_profile)
     available = set(p.stem for p in settings_dir.glob('*.prof'))
     if len(available) > 1:
-        choose_from = f'Choose from {conjoin(sorted(available))}.'
+        choose_from = f'Choose profile from {conjoin(sorted(available))}.'
         default = f'The default is {default_profile}.'
-        available_profiles = f'{choose_from} {default}\n'
+        available_profiles = f'{choose_from}  {default}'
     else:
         available_profiles = ''
 
     cmdline = docopt(__doc__.format(
         **locals()
     ))
     profile = cmdline['--profile'].rstrip('#') if cmdline['--profile'] else None
@@ -146,16 +153,21 @@
             last = waves[(name, 'ordinate')][-1]
             trace.set_label(f'{name}  {last.render(prec=2)}')
         except KeyError as e:
             error('unknown.', culprit=e.args[0][0])
     if trace:
         formatter = FuncFormatter(lambda v, p: Quantity(v, '$'))
         axis.yaxis.set_major_formatter(formatter)
-        axis.legend()
-        #axis.set_title('Worth')
+        figure.autofmt_xdate()
+        axis.legend(loc='lower left')
+        axis.set_title(f'{title_case(profile)}')
+        axis.grid(which='major', color='#DDDDDD', linewidth=0.8)
+        axis.grid(which='minor', color='#EEEEEE', linestyle=':', linewidth=0.5)
+        axis.minorticks_on()
+
         if svg_file:
             plt.savefig(svg_file)
         else:
             plt.show()
     else:
         error('nothing to plot.')
```

### Comparing `networth-1.1.0/setup.py` & `networth-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 from codecs import open
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name = 'networth',
-    version = '1.1.0',
+    version = '1.2',
     author = 'Ken Kundert',
     author_email = 'networth@nurdletech.com',
     description = 'Summarize net worth',
     long_description = readme,
     long_description_content_type = 'text/x-rst',
     url = 'https://github.com/kenkundert/networth',
     download_url = 'https://github.com/kenkundert/networth/tarball/master',
-    license = 'GPLv3+',
     scripts = 'networth plot-networth'.split(),
     install_requires = [
         'appdirs',
         'arrow',
         'avendesora>=1.12',
         'docopt',
         'inform>=1.14',
@@ -30,22 +29,21 @@
             # incompatible fork of 'python-gnupg'.  If both are installed, the 
             # user will probably have compatibility issues.
         'quantiphy',
         'quantiphy_eval>=0.3',
         'voluptuous',
     ],
     python_requires='>=3.6',
+    zip_safe = True,
+    license = 'GPLv3+',
     keywords = 'networth'.split(),
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3',
         'Topic :: Utilities',
     ],
 )
```

