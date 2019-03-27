---
title: KeywordCategoryResult Data Object - Ad Insight
ms.service: bing-ads-ad-insight-service
ms.topic: article
author: eric-urban
ms.author: eur
description: Defines an object that contains the keyword and a list of keyword categories that the keyword might belong to.
---
> [!IMPORTANT]
> The Bing Ads API Version 13 preview documentation is subject to change. To view version 12 content, use the version selector near the table of contents at the top and left side of the page.

# KeywordCategoryResult Data Object - Ad Insight
Defines an object that contains the keyword and a list of keyword categories that the keyword might belong to.

## Syntax
```xml
<xs:complexType name="KeywordCategoryResult" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:sequence>
    <xs:element minOccurs="0" name="Keyword" nillable="true" type="xs:string" />
    <xs:element minOccurs="0" name="KeywordCategories" nillable="true" type="tns:ArrayOfKeywordCategory" />
  </xs:sequence>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="keyword"></a>Keyword|The keyword being categorized.|**string**|
|<a name="keywordcategories"></a>KeywordCategories|An array of [KeywordCategory](keywordcategory.md) objects that contains a keyword category and a score that indicates the confidence that the keyword belongs to that keyword category.|[KeywordCategory](keywordcategory.md) array|

## Requirements
Service: [AdInsightService.svc v13](https://adinsight.api.bingads.microsoft.com/Api/Advertiser/AdInsight/v13/AdInsightService.svc)  
Namespace: https\://bingads.microsoft.com/AdInsight/v13  

## Used By
[GetKeywordCategories](getkeywordcategories.md)  