# Comparing `tmp/amino.light.py-0.1.2.tar.gz` & `tmp/amino.light.py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.2.tar", last modified: Wed Apr 10 17:27:41 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.3.tar", last modified: Wed Apr 10 20:50:28 2024, max compression
```

## Comparing `amino.light.py-0.1.2.tar` & `amino.light.py-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.233783 amino.light.py-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.155768 amino.light.py-0.1.2/AminoLightPy/
--rw-rw-rw-   0        0        0      296 2024-04-08 13:05:43.000000 amino.light.py-0.1.2/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.2/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    72454 2024-04-10 13:49:30.000000 amino.light.py-0.1.2/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.2/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.157766 amino.light.py-0.1.2/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.2/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.169774 amino.light.py-0.1.2/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    94934 2024-04-10 12:04:03.000000 amino.light.py-0.1.2/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    17113 2024-04-10 13:21:35.000000 amino.light.py-0.1.2/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    75163 2024-04-10 13:49:22.000000 amino.light.py-0.1.2/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4060 2024-04-10 17:27:41.230785 amino.light.py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-04-10 17:23:45.000000 amino.light.py-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 17:27:41.225765 amino.light.py-0.1.2/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     4060 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 17:27:39.000000 amino.light.py-0.1.2/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 17:27:41.245770 amino.light.py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-04-10 17:27:16.000000 amino.light.py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.835242 amino.light.py-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.712244 amino.light.py-0.1.3/AminoLightPy/
+-rw-rw-rw-   0        0        0      296 2024-04-10 20:45:21.000000 amino.light.py-0.1.3/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.3/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    72454 2024-04-10 13:49:30.000000 amino.light.py-0.1.3/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.3/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.714244 amino.light.py-0.1.3/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.3/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.745244 amino.light.py-0.1.3/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    95642 2024-04-10 20:48:55.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    17113 2024-04-10 13:21:35.000000 amino.light.py-0.1.3/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    75163 2024-04-10 13:49:22.000000 amino.light.py-0.1.3/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3567 2024-04-10 20:50:28.834245 amino.light.py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2024-04-10 20:49:56.000000 amino.light.py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.832241 amino.light.py-0.1.3/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     3567 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-10 20:50:27.000000 amino.light.py-0.1.3/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 20:50:28.849240 amino.light.py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-10 20:46:02.000000 amino.light.py-0.1.3/setup.py
```

### Comparing `amino.light.py-0.1.2/AminoLightPy/acm.py` & `amino.light.py-0.1.3/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/client.py` & `amino.light.py-0.1.3/AminoLightPy/client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/constants.py` & `amino.light.py-0.1.3/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.3/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.3/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.3/AminoLightPy/lib/util/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.applicant: Optional[str] = data.get("applicant")
         self.avgDailySpendTimeIn7Days: Optional[int] = data.get("avgDailySpendTimeIn7Days")
         self.adminLogCountIn7Days: Optional[int] = data.get("adminLogCountIn7Days")
 
         # extensions
         self.extensions: Optional[Dict] = data.get("extensions") or {}
         # style
-        self.style: Optional[Dict] = self.extensions.get("style", {})
+        self.style: Optional[Dict] = self.extensions.get("style") or {}
         self.backgroundImage: Optional[str] = self.style.get("backgroundImage")
         self.backgroundColor: Optional[str] = self.style.get("backgroundColor")
 
         self.coverAnimation: Optional[str] = self.extensions.get("coverAnimation")
         self.customTitles: Optional[List[str]] = self.extensions.get("customTitles")
         self.defaultBubbleId: Optional[str] = self.extensions.get("defaultBubbleId")
         self.disabledLevel: Optional[int] = self.extensions.get("__disabledLevel__")
@@ -106,15 +106,15 @@
         self.influencerInfo: Optional[Dict] = data.get("influencerInfo") or {}
         self.fansCount: Optional[int] = self.influencerInfo.get("fansCount")
         self.influencerCreatedTime: Optional[int] = self.influencerInfo.get("createdTime")
         self.influencerMonthlyFee: Optional[int] = data.get("monthlyFee")
         self.influencerPinned: Optional[bool] = data.get("pinned")
 
         # adminInfo
-        self.staffInfo: Optional[Dict] = data.get("adminInfo", {})
+        self.staffInfo: Optional[Dict] = data.get("adminInfo") or {}
         self.globalStrikeCount: Optional[int] = self.staffInfo.get("globalStrikeCount")
         self.lastStrikeTime: Optional[int] = self.staffInfo.get("lastStrikeTime")
         self.lastWarningTime: Optional[int] = self.staffInfo.get("lastWarningTime")
         self.strikeCount: Optional[int] = self.staffInfo.get("strikeCount")
         self.warningCount: Optional[int] = self.staffInfo.get("warningCount")
 
         self.session = None
@@ -143,15 +143,15 @@
 
         self.json = data
         self.nextPageToken = nextPageToken
         self.prevPageToken = prevPageToken
 
         for y in data:
             _author.append(y.get("author"))
-            _quizQuestionList.append(QuizQuestionList(y.get("quizQuestionList")).QuizQuestionList)
+            _quizQuestionList.append(QuizQuestionList(y.get("quizQuestionList", [])).QuizQuestionList)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.quizQuestionList = _quizQuestionList
 
         self.createdTime = []
         self.globalVotesCount = []
         self.globalVotedValue = []
@@ -172,15 +172,14 @@
         self.globalCommentsCount = []
         self.modifiedTime = []
         self.widgetDisplayInterval = []
         self.totalPollVoteCount = []
         self.blogId = []
         self.viewCount = []
         self.fansOnly = []
-        self.backgroundColor = []
         self.votesCount = []
         self.endTime = []
         self.refObjectId = []
         self.refObject = []
         self.votedValue = []
         self.extensions = []
         self.commentsCount = []
@@ -193,14 +192,17 @@
         self.quizTrendingTimes = []
         self.quizLastAddQuestionTime = []
         self.isIntroPost = []
 
     @property
     def BlogList(self):
         for x in self.json:
+            tipInfo = x.get("tipInfo") or {}
+            extensions = x.get("extensions") or {}
+
             self.globalVotesCount.append(x.get("globalVotesCount"))
             self.globalVotedValue.append(x.get("globalVotedValue"))
             self.keywords.append(x.get("keywords"))
             self.mediaList.append(x.get("mediaList"))
             self.style.append(x.get("style"))
             self.totalQuizPlayCount.append(x.get("totalQuizPlayCount"))
             self.title.append(x.get("title"))
@@ -222,43 +224,53 @@
             self.votedValue.append(x.get("votedValue"))
             self.content.append(x.get("content"))
             self.createdTime.append(x.get("createdTime"))
             self.shareUrl.append(x.get("shareURLFullPath"))
             self.commentsCount.append(x.get("commentsCount"))
 
             # tip info
-            self.tipInfo.append(x.get("tipInfo"))
-            self.tippersCount.append(self.tipInfo.get("tippersCount"))
-            self.tippable.append(self.tipInfo.get("tippable"))
-            self.tippedCoins.append(self.tipInfo.get("tippedCoins"))
+            self.tipInfo.append(tipInfo)
+            self.tippersCount.append(tipInfo.get("tippersCount"))
+            self.tippable.append(tipInfo.get("tippable"))
+            self.tippedCoins.append(tipInfo.get("tippedCoins"))
 
             # extensions
-            self.extensions.append(x.get("extensions"))
-            self.fansOnly.append(self.extensions.get("fansOnly"))
-            self.backgroundColor.append(self.extensions.get("style", {"backgroundColor": None})["backgroundColor"])
-            self.featuredType.append(self.extensions.get("featuredType"))
-            self.disabledTime.append(self.extensions.get("__disabledTime__"))
-            self.quizPlayedTimes.append(self.extensions.get("quizPlayedTimes"))
-            self.quizTotalQuestionCount.append(self.extensions.get("quizTotalQuestionCount"))
-            self.quizTrendingTimes.append(self.extensions.get("quizTrendingTimes"))
-            self.quizLastAddQuestionTime.append(self.extensions.get("quizLastAddQuestionTime"))
-            self.isIntroPost.append(self.extensions.get("isIntroPost"))
+            self.extensions.append(extensions)
+            self.fansOnly.append(extensions.get("fansOnly"))
+            self.featuredType.append(extensions.get("featuredType"))
+            self.disabledTime.append(extensions.get("__disabledTime__"))
+            self.quizPlayedTimes.append(extensions.get("quizPlayedTimes"))
+            self.quizTotalQuestionCount.append(extensions.get("quizTotalQuestionCount"))
+            self.quizTrendingTimes.append(extensions.get("quizTrendingTimes"))
+            self.quizLastAddQuestionTime.append(extensions.get("quizLastAddQuestionTime"))
+            self.isIntroPost.append(extensions.get("isIntroPost"))
 
         return self
 
 class RecentBlogs:
+    __slots__ = (
+        'json', 
+        'nextPageToken', 
+        'prevPageToken'
+    )
+
     def __init__(self, data):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+
+            return
         self.json = data
 
         self.nextPageToken = None
         self.prevPageToken = None
 
     @property
     def RecentBlogs(self):
-        paging = self.json.get("paging", {})
+        paging = self.json.get("paging") or {}
         self.nextPageToken = paging.get("nextPageToken")
         self.prevPageToken = paging.get("prevPageToken")
 
         return BlogList(self.json.get("blogList"), self.nextPageToken, self.prevPageToken).BlogList
 
 class BlogCategoryList:
     def __init__(self, data):
@@ -295,17 +307,17 @@
 class Blog:
     def __init__(self, data):
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
         self.quizQuestionList: QuizQuestionList = QuizQuestionList(data.get("quizQuestionList", [])).QuizQuestionList
 
-        extensions = self.json.get("extensions", {})
-        tipInfo = self.json.get("tipInfo", {})
-        style = extensions.get("style", {})
+        extensions = self.json.get("extensions") or {}
+        tipInfo = self.json.get("tipInfo") or {}
+        style = extensions.get("style") or {}
 
         self.globalVotesCount = self.json.get("globalVotesCount")
         self.globalVotedValue = self.json.get("globalVotedValue")
         self.keywords = self.json.get("keywords")
         self.mediaList: Optional[MediaObject] = self.json.get("mediaList")
         self.style = self.json.get("style")
         self.totalQuizPlayCount = self.json.get("totalQuizPlayCount")
@@ -354,17 +366,17 @@
     def __init__(self, data):
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
         try: self.labels: WikiLabelList = WikiLabelList(data["extensions"]["props"]).WikiLabelList
         except (KeyError, TypeError): self.labels: WikiLabelList = WikiLabelList([])
 
-        extensions = self.json.get("extensions", {})
-        style = extensions.get("style", {})
-        knowledgeBase = extensions.get("knowledgeBase", {})
+        extensions = self.json.get("extensions") or {}
+        style = extensions.get("style") or {}
+        knowledgeBase = extensions.get("knowledgeBase") or {}
 
         self.wikiId = self.json.get("itemId")
         self.status = self.json.get("status")
         self.style = self.json.get("style")
         self.globalCommentsCount = self.json.get("globalCommentsCount")
         self.modifiedTime = self.json.get("modifiedTime")
         self.votedValue = self.json.get("votedValue")
@@ -463,22 +475,22 @@
         self.json = data
 
         self.agent: UserProfile = UserProfile(data.get("agent", [])).UserProfile
 
         try: self.rankingTable: RankingTableList = RankingTableList(data["advancedSettings"]["rankingTable"]).RankingTableList
         except (KeyError, TypeError): self.rankingTable: RankingTableList = RankingTableList([])
 
-        themePack: Dict = data.get("themePack", {})
-        configuration: Dict = data.get("configuration", {})
-        appearance: Dict = configuration.get("appearance", {})
-        leftSidePanel: Dict = appearance.get("leftSidePanel", {})
-        style: Dict = leftSidePanel.get("style", {})
-        page: Dict = configuration.get("page", {})
-        advancedSettings: Dict = data.get("advancedSettings", {})
-        extensions: Dict = data.get("extensions", {})
+        themePack: Dict = data.get("themePack") or {}
+        configuration: Dict = data.get("configuration") or {}
+        appearance: Dict = configuration.get("appearance") or {}
+        leftSidePanel: Dict = appearance.get("leftSidePanel") or {}
+        style: Dict = leftSidePanel.get("style") or {}
+        page: Dict = configuration.get("page") or {}
+        advancedSettings: Dict = data.get("advancedSettings") or {}
+        extensions: Dict = data.get("extensions") or {}
 
         self.name: Optional[str] = data.get("name")
         self.usersCount: Optional[int] = data.get("membersCount")
         self.createdTime: Optional[str] = data.get("createdTime")
         self.aminoId = data.get("endpoint")
         self.icon = data.get("icon")
         self.link = data.get("link")
@@ -492,17 +504,17 @@
         self.probationStatus = self.json.get("probationStatus")
         self.listedStatus = self.json.get("listedStatus")
         self.themePack = themePack
         self.themeColor = themePack.get("themeColor")
         self.themeHash = themePack.get("themePackHash")
         self.themeVersion = themePack.get("themePackRevision")
         self.themeUrl = themePack.get("themePackUrl")
-        self.themeHomePageAppearance = appearance.get("homePage", {}).get("navigation")
-        self.themeLeftSidePanelTop = leftSidePanel.get("navigation", {}).get("level1")
-        self.themeLeftSidePanelBottom = leftSidePanel.get("navigation", {}).get("level2")
+        self.themeHomePageAppearance = appearance.get("homePage") or {}.get("navigation")
+        self.themeLeftSidePanelTop = leftSidePanel.get("navigation") or {}.get("level1")
+        self.themeLeftSidePanelBottom = leftSidePanel.get("navigation") or {}.get("level2")
         self.themeLeftSidePanelColor = style.get("iconColor")
         self.customList = page.get("customList")
         self.tagline = self.json.get("tagline")
         self.searchable = self.json.get("searchable")
         self.isStandaloneAppDeprecated = self.json.get("isStandaloneAppDeprecated")
         self.influencerList = self.json.get("influencerList")
         self.keywords = data.get("keywords")
@@ -570,15 +582,15 @@
         return self
 
 
 class Membership:
     def __init__(self, data):
         self.json = data
 
-        membership = data.get("membership", {})
+        membership = data.get("membership") or {}
 
         self.premiumFeature = data.get("premiumFeatureEnabled")
         self.hasAnyAndroidSubscription = data.get("hasAnyAndroidSubscription")
         self.hasAnyAppleSubscription = data.get("hasAnyAppleSubscription")
         self.accountMembership = data.get("accountMembershipEnabled")
         self.paymentType = data.get("paymentType")
         self.membershipStatus = membership.get("membershipStatus")
@@ -592,28 +604,28 @@
     def Membership(self):
         return self
 
 class FromCode:
     def __init__(self, data):
         self.json = data
 
-        extensions = data.get("extensions", {})
-        linkInfo = extensions.get("linkInfo", {})
+        extensions = data.get("extensions") or {}
+        linkInfo = extensions.get("linkInfo") or {}
 
         self.community: Community = Community(extensions.get("community")).Community
         self.path = data.get("path")
         self.objectType = linkInfo.get("objectType")
         self.shortCode = linkInfo.get("shortCode")
         self.fullPath = linkInfo.get("fullPath")
         self.targetCode = linkInfo.get("targetCode")
         self.objectId = linkInfo.get("objectId")
         self.shortUrl = linkInfo.get("shareURLShortCode")
         self.fullUrl = linkInfo.get("shareURLFullPath")
         self.comIdPost = linkInfo.get("ndcId")
-        self.comId = self.comIdPost or extensions.get("community", {}).get("ndcId")
+        self.comId = self.comIdPost or extensions.get("community") or {}.get("ndcId")
 
     @property
     def FromCode(self):
         return self
 
 class UserProfileCountList:
     __slots__ = (
@@ -803,16 +815,16 @@
         self.json = data
 
         try: self.author = UserProfile(data["itemCategory"]["author"]).UserProfile
         except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
         try: self.subCategory = WikiCategoryList(data["childrenWrapper"]["itemCategoryList"]).WikiCategoryList
         except (KeyError, TypeError): self.subCategory: WikiCategoryList = WikiCategoryList([])
 
-        itemCategory = data.get("itemCategory", {})
-        childrenWrapper = data.get("childrenWrapper", {})
+        itemCategory = data.get("itemCategory") or {}
+        childrenWrapper = data.get("childrenWrapper") or {}
 
         self.itemsCount = itemCategory.get("itemsCount")
         self.parentCategoryId = itemCategory.get("parentCategoryId")
         self.categoryId = itemCategory.get("categoryId")
         self.extensions = itemCategory.get("extensions")
         self.createdTime = itemCategory.get("createdTime")
         self.title = itemCategory.get("label")
@@ -896,15 +908,15 @@
         self.condition = data.get("condition")
         self.icon = data.get("icon")
         self.latestActivityTime = data.get("latestActivityTime")
         self.comId = data.get("ndcId")
         self.createdTime = data.get("createdTime")
 
         # extensions
-        self.extensions = data.get("extensions", {})
+        self.extensions = data.get("extensions") or {}
         self.viewOnly = self.extensions.get("viewOnly")
         self.coHosts = self.extensions.get("coHost")
         self.membersCanInvite = self.extensions.get("membersCanInvite")
         self.language = self.extensions.get("language")
         self.announcement = self.extensions.get("announcement")
         self.backgroundImage = self.extensions.get("bm", [None, None])[1]
         self.lastMembersSummaryUpdateTime = self.extensions.get("lastMembersSummaryUpdateTime")
@@ -916,19 +928,19 @@
         self.pinAnnouncement = self.extensions.get("pinAnnouncement")
         self.vvChatJoinType = self.extensions.get("vvChatJoinType")
         self.disabledTime = self.extensions.get("__disabledTime__")
         self.tippingPermStatus = self.extensions.get("tippingPermStatus")
         self.screeningRoomHostId = self.extensions.get("screeningRoomHostUid")
 
         # screeningRoomPermission
-        screeningRoomPermission = self.extensions.get("screeningRoomPermission", {})
+        screeningRoomPermission = self.extensions.get("screeningRoomPermission") or {}
         self.screeningRoomPermission = screeningRoomPermission.get("action")
 
         # organizerTransferRequest
-        organizerTransferRequest = self.extensions.get("organizerTransferRequest", {})
+        organizerTransferRequest = self.extensions.get("organizerTransferRequest") or {}
         self.organizerTransferCreatedTime = organizerTransferRequest.get("createdTime")
         self.organizerTransferId = organizerTransferRequest.get("requestId")
 
     @property
     def Thread(self):
         return self
 
@@ -1115,15 +1127,15 @@
         #extensions
         self.extensions = data.get("extensions") or {}
         self.iconSourceStickerId = self.extensions.get("iconSourceStickerId")
         self.originalAuthor: UserProfile = UserProfile(self.extensions.get("originalAuthor")).UserProfile
         self.originalCommunity: Community = Community(self.extensions.get("originalCommunity")).Community
 
         #restrictionInfo
-        self.restrictionInfo = data.get("restrictionInfo", {})
+        self.restrictionInfo = data.get("restrictionInfo") or {}
         self.discountStatus = self.restrictionInfo.get("discountStatus")
         self.discountValue = self.restrictionInfo.get("discountValue")
         self.ownerId = self.restrictionInfo.get("ownerUid")
         self.ownerType = self.restrictionInfo.get("ownerType")
         self.restrictType = self.restrictionInfo.get("restrictType")
         self.restrictValue = self.restrictionInfo.get("restrictValue")
         self.availableDuration = self.restrictionInfo.get("availableDuration")
@@ -1212,16 +1224,16 @@
 
 class Message:
     def __init__(self, data):
         self.json = data
 
         self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
 
-        extensions = data.get("extensions", {})
-        videoExtensions = extensions.get("videoExtensions", {})
+        extensions = data.get("extensions") or {}
+        videoExtensions = extensions.get("videoExtensions") or {}
 
         self.sticker: Sticker = Sticker(extensions.get("sticker")).Sticker
 
         self.content = data.get("content")
         self.includedInSummary = data.get("includedInSummary")
         self.isHidden = data.get("isHidden")
         self.messageId = data.get("messageId")
@@ -1307,33 +1319,33 @@
             self.mediaType.append(x.get("mediaType"))
 
             # extensions
             self.extensions.append(x.get("extensions"))
             self.originalStickerId.append(self.extensions[n].get("originalStickerId"))
             self.mentionUserIds.append([m.get("uid") for m in self.extensions[n].get("mentionedArray", [])])
             self.videoExtensions.append(self.extensions[n].get("videoExtensions"))
-            self.videoDuration.append(self.extensions[n].get("videoExtensions", {}).get("duration"))
-            self.videoHeight.append(self.extensions[n].get("videoExtensions", {}).get("height"))
-            self.videoWidth.append(self.extensions[n].get("videoExtensions", {}).get("width"))
-            self.videoCoverImage.append(self.extensions[n].get("videoExtensions", {}).get("coverImage"))
+            self.videoDuration.append(self.extensions[n].get("videoExtensions") or {}.get("duration"))
+            self.videoHeight.append(self.extensions[n].get("videoExtensions") or {}.get("height"))
+            self.videoWidth.append(self.extensions[n].get("videoExtensions") or {}.get("width"))
+            self.videoCoverImage.append(self.extensions[n].get("videoExtensions") or {}.get("coverImage"))
             self.tippingCoins.append(self.extensions[n].get("tippingCoins"))
 
         return self
 
 class GetMessages:
     def __init__(self, data):
         self.json = data
 
         self.messageList = []
         self.nextPageToken = None
         self.prevPageToken = None
 
     @property
     def GetMessages(self):
-        paging = self.json.get("paging", {})
+        paging = self.json.get("paging") or {}
 
         self.nextPageToken = paging.get("nextPageToken")
         self.prevPageToken = paging.get("prevPageToken")
         self.messageList = self.json.get("messageList")
 
         return MessageList(self.messageList, self.nextPageToken, self.prevPageToken).MessageList
 
@@ -1414,15 +1426,15 @@
         self.objectUrl = []
         self.content = []
         self.value = []
 
     @property
     def AdminLogList(self):
         for x in self.json:
-            extData = x.get("extData", {})
+            extData = x.get("extData") or {}
 
             self.createdTime.append(x.get("createdTime"))
             self.objectType.append(x.get("objectType"))
             self.operationName.append(x.get("operationName"))
             self.comId.append(x.get("ndcId"))
             self.referTicketId.append(x.get("referTicketId"))
             self.extData.append(extData)
@@ -1473,15 +1485,18 @@
 class FanClubList:
     __slots__ = (
         "json", "profile", "targetUserProfile", "userId", "lastThankedTime",
         "expiredTime", "createdTime", "status", "targetUserId"
     )
 
     def __init__(self, data):
-        if not data:
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+
             return
 
         self.json = data
 
         profile_data = []
         targetUserProfile_data = []
         userId_data = []
@@ -1525,15 +1540,27 @@
         self.myFanClub = data.get("myFanClub")
 
     @property
     def InfluencerFans(self):
         return self
 
 class QuizQuestionList:
+    __slots__ = (
+        'json', 'status', 'parentType', 'title', 'createdTime',
+        'questionId', 'parentId', 'mediaList', 'extensions', 'style',
+        'backgroundImage', 'backgroundColor', 'answerExplanation',
+        'answersList'
+    )
     def __init__(self, data):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+
+            return
+
         _answersList = []
 
         self.json = data
 
         for y in data:
             try: _answersList.append(QuizAnswers(y["extensions"]["quizQuestionOptList"]).QuizAnswers)
             except (KeyError, TypeError): _answersList.append(None)
@@ -1551,16 +1578,16 @@
         self.backgroundColor = []
         self.answerExplanation = []
         self.answersList = _answersList
 
     @property
     def QuizQuestionList(self):
         for x in self.json:
-            extensions = x.get("extensions", {})
-            style = extensions.get("style", {})
+            extensions = x.get("extensions") or {}
+            style = extensions.get("style") or {}
             backgroundMediaList: Optional[MediaObject] = style.get("backgroundMediaList", [None, None])
 
             self.status.append(x.get("status"))
             self.parentType.append(x.get("parentType"))
             self.title.append(x.get("title"))
             self.createdTime.append(x.get("createdTime"))
             self.questionId.append(x.get("quizQuestionId"))
@@ -1751,15 +1778,15 @@
         "json", "comId", "alertOption", "membershipStatus",
         "actions", "target", "params", "threadType", "duration",
         "id", "message"
     )
 
     def __init__(self, data):
         self.json = data
-        params = self.json.get("params", {})
+        params = self.json.get("params") or {}
 
         self.comId = self.json.get("ndcId")
         self.alertOption = self.json.get("alertOption")
         self.membershipStatus = self.json.get("membershipStatus")
         self.actions = self.json.get("actions")
         self.target = self.json.get("target")
         self.params = params
@@ -1927,17 +1954,17 @@
         self.showAuthor = []
         self.allowQuickOperation = []
         self.operationList = []
 
     @property
     def NoticeList(self):
         for x in self.json:
-            extensions = x.get("extensions", {})
-            config = extensions.get("config", {})
-            style = extensions.get("style", {})
+            extensions = x.get("extensions") or {}
+            config = extensions.get("config") or {}
+            style = extensions.get("style") or {}
 
             self.title.append(x.get("title"))
             self.icon.append(x.get("icon"))
             self.noticeId.append(x.get("noticeId"))
             self.status.append(x.get("status"))
             self.comId.append(x.get("ndcId"))
             self.modifiedTime.append(x.get("modifiedTime"))
@@ -2025,18 +2052,18 @@
         self.isNew = []
         self.availableComIds = []
         self.status = []
 
     @property
     def AvatarFrameList(self):
         for x in self.json:
-            config = x.get("config", {})
-            restrictionInfo = x.get("restrictionInfo", {})
-            ownershipInfo = x.get("ownershipInfo", {})
-            additionalBenefits = x.get("additionalBenefits", {})
+            config = x.get("config") or {}
+            restrictionInfo = x.get("restrictionInfo") or {}
+            ownershipInfo = x.get("ownershipInfo") or {}
+            additionalBenefits = x.get("additionalBenefits") or {}
 
             self.isGloballyAvailable.append(x.get("isGloballyAvailable"))
             self.extensions.append(x.get("extensions"))
             self.frameType.append(x.get("frameType"))
             self.resourceUrl.append(x.get("resourceUrl"))
             self.md5.append(x.get("md5"))
             self.icon.append(x.get("icon"))
@@ -2106,15 +2133,15 @@
         self.isNew = data.get("isNew")
         self.bubbleId = data.get("bubbleId")
         self.resourceUrl = data.get("resourceUrl")
         self.backgroundImage = data.get("backgroundImage")
         self.status = data.get("status")
         self.modifiedTime = data.get("modifiedTime")
 
-        ownershipInfo = data.get("ownershipInfo", {})
+        ownershipInfo = data.get("ownershipInfo") or {}
         self.ownershipInfo = ownershipInfo
         self.expiredTime = ownershipInfo.get("expiredTime")
         self.isAutoRenew = ownershipInfo.get("isAutoRenew")
 
         self.ownershipStatus = data.get("ownershipStatus")
         self.bannerImage = data.get("bannerImage")
         self.md5 = data.get("md5")
@@ -2126,15 +2153,15 @@
         self.createdTime = data.get("createdTime")
         self.deletable = data.get("deletable")
         self.backgroundMedia = data.get("backgroundMedia")
         self.description = data.get("description")
         self.materialUrl = data.get("materialUrl")
         self.comId = data.get("ndcId")
 
-        restrictionInfo = data.get("restrictionInfo", {})
+        restrictionInfo = data.get("restrictionInfo") or {}
         self.restrictionInfo = restrictionInfo
         self.discountStatus = restrictionInfo.get("discountStatus")
         self.discountValue = restrictionInfo.get("discountValue")
         self.ownerId = restrictionInfo.get("ownerUid")
         self.ownerType = restrictionInfo.get("ownerType")
         self.restrictType = restrictionInfo.get("restrictType")
         self.restrictValue = restrictionInfo.get("restrictValue")
@@ -2223,16 +2250,16 @@
         self.restrictType = []
         self.restrictValue = []
         self.availableDuration = []
 
     @property
     def BubbleList(self):
         for x in self.json:
-            ownershipInfo = x.get("ownershipInfo", {})
-            restrictionInfo = x.get("restrictionInfo", {})
+            ownershipInfo = x.get("ownershipInfo") or {}
+            restrictionInfo = x.get("restrictionInfo") or {}
 
             self.uid.append(x.get("uid"))
             self.isActivated.append(x.get("isActivated"))
             self.isNew.append(x.get("isNew"))
             self.bubbleId.append(x.get("bubbleId"))
             self.resourceUrl.append(x.get("resourceUrl"))
             self.backgroundImage.append(x.get("backgroundImage"))
@@ -2277,17 +2304,17 @@
         self.icon = []
         self.frameUrl = []
         self.value = []
 
     @property
     def AvatarFrame(self):
         for x in self.json:
-            refObject = x.get("refObject", {})
-            config = refObject.get("config", {})
-            restrictionInfo = refObject.get("restrictionInfo", {})
+            refObject = x.get("refObject") or {}
+            config = refObject.get("config") or {}
+            restrictionInfo = refObject.get("restrictionInfo") or {}
 
             self.name.append(config.get("name"))
             self.id.append(config.get("id"))
             self.resourceUrl.append(refObject.get("resourceUrl"))
             self.icon.append(refObject.get("icon"))
             self.frameUrl.append(refObject.get("frameUrl"))
             self.value.append(restrictionInfo.get("restrictValue"))
@@ -2305,17 +2332,17 @@
         self.backgroundImage = []
         self.resourceUrl = []
         self.value = []
 
     @property
     def ChatBubble(self):
         for x in self.json:
-            itemBasicInfo = x.get("itemBasicInfo", {})
-            refObject = x.get("refObject", {})
-            restrictionInfo = refObject.get("restrictionInfo", {})
+            itemBasicInfo = x.get("itemBasicInfo") or {}
+            refObject = x.get("refObject") or {}
+            restrictionInfo = refObject.get("restrictionInfo") or {}
 
             self.name.append(itemBasicInfo.get("name"))
             self.bubbleId.append(refObject.get("bubbleId"))
             self.bannerImage.append(refObject.get("bannerImage"))
             self.backgroundImage.append(refObject.get("backgroundImage"))
             self.resourceUrl.append(refObject.get("resourceUrl"))
             self.value.append(restrictionInfo.get("restrictValue"))
@@ -2331,17 +2358,17 @@
         self.icon = []
         self.value = []
         self.smallIcon = []
 
     @property
     def StoreStickers(self):
         for x in self.json:
-            refObject = x.get("refObject", {})
-            itemBasicInfo = x.get("itemBasicInfo", {})
-            restrictionInfo = refObject.get("restrictionInfo", {})
+            refObject = x.get("refObject") or {}
+            itemBasicInfo = x.get("itemBasicInfo") or {}
+            restrictionInfo = refObject.get("restrictionInfo") or {}
 
             self.id.append(refObject.get("collectionId"))
             self.name.append(itemBasicInfo.get("name"))
             self.icon.append(itemBasicInfo.get("icon"))
             self.value.append(restrictionInfo.get("restrictValue"))
             self.smallIcon.append(refObject.get("smallIcon"))
```

### Comparing `amino.light.py-0.1.2/AminoLightPy/socket.py` & `amino.light.py-0.1.3/AminoLightPy/socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/AminoLightPy/sub_client.py` & `amino.light.py-0.1.3/AminoLightPy/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/LICENSE` & `amino.light.py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/PKG-INFO` & `amino.light.py-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 
 <h1 align="center">AmioLightPy</h1>
 
-![gif](https://d142ifyzxiteda.cloudfront.net/s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
+
 
 <p align="center">
 AminoApps python framework to create bots and scripts easily.
 </p>
 
 <p align="center">
     <a href="https://github.com/AugustLigh/AminoLightPy/releases"><img src="https://img.shields.io/github/release/AugustLigh/AminoLightPy.svg" alt="GitHub release" />
```

#### html2text {}

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.2 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.3 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 Requires-Dist: websocket-client
                            ************ AAmmiiooLLiigghhttPPyy ************
-![gif](https://d142ifyzxiteda.cloudfront.net/
-s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-
-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-
-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-
-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/
+ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
```

### Comparing `amino.light.py-0.1.2/README.md` & `amino.light.py-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <h1 align="center">AmioLightPy</h1>
 
-![gif](https://d142ifyzxiteda.cloudfront.net/s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
+
 
 <p align="center">
 AminoApps python framework to create bots and scripts easily.
 </p>
 
 <p align="center">
     <a href="https://github.com/AugustLigh/AminoLightPy/releases"><img src="https://img.shields.io/github/release/AugustLigh/AminoLightPy.svg" alt="GitHub release" />
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
                            ************ AAmmiiooLLiigghhttPPyy ************
-![gif](https://d142ifyzxiteda.cloudfront.net/
-s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-
-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-
-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-
-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/
+ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
```

### Comparing `amino.light.py-0.1.2/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.3/amino.light.py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Best Amino.py alternative
 Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 
 <h1 align="center">AmioLightPy</h1>
 
-![gif](https://d142ifyzxiteda.cloudfront.net/s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
+
 
 <p align="center">
 AminoApps python framework to create bots and scripts easily.
 </p>
 
 <p align="center">
     <a href="https://github.com/AugustLigh/AminoLightPy/releases"><img src="https://img.shields.io/github/release/AugustLigh/AminoLightPy.svg" alt="GitHub release" />
```

#### html2text {}

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.2 Summary: Best
+Metadata-Version: 2.1 Name: amino.light.py Version: 0.1.3 Summary: Best
 Amino.py alternative Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight License: MIT Keywords:
 amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino-
 bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight,aminolightpy,amino.py
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 Requires-Dist: websocket-client
                            ************ AAmmiiooLLiigghhttPPyy ************
-![gif](https://d142ifyzxiteda.cloudfront.net/
-s3qk21%2Fpreview%2F57156938%2Fmain_large.gif?response-content-
-disposition=inline%3Bfilename%3D%22main_large.gif%22%3B&response-content-
-type=image%2Fgif&Expires=1712770066&Signature=LGr3nJ2CpCtpLryFHYP7rZlXtHFEfad9BbpxIXBAo0W7LBbdVQaLxNQHYmZHGpDNc67aec9sdJuXBnA3sA9KS3DvbLkNOTPaJwUNoVOF1MGxiX30TUto57peJ0lI99vFQwfeSZJF6FW6Q02YfgVhXa12L30mCZv49jFp0crKkMfBx85jOJMuYLbMdNNBHAsB3RKIj6a9ISNIxcJSZ2RyZCmqA8DqkDIdyBOZmodgS3TsL~orHDMwNdL6OSsKqBA3P5gT67erTrSGJM9Aw4ijC~SQADAmBdgpuT3YRx2J4ZOg9hGHAYb37gpTCc~KP8Ea3fl4xJzrlBVpXZrigccc-
-w__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ)
+![IMG_1363](https://github.com/AugustLigh/AminoLightPy/assets/125802350/
+ba1ae102-dee9-45ab-95c4-f5c5e0249d26)
          AminoApps python framework to create bots and scripts easily.
                         _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_]_[_D_o_c_s_]_[_l_i_c_e_n_c_e_]
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
```

### Comparing `amino.light.py-0.1.2/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.3/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.2/setup.py` & `amino.light.py-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from setuptools import setup, find_packages
 from os import path
+from setuptools import setup, find_packages
 
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 keywords = [
-    'amino',
-    'aminoapps',
-    'amino.fix',
-    'amino.light',
-    'amino.ligt.py',
-    'AminoLightPy',
-    'amino-bot',
-    'narvii',
-    'medialab',
-    'api',
-    'python',
-    'python3',
-    'python3.x',
-    'minori',
-    'august',
-    'augustlight',
-    'aminolightpy',
-    'amino.py'
+    "amino",
+    "aminoapps",
+    "amino.fix",
+    "amino.light",
+    "amino.ligt.py",
+    "AminoLightPy",
+    "amino-bot",
+    "narvii",
+    "medialab",
+    "api",
+    "python",
+    "python3",
+    "python3.x",
+    "minori",
+    "august",
+    "augustlight",
+    "aminolightpy",
+    "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.2",
+    version="0.1.3",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     keywords=keywords,
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

