# Comparing `tmp/py-portfolio-tools-0.0.3.tar.gz` & `tmp/py-portfolio-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-tools-0.0.3.tar", last modified: Sun Apr 23 17:05:07 2023, max compression
+gzip compressed data, was "py-portfolio-tools-0.0.5.tar", last modified: Sun Apr 23 17:25:49 2023, max compression
```

## Comparing `py-portfolio-tools-0.0.3.tar` & `py-portfolio-tools-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/
--rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0     1198 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.404878 py-portfolio-tools-0.0.3/py-portfolio-tools/
--rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/DataFetch.py
--rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Logger.py
--rw-rw-rw-   0        0        0     5878 2023-04-22 19:00:29.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Portfolio.py
--rw-rw-rw-   0        0        0     3214 2023-04-22 08:15:11.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioInputWindow.py
--rw-rw-rw-   0        0        0     6325 2023-04-22 08:18:46.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioManager.py
--rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Predictor.py
--rw-rw-rw-   0        0        0     2554 2023-04-22 08:12:50.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Tickers.py
--rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/Utils.py
--rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.3/py-portfolio-tools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:05:07.422440 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-23 17:05:07.000000 py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 17:05:07.423438 py-portfolio-tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-04-23 17:04:50.000000 py-portfolio-tools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:25:49.267827 py-portfolio-tools-0.0.5/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0     1198 2023-04-23 17:25:49.267827 py-portfolio-tools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 17:25:49.267827 py-portfolio-tools-0.0.5/py-portfolio-tools/
+-rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/DataFetch.py
+-rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/Logger.py
+-rw-rw-rw-   0        0        0     7954 2023-04-23 17:21:20.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/Portfolio.py
+-rw-rw-rw-   0        0        0     3232 2023-04-23 17:24:00.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/PortfolioInputWindow.py
+-rw-rw-rw-   0        0        0     6783 2023-04-23 17:19:46.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/PortfolioManager.py
+-rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/Predictor.py
+-rw-rw-rw-   0        0        0     2076 2023-04-23 17:24:05.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/Tickers.py
+-rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/Utils.py
+-rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.5/py-portfolio-tools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 17:25:49.267827 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-04-23 17:25:49.000000 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-04-23 17:25:49.000000 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 17:25:49.000000 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-04-23 17:25:49.000000 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-23 17:25:49.000000 py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 17:25:49.267827 py-portfolio-tools-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-04-23 17:25:39.000000 py-portfolio-tools-0.0.5/setup.py
```

### Comparing `py-portfolio-tools-0.0.3/LICENSE.md` & `py-portfolio-tools-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/PKG-INFO` & `py-portfolio-tools-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/DataFetch.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/DataFetch.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/Logger.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/Logger.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/Portfolio.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/Portfolio.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,20 +22,17 @@
             weights = [1.0 / len(stocks)] * len(stocks)
         self._weights = weights
         self._predictor = predictor
         self._dataFetch = dataFetch
         self._logger = logger
         self._analysis = None
         self._hasAnalysis = False
+        self._stockHistory = None
     
-    def NuemericalAnalysis(self):
-        
-
-    def Analyse(self, startDate, endDate):
-        """Analyse the portfolio from the start date to the end date"""
+    def FetchStockHistory(self, startDate, endDate, silent):
         # is endDate is None, then set it to today
         if endDate == None:
             endDate = str(datetime.now().strftime("%Y-%m-%d"))
         # check if end date after today
         requirePrediction = False
         finalEndDate = endDate
         if datetime.strptime(endDate, "%Y-%m-%d") > datetime.now():
@@ -51,20 +48,69 @@
         
         if requirePrediction:
             self._logger.Log(f'Predicting stock history from {finalEndDate} to {endDate}')
             if self._predictor == None:
                 raise RuntimeError("Predictor is not set")
             self._stockHistory = self._predictor.Predict(self._stockHistory, finalEndDate, endDate)
         
+
+    
+    def NumericalAnalysis(self, startDate, endDate, silent = False):
+        """Do a numerical analysis of the portfolio"""
+
+        if not silent:
+            self._logger.Log(f"Starging numerical analysis of portfolio {self._name}")
+            self._logger.Log(f"Stocks: {self._stocks}")
+            self._logger.Log(f"Weights: {self._weights}")
+        
+        if self._analysis == None:
+            self.FetchStockHistory(startDate, endDate, silent)
+            self._analysis = Object()
+            self._analysis.startDate = startDate
+            self._analysis.endDate = endDate
+            self._analysis.stockHistory = self._stockHistory.copy()
+
+        # calculate the daily returns
+        self._analysis.dailyReturns = self._stockHistory.pct_change()
+
+        # calculate the mean daily returns
+        self._analysis.meanDailyReturns = self._analysis.dailyReturns.mean()
+
+        # calculate the covariance matrix
+        self._analysis.covarianceMatrix = self._analysis.dailyReturns.cov()
+
+        # calculate the portfolio variance
+        self._analysis.portfolioVariance = np.dot(self._weights, np.dot(self._analysis.covarianceMatrix, self._weights)) * 252
+
+        # calculate the portfolio standard deviation
+        self._analysis.portfolioStandardDeviation = np.sqrt(self._analysis.portfolioVariance)
+        self._analysis.portfolioRisk = self._analysis.portfolioStandardDeviation
+
+        # calculate the portfolio expected return
+        self._analysis.portfolioExpectedReturn = np.dot(self._weights, self._analysis.meanDailyReturns) * 252
+
+        # calculate the portfolio sharpe ratio
+        self._analysis.portfolioSharpeRatio = self._analysis.portfolioExpectedReturn / self._analysis.portfolioStandardDeviation
+
+        
+        
+
+    def Analyse(self, startDate, endDate):
+        """Analyse the portfolio from the start date to the end date"""
         self._logger.Log(f'Calculating portfolio history from {startDate} to {endDate}')
         
-        self._analysis = Object()
-        self._analysis.startDate = startDate
-        self._analysis.endDate = endDate
-        self._analysis.stockHistory = self._stockHistory.copy()
+        if self._stockHistory == None:
+            self.FetchStockHistory(startDate, endDate, False)
+
+        if self._analysis == None:
+            self._analysis = Object()
+            self._analysis.startDate = startDate
+            self._analysis.endDate = endDate
+            self._analysis.stockHistory = self._stockHistory.copy()
+
         self._analysis.stockHistoryPlots = []
         
         # plot the stock history of individual stocks in individual graphs
         self._logger.Log(f'Plotting stock history of individual stocks')
         for stock in self._stocks:
             plt.plot(self._stockHistory[stock])
             plt.title(stock)
@@ -118,10 +164,10 @@
         plt.title("Sector Based Distribution")
         buffer = io.BytesIO()
         plt.savefig(buffer, format = "png")
         self._analysis.sectorBasedDistributionPlot = buffer
         plt.clf()
 
         
-
+        self.NumericalAnalysis(startDate, endDate, True)
 
         self._hasAnalysis = True
```

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioInputWindow.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/PortfolioInputWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         if imgui.button("Clear All"):
             self._portfolioStocks.clear()
         
         if imgui.button("Add Portfolio") and len(self._portfolioStocks) > 0:
             totalStocksInPortfolio = sum([stock.quantity for stock in self._portfolioStocks])
             weights = [stock.quantity / totalStocksInPortfolio for stock in self._portfolioStocks]
-            stocks = [STOCK_TICKERS[stock.tickerId] for stock in self._portfolioStocks]
+            stocks = [list(STOCK_TICKER_NAMES.keys())[stock.tickerId] for stock in self._portfolioStocks]
             portfolio = Portfolio(self._portfolioName, stocks, weights, None)
             self._portfolios.append(PortfolioManager(portfolio))
             self._portfolioStocks.clear()
             self._portfolioName = f"Portfolio {len(self._portfolios)}"
         
         imgui.same_line()
```

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/PortfolioManager.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/PortfolioManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,21 @@
                 SaveImageAsFile(self._countryBasedDistributionPlotTexture, ShowFileSaveWindow() + ".png")
             
             imgui.text("Sector Based Distribution")
             imgui.image(self._sectorBasedDistributionPlotTexture.id, self._sectorBasedDistributionPlotTexture.width, self._sectorBasedDistributionPlotTexture.height)
             if imgui.button("Save Sector Based Distribution as File"):
                 SaveImageAsFile(self._sectorBasedDistributionPlotTexture, ShowFileSaveWindow() + ".png")
 
+        expanded, visible = imgui.collapsing_header("Numerical Analysis")
+        if expanded:
+            imgui.text("Variance: " + str(self._portfolio._analysis.portfolioVariance))
+            imgui.text("Risk: " + str(self._portfolio._analysis.portfolioRisk))
+            imgui.text("Return: " + str(self._portfolio._analysis.portfolioExpectedReturn))
+            imgui.text("Sharpe Ratio: " + str(self._portfolio._analysis.portfolioSharpeRatio))
+
     def UnloadAnalysis(self):
         for texture in self._stockHistoryTextures:
             DeleteGLTexture(texture.id)
 
         if self._stockHistoryComparisonTexture != None:
             DeleteGLTexture(self._stockHistoryComparisonTexture.id)
```

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/Tickers.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/Tickers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-STOCK_TICKERS = ['IBM', 'GE', 'CSCO', 'INTC', 'ORCL', 'ACN', 'GS', 'JPM', 'WFC', 'AXP', 'BRK.A', 'BUD', 'DEO', 'ULVR.L', 'HSBA.L', 'BP.L', 'VOD.L', 'LLOY.L', 'RY.TO', 'TD.TO', 'BNS.TO', 'ENB.TO', 'SHOP.TO', 'BMO.TO', 'RYAAY', 'RYA.L', 'LGEN.L', 'SGE.L', 'BMW.DE', 'DAI.DE', 'DPW.DE', 'ADS.DE', 'BNP.PA', 'SAN.PA', 'AIR.PA', 'OR.PA', 'GLE.PA', 'ASML', 'INGA.AS', 'RDSA.AS', 'UNA.AS', 'HEIA.AS', 'RDSB.L', 'GSK.L', 'AZN.L', 'ULVR.L', 'BATS.L', 'NOVN.SW', 'NESN.SW', 'UBSG.SW']
-
 STOCK_TICKER_NAMES = {
     'AAPL': 'Apple Inc.',
     'MSFT': 'Microsoft Corporation',
     'AMZN': 'Amazon.com, Inc.',
     'GOOG': 'Alphabet Inc. (Class C)',
     'TSLA': 'Tesla, Inc.',
     'BABA': 'Alibaba Group Holding Limited (ADR)',
```

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/Utils.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/Utils.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/py-portfolio-tools/__main__.py` & `py-portfolio-tools-0.0.5/py-portfolio-tools/__main__.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/PKG-INFO` & `py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.3/py_portfolio_tools.egg-info/SOURCES.txt` & `py-portfolio-tools-0.0.5/py_portfolio_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.3/setup.py` & `py-portfolio-tools-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import re
 
 requirements = ['numpy', 'pandas', 'matplotlib', 'yfinance', "PyOpenGL", "glfw", "imgui[glfw]", "Pillow"] 
 
-version = '0.0.3'
+version = '0.0.5'
 
 if not version:
     raise RuntimeError('version is not set')
 
 readme = 'Coming Soon ...'
 
 setup(
```

